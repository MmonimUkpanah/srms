<template>
    <div class="one">
        <div class="one1">
            <div class="one3">
                <h2>Student Result Details</h2>
            </div>
            
        <div>
            <p>Student Name:</p>
            <p>Registration Number:</p>
            <p>Session:</p>
            <p>Semester:</p>
        </div>
        <div>
            <div class="table-responsive">
                            <table class="table">
        <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">Course</th>
      <th scope="col">Mark</th>
      <th scope="col">Grade</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th scope="row">3</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
        </table>
            </div>
    <div>
        <p>Remarks: </p>
    </div>
    <div class="one2">
        <img src="../assets/download.png" alt="">
    </div>
        </div>
        </div>
        
    </div>
</template>
<script>
export default {
    data(){
        return{
            studentdetails:{
                studentname: " ",
                registrationnumber: " ",
                session: " ",
                semester:" ",
                courses: " ",
                mark: " ",
                grade: " ",
                remarks: " ",
            },
            students:{

            }

        }
    },
    methods: {
        getResult(){
            axios.post("https://srms-project.herokuapp.com/api/student-result",formData).then(res=>{
          console.log(res.data)});
        },
        created(){
            getResult()
        }
        
        
    }
}
</script>
<style scoped>
    .one{
        margin-top: 50px;
        margin-left: 20%;
        margin-right: 20%;
        background: #E5E5E5 ;
        margin-bottom: 50px;
        border-radius: 10px;
    }
    .one1{
        padding: 30px 30px;
    }
    .one2 img{
        width: 5%;
    }
    .one2{
        text-align: center;
    }
    .one3{
        text-align: center;
    }

    @media(max-width: 567px){
        .one{
        margin-top: 50px;
        margin-left: 20px;
        margin-right: 20px;
        background: #E5E5E5 ;
        margin-bottom: 50px;
    }
    .one2 img{
        width: 10%;
    }
    }
</style>