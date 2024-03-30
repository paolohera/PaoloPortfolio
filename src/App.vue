<template>
  <body>
    
<nav class="navbar">
<h1 class="logo">hera</h1> 
<ul class="links">
    
  <li><a class="hover-underline-animation" href="#bout">ABOUT ME</a></li>
        <li><a class="hover-underline-animation" href="#rec">PROJECTS</a></li>
        <li><a class="hover-underline-animation" href="#conts1">CONTACT</a></li>

</ul>
</nav>
<div class="intro"><span class="hi">Hi there! Im Paolo Patigdas </span> <br>  a Web Designer and Developer from Cordova Public College</div>
   
<div class="imgcont2"></div>
    <div class="imgcont1"></div>
    <div class="imgcont">
        <img class="pic" src="/src/assets/pao.png">
    </div>
    <div class='btn-cont'>
  <a class='btn' href='#' @click="handleSweetAlert">
   MESSAGE ME
    <span class='line-1'></span>
    <span class='line-2'></span>
    <span class='line-3'></span>
    <span class='line-4'></span>
  </a>
</div>
<div id="bout">
  ABOUT ME
</div>
    <div class="container">
        <div class="conts">
            <br><br>
            I am an IT college student specializing in network configuration, proficient in operating system installation, hardware, and software setup. My coding expertise lies in HTML, CSS, JavaScript, and Vue.js, where I am passionate about crafting immersive and user-friendly web experiences. Beyond my technical skills, I am dedicated to continuous learning and staying updated with the latest advancements in the IT industry, always eager to tackle new challenges and expand my knowledge.
        </div>
      <div class="lenks"><a href="https://web.facebook.com/paopao.hera"><img class="face" src="/src/assets/face.png" alt=""></a>
      <a href="https://github.com/paolohera"><img class="face" src="/src/assets/get.png" alt=""></a>
      <a href="mailto:paolopatigdas123@gmail.com"><img class="face" src="/src/assets/mail.png" alt=""></a>
    </div>
    </div>
  
   <div id="rec"> RECENT PROJECTS</div>
  
    <div class="card-list">
        <div href="#" class="card-item">
            <img class="img1" src="/src/assets/port.png" alt="Card Image">
            <span class="designer">Portfolio</span>
            <h3>A Website Portfolio created by me Using VueJS and Hardcoded CSS</h3>
            <img class="git" src="/src/assets/git.png">
        </div>
        <div href="#" class="card-item">
            <img class="img1" src="/src/assets/ola.png" alt="Card Image">
            <span class="designer">Room Reservation</span>
            <h3>A Web Application created by my Team Using VueJS, NodeJs, HTML&CSS. and I was assigned to be the front end.</h3>
            <img  class="git" src="/src/assets/git.png">
        </div>
        <div href="#" class="card-item">
            <img class="img1" src="/src/assets/olas.png" alt="Card Image">
            <span class="designer">Static Website</span>
            <h3>A Static Website created by me using HTML & CSS. Its purpose is only to guide and let users view what Olango Island Has.</h3>
            <a href="https://github.com/paolohera/featuringOlangoIsland"><img class="git" src="/src/assets/git.png"></a>
        </div>
        <div href="#" class="card-item">
            <img class="img1" src="/src/assets/aqua.png" alt="Card Image">
            <span class="designer">aquatic marketplace</span>
            <h3>A prototype web application created by me using HTML & CSS.</h3>
            <img class="git" src="/src/assets/git.png">
        </div>
        <div href="#" class="card-item">
            <img class="img1" src="/src/assets/wtd.png" alt="Card Image">
            <span class="designer">Online Trading System</span>
            <h3>A Prototype Website created by me using HTML & CSS.</h3>
            <img class="git" src="/src/assets/git.png">
        </div>
        <div href="#" class="card-item">
            <img class="img1"  src="/src/assets/cpc.png" alt="Card Image">
            <span class="designer">Student Management</span>
            <h3>A web application created by Me and Michael John Tampus use for managing student information using PHP, HTML & CSS </h3>
            <img class="git" src="/src/assets/git.png">
        </div>
    </div>
    
   <div id="conts1">CONTACT DETAILS</div>

