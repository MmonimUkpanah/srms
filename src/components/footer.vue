<template>
    <div class="one">
        <div class="one1">
            <div>
                <div class="one2">
                    <img src="../assets/Group 6.png" alt="" class="one3">
                <div class="one4">
                    <img src="..\assets\Facebook__x28_alt_x29_.png" alt="">
                    <img src="..\assets\Shape (1).png" alt="">
                    <img src="..\assets\Shape (2).png" alt="">
                    <img src="..\assets\Shape (3).png" alt="">
                </div>
                </div>
                
            </div>
            <div>
                <h5>School</h5>
                <p>About Us</p>
                <p>Blog</p>
                <p>Contact</p>
                <p>Learn more</p>
            </div>
            <div>
                <h5>Semesters</h5>
                <p>2019/2020</p>
                <p>2018/2019</p>
                <p>2018/2017</p>
            </div>
            <div>
                <h5>Resources</h5>
                <p>School guides</p>
                <p>School Rules</p>
                <p>Courses</p>
            </div>
        </div>
        <hr>
        <div class="one5">
            <p >&copy; 2020 StudMG | All Rights Reserved</p>
        </div>
        
    </div>
</template>

<script>
export default {
    
}
</script>


<style scoped>
    .one{
        margin-left: 115px;
        margin-right: 100px;
    }
    .one1{
        display: grid;
        grid-template-columns: 1fr 1fr 1fr 1fr;
        grid-gap: 2rem;
    }
    .one1 h5{
        margin-bottom: 30px;
        color: #283040;
        font-size: 18px;
    }
    .one1 p{
        color: #67758D;
        font-size: 16px;
    }
    .one2{
        padding-top: 40px;
    }
    .one3{
        margin-bottom: 25px;
    }
    .one4 img{
        margin-right: 20px;
    }
    hr{
        background: #EAF0F7;
    }
    .one5 p{
        color: #67758D;
    }


    @media(max-width: 567px){
        .one{
        margin-left: 25px;
        margin-right: 20px;
        }
        .one1{
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-gap: 1rem;
        text-align: center;
        }
        .one4 img{
        margin-right: 10px;
        margin-bottom: 20px;
        }
        .one1 h5{
        margin-bottom: 20px;
        color: #283040;
        font-size: 18px;
        }
        .one5{
            text-align: center;
        }
        
    }


    @media(min-width:568px ) and (max-width: 768px){
        .one{
        margin-left: 35px;
        margin-right: 20px;
        }
        .one1{
        display: grid;
        grid-template-columns: 1fr 1fr 1fr 1fr;
        grid-gap: 1rem;
        text-align: left;
        }
        .one4 img{
        margin-right: 10px;
        margin-bottom: 20px;
        }
        .one1 h5{
        margin-bottom: 20px;
        color: #283040;
        font-size: 18px;
        }
        .one5{
            text-align: center;
        }
    }
</style>