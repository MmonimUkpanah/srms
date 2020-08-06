<template>
  <div >
      <div class="one">
           <section class="one1">
          <h2>What are you looking for?</h2>
          <p>All the resources you need to get the most out of our school, quickly and effectively! </p>
          <input type="text" placeholder="Search...">
      </section>
      </div>
     
      <section class="two">
          <div class="grid">
              <div class="two1">
                  <img src="../assets/Group.png" alt="">
                  <h6>Resources</h6>
                  <p>Check our student resources & guidelines before using the website.</p>
              </div>
              <div class="two1">
                  <img src="../assets/Group (1).png" alt="">
                  <h6>Forum</h6>
                  <p>Input your registration number and ask for help on our school forum.</p>
              </div>
              <div class="two1">
                  <img src="../assets/Group (2).png" alt="">
                  <h6>Contact Us</h6>
                  <p>Contact us for complaints. We'll do everything to help you.</p>
              </div>
              
          </div>  
      </section>
      <section class="three"> 
          <div>
              <div class="grid2">
                  <div>
                      <h5>Popular Semesters</h5>
                      <div class="three1">
                          <p><img src="../assets/link.png" alt=""> 2019/2020</p>
                          <p><img src="../assets/link.png" alt=""> 2018/2019</p>
                          <p><img src="../assets/link.png" alt=""> 2017/2018</p>
                          <p><img src="../assets/link.png" alt=""> 2016/2017</p>
                          <p><img src="../assets/link.png" alt=""> 2015/2016</p>
                      </div>
                  </div>
                  <div>
                      <h5>Lastest Results</h5>
                        <div class="three1">
                            <p><img src="../assets/Shape (4).png" alt=""> Engineering Faculty</p>
                            <p><img src="../assets/Shape (4).png" alt=""> Basic Science and Technology</p>
                            <p><img src="../assets/Shape (4).png" alt=""> Social Sciences</p>
                            <p><img src="../assets/Shape (4).png" alt=""> Faculty of Medicine</p>
                            <p><img src="../assets/Shape (4).png" alt=""> Faculty of Education</p>
                        </div>  
                  </div>
                  <div>
                      <h5>From Our Resources</h5>
                      <div class="three1">
                          <p><img src="../assets/chat-2.png" alt=""> How to set up a Laboratory by : <span>James Gordon</span></p>
                          <p><img src="../assets/chat-2.png" alt=""> Check out our history hub by : <span>Kevin Dart</span></p>
                          <p><img src="../assets/chat-2.png" alt=""> Our rules and guidelines by : <span>Neville Griff</span></p>
                          <p><img src="../assets/chat-2.png" alt=""> Welcome to our university by : <span>Daya Chitan</span></p>
                          <p><img src="../assets/chat-2.png" alt=""> How you can get a First Class by : <span>James Gordon</span></p>
                      </div>
                  </div>
              </div>
          </div>
      </section>
        

    
  </div>
</template>

<script>

export default {
 
}
</script>