<div class='btn1'>
  <div class='btn' href='#'>
   
    <span class='line-1'></span>
    <span class='line-2'></span>
    <span class='line-3'></span>
    <span class='line-4'></span>
  </div>
  <br><br>
  <h1 class="email">Email</h1>
  <p>paolopatigdas123@gmail.com
    <br>paolohera01@gmail.com
  </p><hr class="her">
  <h1 class="sa">Social Accounts</h1>
  <p>Facebook: https://web.facebook.com/paopao.hera
    <br>Instagram: @paolohera
  </p><hr class="her">
  <h1 class="pn">Phone Number</h1>
  <p>+639669118034</p><hr class="her">
  <h1 class="ha">Home Adress</h1>
  <p>Gun-ob Lapu-Lapu City, Cebu</p><hr class="her">
</div>

<div class="map" >
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1617.7456774798827!2d123.95078322737866!3d10.299798664774718!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x33a99934b1b55063%3A0x196b599a4839df94!2sGun%20ob%20lapu%20lapu%20city%20cebu!5e1!3m2!1sen!2sph!4v1711693840941!5m2!1sen!2sph" 
width="600" height="500" style="border:0;" 
allowfullscreen="" 
loading="lazy"  
 referrerpolicy="no-referrer-when-downgrade">
 </iframe>
</div>
<footer>
  <div class="pao">©Paolo Hera. All Rights Reserved.</div>
</footer>
  </body>
  
</template>

<script setup>
import Swal from 'sweetalert2'

const handleSweetAlert = async () => {
  const { value: text } = await Swal.fire({
    input: "textarea",
    inputLabel: "Message",
    inputPlaceholder: "Type your message here...",
    inputAttributes: {
      "aria-label": "Type your message here"
    },
    showCancelButton: true
  });

  if (text) {
    Swal.fire(text);
  }
}
</script>



<style scoped>
@import url('https://fonts.cdnfonts.com/css/technolab');
@import url('https://fonts.cdnfonts.com/css/trocchi-3');
@import url('https://fonts.cdnfonts.com/css/ruwudu');
footer{
  background-color: black;
  height: 50px;
  margin-top: 20%;
}
.lenks{
  margin-left: 13%;
}
.face{
  width: 50px;
  height: 50px;
  border-radius: 50%;
  margin-right: 10%;
  margin-top: 15%;
}
.pao{
  color: white;
  text-align: center;
  padding-top: 15px;
}
.swal2-shown {
  overflow: hidden !important;
}
.btn-cont {
  position: absolute;
  margin-top: 22%;
  margin-left: 27%;
  text-align: center;
}
.btn-cont .btn {
  padding-bottom: 15px;
  padding-top: 15px;
  position: absolute;
  width: 150px;
  border: 1px solid rgb(255, 255, 255);
  color: white;
  text-decoration: none;
  font-size: 10px;
  font-family: 'Technolab', sans-serif;
  text-transform: uppercase;
  letter-spacing: 2px;
  -webkit-font-smoothing: antialiased;
}
.btn-cont .btn:hover {
  border: none;
}
.btn-cont .btn:hover .line-1 {
  -webkit-animation: move1 1500ms infinite ease;
          animation: move1 1500ms infinite ease;
}
.btn-cont .btn:hover .line-2 {
  -webkit-animation: move2 1500ms infinite ease;
          animation: move2 1500ms infinite ease;
}
.btn-cont .btn:hover .line-3 {
  -webkit-animation: move3 1500ms infinite ease;
          animation: move3 1500ms infinite ease;
}
.btn-cont .btn:hover .line-4 {
  -webkit-animation: move4 1500ms infinite ease;
          animation: move4 1500ms infinite ease;
}
.btn-cont .line-1 {
  content: "";
  display: block;
  position: absolute;
  width: 1px;
  background-color: rgb(35, 255, 6);
  left: 0;
  bottom: 0;
}
.btn-cont .line-2 {
  content: "";
  display: block;
  position: absolute;
  height: 1px;
  background-color: rgb(35, 255, 6);
  left: 0;
  top: 0;
}
.btn-cont .line-3 {
  content: "";
  display: block;
  position: absolute;
  width: 1px;
  background-color: rgb(35, 255, 6);
  right: 0;
  top: 0;
}
.btn-cont .line-4 {
  content: "";
  display: block;
  position: absolute;
  height: 1px;
  background-color: rgb(35, 255, 6);
  right: 0;
  bottom: 0;
}

