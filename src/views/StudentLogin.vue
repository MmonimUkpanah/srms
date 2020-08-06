<template>
  <div class="about">
    <div>
      <div>
    
      </div>
    <div class="one">
      <div class="one1">
        <h2>Check your results</h2>
      </div>
      
      <div class="one2">
        <form @submit.prevent="checkResult" >
          <label for="Username"><h6>Reg Number</h6> </label><br>
          <input type="text" placeholder="13/EG/CE/505" v-model="logindetails.reg_no" ><br>
          
         <div class="grid">
           <div>
             <label for=""><h6>Session</h6></label>
             <div class="input-group" >
              <select class="custom-select" id="inputGroupSelect04" aria-label="Example select with button addon" v-model="logindetails.sessions_id">
                <option  selected disabled>Session</option>
                <option v-for="session in sessions" :key="session.id" >{{session.name}}</option>
                
                
              </select>
  
            </div> 
           </div>
           <div>
             <label for=""><h6>Semester</h6></label>
             <div class="input-group" >
              <select class="custom-select" id="inputGroupSelect04" aria-label="Example select with button addon"  v-model="logindetails.semesters_id">
                <option  selected disabled>Semester</option>
                <option v-for="semester in semesters" :key="semester.id">{{semester.name}}</option>
              </select>
  
            </div> 
           </div>
           
            
         </div>
          <div class="center">
            <input type="submit" value="Check Results" >
          </div>
          
        </form>
        
      </div>
    </div>
    </div>
    <div>
      
    </div>
  </div>
</template>

<script>
import axios from 'axios'
export default {
   data(){
     return{
       logindetails: {
         reg_no: "",
         sessions_id:  "",
        semesters_id : ""
       },
       result:[],
       sessions: [],
       semesters: [],
       resultDetails:[]
     }
   },
   methods:{
     getSession( ){
       axios.get('https://srms-project.herokuapp.com/api/sessions').then(res => {
         this.sessions= res.data.data;
       }),console.log(this.sessions)
     },
     getSemester( ){
       axios.get('https://srms-project.herokuapp.com/api/semesters').then(res => {
         this.semesters= res.data.data
       }),console.log(this.semesters)
     },
       
     checkResult(){
       const formData=new FormData();
       formData.append('reg_no',this.logindetails.reg_no);
       formData.append('sessions_id',this.logindetails.sessions_id);
       formData.append('semesters_id',this.logindetails.semesters_id);
       axios.post("https://srms-project.herokuapp.com/api/student-result",formData).then(res=>{
         this.resultDetails = res.data;
          console.log(this.resultDetails);
          this.$router.push('/Result');
          
        
       });
     }
   },
   created(){
     this.getSession(),
     this.getSemester(),
     this.checkResult()
   },
   
}
</script>

<style scoped>
  .one{
    margin-left: 30%;
    margin-right: 30%;
    margin-top: 100px;
    margin-bottom: 100px;
    
  }
  
  .one1{
    text-align: center;
  }
  .one1 h2{
    color: #424B5F;
    font-size: 36px;
    margin-bottom: 30px;
  }
  .one2 label{
    color: #333333;
  }
  .one2 input{
    width: 100% !important;
    margin-bottom: 10px;
    background: #FFFFFF;
    border: 2px solid #E0E0E0;
    border-radius: 4px;
    padding: 5px 10px;
  }
  .btn1{
    width: 40% !important;
    background: #698AFE;
    border-radius: 4px;
    border: none;
    padding-top: 10px;
    padding-bottom: 10px;
    color: #FFFFFF;
    margin-top: 30px;
  }
  .btn2{
    width: 100%;
    background: #698AFE;
    border-radius: 4px;
    border: none;
    padding-top: 10px;
    padding-bottom: 10px;
    color: #FFFFFF;
    margin-top: 10px;
  }
  .center{
      text-align: center;
      margin-top: 30px;
  }
  .center input{
    width: 100%;
    background: #424B5F;
    border-radius: 4px;
    border: none;
    padding-top: 10px;
    padding-bottom: 10px;
    color: #FFFFFF;
    margin-top: 10px !important;
  }
  .grid{
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-gap: 1rem;
  }

  @media (max-width:567px){
    .one{
    margin-left: 20px;
    margin-right: 20px;
    margin-top: 100px;
    margin-bottom: 100px;
  }
  .grid{
    display: grid;
    grid-template-columns: 1fr;
    grid-gap: 1rem;
  }
  }


  @media (min-width:568px) and (max-width:768px){
    .one{
    margin-left: 20% !important;
    margin-right: 20% !important;
    margin-top: 100px;
    margin-bottom: 100px;
  }
  }

  @media (min-width:769px) and (max-width:1200px){

    .one{
    margin-left: 20% !important;
    margin-right: 20% !important;
    margin-top: 100px;
    margin-bottom: 150px;
  }
  }
</style>