<style scoped>
    *{
        margin: 0px;
        padding: 0px;
        box-sizing: border-box;
    }
    .one{
        background: linear-gradient(180deg, #FFFFFF 0%, #F6F9FC 100%);
        
    }
    .one1{
        margin-left: 32%;
        margin-right: 32%;
        text-align: center;
        padding-top: 50px;
        padding-bottom: 150px;
    }
    .one1 h2{
        font-size: 36px;
        color: #424B5F;
        margin-bottom: 30px;
    }
    .one1 p{
        color: #67758D;
        font-size: 20px;
        margin-bottom: 40px;
    }
    .one1 input{
        border-radius: 25px;
        border: none;
        color: #97A4BA;
        font-size: 16px;
        width: 100% !important;
        padding: 8px 15px;
        background: #EAF0F7 url(../assets/Shape.png) no-repeat center;
        background-position-x: 95% !important;
    }
    .grid{
        margin-left: 12%;
        margin-right: 12%;
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        grid-gap: 3rem;
        text-align: center;
    }
    .two{
        margin-top: -100px;
    }
    .two1{
        background: #FFFFFF;
        border: 1px solid #F6F9FC;
        box-shadow: 0px 10px 20px -10px rgba(0, 0, 0, 0.15);
        border-radius: 4px;
        padding: 20px 30px;
    }
    .two1 img{
        width: 20%;
        margin-bottom: 20px;
    }
    .two1 p{
        font-size: 16px;
        color: #67758D;
    }
    .two2{
        background: #F6F9FC;
        border-radius: 30px;
        margin-left: 20%;
        margin-right: 20%;
        margin-top: 50px;
        padding: 7px 20px;
    }
    .two2 p{
        color: #424B5F;
    }
    .btn1{
        background: #51C81C;
        border-radius: 30px;
        border: none;
        padding: 10px 20px;
        margin-right: 10px;
        color: #FFFFFF;
    }
    .two3{
        color: #698AFE;
    }
    .three{
        background: #424B5F;
        margin-top: 50px;
        margin-bottom: 100px;
    }
    .grid2{
        margin-left: 8%;
        margin-right: 8%;
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        padding-top: 50px;
        padding-bottom: 50px;
    }
    .grid2 h5{
        color: #FFFFFF;
        font-size: 18px;
        margin-bottom: 25px;
    }
    .three1 p{
        color: white;
        font-size: 16px;
        margin-bottom: 15px;
    }
    .three1 img{
        margin-right: 5px;
    }
    .four{
        margin-left: 8%;
        margin-right: 8%;
        margin-top: 80px;
    }
    .hr1{
        background: #DEE5EF;
        border-radius: 2px;
        width: 40px;
        height: 3px;
        margin-top: 5px;
    }
    .grid3{
        margin-right: 25%;
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-gap: 2rem;
    }


    @media(max-width: 567px){
        .one1{
        margin-left: 20px;
        margin-right: 20px;
        text-align: center;
        padding-top: 50px;
        padding-bottom: 150px;
    }
    .one1 h2{
        font-size: 36px;
        color: #424B5F;
        margin-bottom: 30px;
    }
    .one1 p{
        color: #67758D;
        font-size: 20px;
        margin-bottom: 40px;
    }
    .one1 input{
        border-radius: 25px;
        border: none;
        color: #97A4BA;
        font-size: 16px;
        width: 100% !important;
        padding: 8px 15px;
        background: #EAF0F7 url(../assets/Shape.png) no-repeat center;
        background-position-x: 95% !important;
    }
    .grid{
        margin-left: 20px;
        margin-right: 20px;
        display: grid;
        grid-template-columns: 1fr ;
        grid-gap: 1rem;
        text-align: center;
    }
    .two{
        margin-top: 30px;
    }
    .two1{
        background: #FFFFFF;
        border: 1px solid #F6F9FC;
        box-shadow: 0px 10px 20px -10px rgba(0, 0, 0, 0.15);
        border-radius: 4px;
        padding: 20px 30px;
    }
    .two1 img{
        width: 20%;
        margin-bottom: 20px;
    }
    .two1 p{
        font-size: 16px;
        color: #67758D;
    }
    .two2{
        display: none;
    }
    .two2 p{
        color: #424B5F;
    }
    .btn1{
        background: #51C81C;
        border-radius: 30px;
        border: none;
        padding: 10px 20px;
        margin-right: 10px;
        color: #FFFFFF;
    }
    .two3{
        color: #698AFE;
    }
    .three{
        background: #424B5F;
        margin-top: 50px;
        margin-bottom: 100px;
    }
    .grid2{
        margin-left: 20px;
        margin-right: 20px;
        display: grid;
        grid-template-columns: 1fr ;
        padding-top: 50px;
        padding-bottom: 50px;
        text-align: center;
    }
    .grid2 h5{
        color: #FFFFFF;
        font-size: 18px;
        margin-bottom: 25px;
    }
    .three1 p{
        color: white;
        font-size: 16px;
        margin-bottom: 15px;
    }
    .three1 img{
        margin-right: 5px;
    }
    .four{
        margin-left: 8%;
        margin-right: 8%;
        margin-top: 80px;
    }
    .hr1{
        background: #DEE5EF;
        border-radius: 2px;
        width: 40px;
        height: 3px;
        margin-top: 5px;
    }
    .grid3{
        margin-right: 25%;
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-gap: 2rem;
    }


    }
    
</style>