@-webkit-keyframes move1 {
  0% {
    height: 100%;
    bottom: 0;
  }
  54% {
    height: 0;
    bottom: 100%;
  }
  55% {
    height: 0;
    bottom: 0;
  }
  100% {
    height: 100%;
    bottom: 0;
  }
}

@keyframes move1 {
  0% {
    height: 100%;
    bottom: 0;
  }
  54% {
    height: 0;
    bottom: 100%;
  }
  55% {
    height: 0;
    bottom: 0;
  }
  100% {
    height: 100%;
    bottom: 0;
  }
}
@-webkit-keyframes move2 {
  0% {
    width: 0;
    left: 0;
  }
  50% {
    width: 100%;
    left: 0;
  }
  100% {
    width: 0;
    left: 100%;
  }
}
@keyframes move2 {
  0% {
    width: 0;
    left: 0;
  }
  50% {
    width: 100%;
    left: 0;
  }
  100% {
    width: 0;
    left: 100%;
  }
}
@-webkit-keyframes move3 {
  0% {
    height: 100%;
    top: 0;
  }
  54% {
    height: 0;
    top: 100%;
  }
  55% {
    height: 0;
    top: 0;
  }
  100% {
    height: 100%;
    top: 0;
  }
}
@keyframes move3 {
  0% {
    height: 100%;
    top: 0;
  }
  54% {
    height: 0;
    top: 100%;
  }
  55% {
    height: 0;
    top: 0;
  }
  100% {
    height: 100%;
    top: 0;
  }
}
@-webkit-keyframes move4 {
  0% {
    width: 0;
    right: 0;
  }
  55% {
    width: 100%;
    right: 0;
  }
  100% {
    width: 0;
    right: 100%;
  }
}
@keyframes move4 {
  0% {
    width: 0;
    right: 0;
  }
  55% {
    width: 100%;
    right: 0;
  }
  100% {
    width: 0;
    right: 100%;
  }
}

.conts{
  font-family: 'Trocchi', sans-serif;
  font-weight: 100;
  color: white;
}
#conts1{
  color: white;
  font-family: 'Technolab', sans-serif; 
  font-size: 25px;
  width: 80%;
  height: 50px;
  border-top: 1px solid white;
  border-bottom: 1px solid rgb(35, 255, 6);
  margin-top: 10%;
  margin-left: 10%;
  text-align: center;
  padding-top: 10px;
}
#bout{
  color: white;
  font-family: 'Technolab', sans-serif; 
  font-size: 25px;
  width: 80%;
  height: 50px;
  border-top: 1px solid white;
  border-bottom: 1px solid rgb(35, 255, 6);
  margin-top: 50%;
  margin-left: 10%;
  text-align: center;
  padding-top: 10px;
}
#rec{
  color: white;
  font-family: 'Technolab', sans-serif; 
  font-size: 25px;
  width: 80%;
  height: 50px;
  border-top: 1px solid white;
  border-bottom: 1px solid rgb(35, 255, 6);
  margin-top: 15%;
  margin-left: 10%;
  text-align: center;
  padding-top: 10px;
}
body{
  background-color: rgb(33, 33, 34);
  height: 540vh;
  width: 100%;
  margin-left: 0;
  padding-top: 0;
 
}
.intro{
  font-family: 'Technolab', sans-serif; 
  color : white ;
    font-size: 15px;
    width: 40%;
    position: absolute;
    margin-top: 12%;
    margin-left: 13%;
    text-align: center;
    
}
.hi{
  color: rgb(81, 255, 0);
  font-size: 28px;
}
.logo{
  font-family: 'Technolab', sans-serif;                                              
    color : white ;
    font-size: 50px;
    margin-top: 15px;
    position: absolute;
    margin-left: 5%;
   cursor: pointer;
}

