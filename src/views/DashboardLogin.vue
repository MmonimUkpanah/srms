<template>
  <div class="about">
    <div class="one">
      <div class="one2">
          <router-link to="/StudentLogin" ><button class="btn1">Login as Student</button></router-link>

          <router-link to="/AdminLogin" ><button class="btn1">Login as Admin</button></router-link>
        
        
      </div>
    </div>
  </div>
</template>

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
    color: #698AFE;
    font-size: 36px;
    margin-bottom: 30px;
  }
  .one2 label{
    color: #333333;
  }
  .one2 input{
    width: 100% !important;
    margin-top: -20px !important;
    margin-bottom: 30px;
    background: #FFFFFF;
    border: 2px solid #E0E0E0;
    border-radius: 4px;
    padding: 5px 10px;
  }
  .btn1{
    width: 100% !important;
    background: #698AFE;
    border-radius: 4px;
    border: none;
    padding-top: 5px;
    padding-bottom: 5px;
    color: #FFFFFF;
    margin-top: 10px;
    margin-bottom: 30px;
    
  }

  @media (max-width:567px){
    .one{
    margin-left: 20px;
    margin-right: 20px;
    margin-top: 100px;
    margin-bottom: 100px;
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
