<template>
    <div>
        <section class="one">
            <nav class="navbar navbar-expand-lg navbar-light">
  <a class="navbar-brand" href="#"><img src="../assets/Group 6.png" alt=""></a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarTogglerDemo02" aria-controls="navbarTogglerDemo02" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>

  <div class="collapse navbar-collapse one1" id="navbarTogglerDemo02">
    <ul class="navbar-nav ml-auto mt-2 mt-lg-0">
      <li class="nav-item active">
        
        <router-link to="/" class="nav-link">Home <span class="sr-only">(current)</span></router-link>
      </li>
      <li class="nav-item">
        <router-link to="/StudentLogin" class="nav-link" href="#">Check  Results</router-link>
      </li>
      <li class="nav-item">
        <router-link to="/AdminLogin" class="nav-link" href="#">Dashboard</router-link>
      </li>

    </ul>
    
  </div>
</nav>
        </section>
        
    </div>
</template>


<script>
export default {
    
}
</script>

<style scoped>
    .one{
        margin-left: 100px;
        margin-right: 100px;
    }
    nav ul li{
        margin-left: 50px !important;
    }
    nav ul li a{
        color: #424B5F !important;
    }
    nav ul li a:hover{
        color: #698AFE !important;
    }
    .btn1{
        background: #698AFE;
        border-radius: 3px;
        color: white;
        padding: 8px 30px;
        border: none;
        margin-left: 50px;
    }


    @media(max-width: 576px){
        .one{
        margin-left: 10px;
        margin-right: 10px;
    }
    nav ul li{
        margin-left: 0px !important;
    }
    .btn1{
        background: #698AFE;
        border-radius: 3px;
        color: white;
        padding: 8px 30px;
        border: none;
        margin-left: 0px;
    }
    }

    @media(min-width: 577px) and (max-width: 768px){
        .one{
        margin-left: 20px;
        margin-right: 20px;
    }
    nav ul li{
        margin-left: 0px !important;
    }
    .btn1{
        background: #698AFE;
        border-radius: 3px;
        color: white;
        padding: 8px 30px;
        border: none;
        margin-left: 0px;
    }
    }



</style>