nav {
    background-color: transparent;
    height: 80px;
    width: 100%;
    text-transform: uppercase;  
}

nav ul {
    float: right;
    margin-top: 2px;
    margin-right: 5%;
}

nav ul li {
    display: inline-block;
    line-height: 30px;
    margin: 0 10px;
    margin-top: 20px;
}

nav ul li a {
    font-size: 10px;
    padding: 5px 13px;
    text-decoration: none;
    color: white;
    font-family: 'Technolab', sans-serif;
                                                
}

.hover-underline-animation {
    display: inline-block;
    position: relative;
    color:white ;
  }
  
  .hover-underline-animation:after {
    content: '';
    position: absolute;
    width: 100%;
    transform: scaleX(0);
    height: 2px;
    bottom: 0;
    left: 0;
    background-color: rgb(35, 255, 6);
    transform-origin: bottom right;
    transition: transform .5s ease-out;
  }
  
  .hover-underline-animation:hover:after {
    transform: scaleX(1);
    transform-origin: bottom left;
  }

  .pic{
    
    width: 270px;
    height: 430px;
    border-radius: 5px;
   
   }
   .container{
    color: white;
    width:60%;
    margin-left: 20%;
    margin-top: 5%;
    text-align: center;
    padding: 5px;
    font-family: 'Ruwudu', sans-serif; 
    border-radius: 5px;
    font-size: 15px;
   }
   .imgcont{
    border: 1px solid rgb(35, 255, 6);
    width: 270px;
    height: 430px;
    position: absolute;
    align-items: center;
    margin-left: 60%;
    border-radius: 5px;
    display: flex;
    margin-top: 5%;
   }
   .imgcont1{
    border: 1px solid white;
    width: 270px;
    height: 430px;
    position: absolute;
    align-items: center;
    margin-left: 61%;
    border-radius: 5px;
    display: flex;
    margin-top: 4%;
   }
   .imgcont2{
    border: 1px solid rgb(35, 255, 6);
    width: 270px;
    height: 430px;
    position: absolute;
    align-items: center;
    margin-left: 62%;
    border-radius: 5px;
    display: flex;
    margin-top: 3%;
   }
   

.card-list {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    max-width: 1250px;
    margin: 100px auto;
    padding: 20px;
    gap: 20px;
    
}
.card-list .card-item {
    background:  transparent;
    padding: 26px;
    border-radius: 8px;
    box-shadow: 0px 5px 10px rgba(0, 0, 0, 0.04);
    list-style: none;
    text-decoration: none;
    border: 1px solid white;
    transition: border 0.5s ease;
}

.card-list .card-item .img1 {
    width: 100%;
    height: 40%;
    border-radius: 8px;
    object-fit: cover;
}
.card-list span {
    display: inline-block;
    background: #F7DFF5;
    margin-top: 32px;
    padding: 8px 15px;
    font-size: 12px;
    border-radius: 50px;
    font-weight: 600;
}

.card-list .designer {
    background-color: #d1e8ff;
    color: #2968a8;
    font-family: 'Technolab', sans-serif;
}

.card-item h3 {
    color: white;
    font-size: 18px;
    margin-top: 28px;
    font-family: 'Ruwudu', sans-serif;
    font-weight: 100;
}
.git{
    width: 100px;
    height: 40px;
    border-radius: 5px;
    cursor: pointer;
    margin-left: 33%;
    transition: 0.5s;
}
.git:hover{
    transform: scale(1.1);
}
@media (max-width: 1200px) {
    .card-list .card-item {
        padding: 15px;
    }
}
@media screen and (max-width: 680px) {
    .card-list {
        margin: 0 auto;
    }
    body{
      height: 840vh;
    }
    footer{
      margin-top: 20%;
    }
    iframe{
      margin-left: -85%;
    margin-top: 220%; 
    width: 500px;
    }
    .logo{
      display: none;
    }
    nav ul {
    
    margin-right: 9%;
}
.intro{
 font-size: 13px;
 margin-top: 90%;
 margin-left: 18%;
 width: 300px;
}
.hi{
  font-size: 18px;

}
.btn-cont {
 margin-top: 120%;
 margin-left: 35%;
}
#bout{
  margin-top: 160%;
}

.pic{
      width: 160px;
    height: 300px;
   }
  
   .imgcont{ 
    width: 160px;
    height: 300px;
    margin-left: 35%;
    margin-top: 15%;
   }
   .imgcont1{
    width: 160px;
    height: 300px;
    margin-left: 37%;
    margin-top: 13%;
   }
   .imgcont2{
    width: 160px;
    height: 301px;
    margin-left: 39%;
    margin-top: 11%;
   }
   #rec{
    font-size: 24px;
    margin-bottom: 5%;
   }
   #conts1{
    margin-bottom: 5%;
   }
   
.btn1 .btn {
  margin-top: 5%;
  height: 500px;
  width: 200px; 
  margin-left: -13.5%
}
  
}


.hr2{
  width: 70%;
  margin-top: 5%;
}
.hr3{
  width: 70%;
  margin-top: 5%;
}
.map{
    margin-left: 47%;
    margin-top: 5%;
}
.btn1 {
  position: absolute;
  margin-left: 11%;
    margin-top: 5%;
}
.btn1 .btn {
  height: 500px;
  position: absolute;
  width: 500px;
  border: 1px solid white;
  color: white;
  text-decoration: none;
  font-family: 'Technolab', sans-serif;
  text-transform: uppercase;
  letter-spacing: 2px;
  -webkit-font-smoothing: antialiased;
}
.btn1 .btn:hover {
  border: none;
}
.btn1 .btn:hover .line-1 {
  -webkit-animation: move1 1500ms infinite ease;
          animation: move1 1500ms infinite ease;
}
.btn1 .btn:hover .line-2 {
  -webkit-animation: move2 1500ms infinite ease;
          animation: move2 1500ms infinite ease;
}
.btn1 .btn:hover .line-3 {
  -webkit-animation: move3 1500ms infinite ease;
          animation: move3 1500ms infinite ease;
}
.btn1 .btn:hover .line-4 {
  -webkit-animation: move4 1500ms infinite ease;
          animation: move4 1500ms infinite ease;
}
.btn1 .line-1 {
  content: "";
  display: block;
  position: absolute;
  width: 1px;
  background-color: rgb(35, 255, 6);
  left: 0;
  bottom: 0;
}
.btn1 .line-2 {
  content: "";
  display: block;
  position: absolute;
  height: 1px;
  background-color: rgb(35, 255, 6);
  left: 0;
  top: 0;
}
.btn1 .line-3 {
  content: "";
  display: block;
  position: absolute;
  width: 1px;
  background-color: rgb(35, 255, 6);
  right: 0;
  top: 0;
}
.btn1 .line-4 {
  content: "";
  display: block;
  position: absolute;
  height: 1px;
  background-color: rgb(35, 255, 6);
  right: 0;
  bottom: 0;
}

h1{
    color: white;
    font-family: 'Technolab', sans-serif;
    text-transform: uppercase;
    font-size: 17px;
    margin-left: 8%;
    margin-top: 4%;
}
p{
    color: white;
    font-family: 'Technolab', sans-serif;
    font-size: 10px;
    margin-left: 20%;
}
.her{
    margin-left: 20%;
    width: 90%;
}
</style>