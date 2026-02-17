<html lang="fa">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>{Dragon Role play}</title>

<style>
#server-ip {
  cursor: pointer;
  position: relative;
  transition: .3s;
}

#server-ip:hover {
  box-shadow: 0 0 15px #ff7b00,
    0 0 30px #ff7b00;
  transform: scale(1.05);
}

#copy-msg {
  position: absolute;
  bottom: -30px;
  left: 50%;
  transform: translateX(-50%);
  background: #00ffea;
  color: #000;
  padding: 5px 15px;
  border-radius: 10px;
  font-weight: bold;
  opacity: 0;
  pointer-events: none;
  transition: .3s;
}
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family:tahoma;
  scroll-behavior:smooth;
}

body {
  color: #fff;
  background:
    radial-gradient(circle at top, rgba(255, 140, 0, 0.25), transparent 40%),
    radial-gradient(circle at bottom, rgba(255, 90, 0, 0.2), transparent 40%),
    linear-gradient(135deg, #0b0602, #140900, #0b0602);
  background-attachment: fixed;
  overflow-x: hidden;
}

/* ===== Preloader ===== */
#preloader{
  position:fixed;
  width:100%;
  height:100%;
  background:#fff;
  display:flex;
  justify-content:center;
  align-items:center;
  z-index:9999;
}

.loader{
  width:60px;
  height:60px;
  border:6px solid #1E90FF;
  border-top:6px solid transparent;
  border-radius:50%;
  animation:spin 1s linear infinite;
}

@keyframes spin{
  100%{transform:rotate(360deg);}
}

/* ===== Navbar ===== */
.navbar{
  position:fixed;
  top:0;
  width:100%;
  display:flex;
  justify-content:space-between;
  align-items:center;
  padding:10px 20px;
  background: rgba(255,255,255,0.95);
  z-index:1000;
  border-radius: 0 0 15px 15px;
}

.menu-toggle{
  display:none;
  flex-direction:column;
  gap:5px;
  cursor:pointer;
}

.menu-toggle div{
  width:30px;
  height:4px;
  background:#1E90FF;
  border-radius:2px;
}

.navbar ul{
  display:flex;
  gap:20px;
  list-style:none;
}

.navbar a{
  color:#d77400;
  text-decoration:none;
  font-weight:bold;
  padding:8px 15px;
  border-radius:8px;
  transition:.3s;
}

.navbar a:hover{
  background:#1E90FF;
  color:white;
}

@media(max-width:900px){
  .menu-toggle{display:flex;}
  .navbar ul{
    display:none;
    flex-direction:column;
    background: rgba(255,255,255,0.95);
    position:absolute;
    top:60px;
    right:20px;
    padding:10px 20px;
    border-radius:8px;
  }
  .navbar ul.show{display:flex;}
}

/* ===== Hero ===== */
.hero{
  height:100vh;
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:center;
  text-align:center;
}

.logo{
  color:#0effff;
  font-size:50px;
  font-weight:bold;
  text-shadow: 0 0 10px #1E90FF;
}

.btn{
  margin-top:20px;
  padding:15px 35px;
  background:#1E90FF;
  color:white;
  border-radius:15px;
  font-weight:bold;
  font-size:18px;
  box-shadow:0 0 20px #1E90FF;
}

/* ===== Sections ===== */
.section{
  padding:80px 20px;
  text-align:center;
}

/* ===== Cards ===== */
.cards{
  display:flex;
  flex-wrap:wrap;
  justify-content:center;
  gap:20px;
  margin-top:40px;
}

.card{
  padding:25px;
  border-radius:10px;
  width:250px;
  font-weight:bold;
  box-shadow: 0 0 15px rgba(0,0,0,0.1);
}

.card.owner{background:#af2d00;}
.card.scripter{background:#af2d00;}

/* ===== Gallery ===== */
.gallery-scroll{
  display:flex;
  overflow-x:auto;
  gap:20px;
  padding:20px 0;
}

.gallery-card{
  width:300px;
  border-radius:12px;
  overflow:hidden;
  box-shadow:0 0 15px rgba(0,0,0,.3);
}

.gallery-card img{width:100%;}

/* ===== Server IP ===== */
#server-ip{
  padding:25px 40px;
  background:rgba(255,140,0,.15);
  border-radius:18px;
  display:inline-block;
  box-shadow:0 0 20px rgba(255,140,0,.7);
}

footer{
  background:#FFD580;
  padding:20px;
  text-align:center;
  font-weight:bold;
  color:#1E90FF;
}
/* ===== Hover Glow Effect ===== */

/* دکمه اصلی */
.btn:hover {
  box-shadow:
    0 0 10px #00f,
    0 0 20px #00f,
    0 0 40px #00ffff;
  transform: scale(1.05);
}

/* دکمه‌های منو */
.navbar a:hover {
  box-shadow:
    0 0 8px #00f,
    0 0 18px #00f,
    0 0 35px #00ffff;
  background: #1E90FF;
  color: #fff;
}

/* کارت‌ها */
.card:hover {
  box-shadow:
    0 0 15px #00ffff,
    0 0 30px #00f;
  transform: translateY(-5px) scale(1.03);
}

/* دکمه همبرگری */
.menu-toggle:hover div {
  box-shadow:
    0 0 10px #00ffff,
    0 0 20px #00f;
    
    .slider {
  width: 90%;
  max-width: 900px;
  margin: 40px auto;
  border-radius: 20px;
  overflow: hidden;
  box-shadow: 0 0 20px #ff7b00;
}

.slider img {
  width: 100%;
  display: block;
  transition: 0.5s;
}
.slider-box {
  width: 90%;
  max-width: 900px;
  margin: 30px auto;
  border-radius: 20px;
  overflow: hidden;
  box-shadow: 0 0 25px rgba(255, 140, 0, .9);
}

.slider-box img {
  width: 100%;
  display: block;
  transition: opacity .6s ease;
} 

</style>
</head>

<body>

<div id="preloader">
  <div class="loader"></div>
</div>

<nav class="navbar">
  <div class="menu-toggle" id="menu-toggle">
    <div></div><div></div><div></div>
  </div>
  <ul id="nav-links">
    <li><a href="#home">خانه</a></li>
    <li><a href="#features">ویژگی‌ها</a></li>
    <li><a href="#team">مدیریت</a></li>
    <li><a href="#gallery">گالری</a></li>
    <li><a href="#server-ip">IP سرور</a></li>
    <li><a href="https://ttaahhaa1123456789-sketch.github.io/Dragon-Rp-Shop/" target="_blank">شاپ</a></li>
    <li><a href="https://ttaahhaa1123456789-sketch.github.io/Froum-DragonRp/" target="_blank">انجمن</a></li>
  </ul>
</nav>

<section id="home" class="hero">
  <h1 class="logo">DRAGON ROLEPLAY</h1>
  <h2><span id="typing"></span></h2>
  <a href="mp://127.0.0.1:7777" class="btn">🎮 Connect To Server</a>
</section>

<section id="features" class="section">
  <h2>ویژگی‌های سرور</h2>
  <div class="cards">
    <div class="card" style="background:#1E90FF;">🚓 سیستم پلیس حرفه‌ای</div>
    <div class="card" style="background:#32CD32;">🏢 گتو و مافیا</div>
    <div class="card" style="background:#FFD700;">💰 اقتصاد واقعی</div>
    <div class="card" style="background:#FF69B4;">🏎 ماشین‌های سفارشی</div>
  </div>
</section>

<section id="team" class="section">
  <h2>تیم مدیریت</h2>
  <div class="cards">
    <div class="card owner">👑 Owner: Mr_Taha</div>
    <div class="card scripter">🛡 Scripter: Kurdx</div>
  </div>
</section>

<section id="gallery" class="section">
  <h2>گالری سرور</h2>
  <div class="gallery-scroll">
    <img id="slider-img" src="https://uploadkon.ir/uploads/418017_26IMG-20250907-151918-804.png" alt="Gallery Image" class="clickable-img">
  </div>
</section>

<style>
  .gallery-scroll {
    width: 100%;
    max-width: 400px;
    margin: 0 auto;
    overflow: hidden;
    border-radius: 12px;
    cursor: pointer;
  }
  
  #slider-img {
    width: 100%;
    border-radius: 12px;
    transition: opacity 0.5s ease-in-out;
  }
  
  #lightbox {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.8);
    display: none;
    justify-content: center;
    align-items: center;
    z-index: 9999;
  }
  
  #lightbox img {
    max-width: 90%;
    max-height: 90%;
    border-radius: 12px;
  }
</style>

<div id="lightbox">
  <img src="" alt="Expanded Image">
</div>

<script>
  const sliderImages = [
    "https://uploadkon.ir/uploads/418017_26IMG-20250907-151918-804.png",
    "https://via.placeholder.com/400x250.png?text=Server+Image+2",
    "https://via.placeholder.com/400x250.png?text=Server+Image+3",
    "https://via.placeholder.com/400x250.png?text=Server+Image+4"
  ];
  
  let sliderIndex = 0;
  const sliderImg = document.getElementById("slider-img");
  
  setInterval(() => {
    sliderIndex++;
    if (sliderIndex >= sliderImages.length) sliderIndex = 0;
    
    sliderImg.style.opacity = 0;
    
    setTimeout(() => {
      sliderImg.src = sliderImages[sliderIndex];
      sliderImg.style.opacity = 1;
    }, 500);
    
  }, 5000);
  
  // ===== Lightbox =====
  const lightbox = document.getElementById("lightbox");
  const lightboxImg = lightbox.querySelector("img");
  
  sliderImg.addEventListener("click", () => {
    lightboxImg.src = sliderImg.src;
    lightbox.style.display = "flex";
  });
  
  lightbox.addEventListener("click", () => {
    lightbox.style.display = "none";
  });
</script>
</section>

<center>
<center>
  <section id="server-ip" onclick="copyIP()">
    <h2>IP سرور</h2>
    <span id="ip-text">127.0.0.1:7777</span>
    <div id="copy-msg">کپی شد ✔</div>
</center>

</center>

<footer>
  Tavsot Tim Dragon Rp | @DraGon_RolePlay | @Mashin_Mazndarn
</footer>

<script>
window.addEventListener("load",()=>{document.getElementById("preloader").style.display="none"});

const menuToggle=document.getElementById('menu-toggle');
const navLinks=document.getElementById('nav-links');
menuToggle.onclick=()=>navLinks.classList.toggle('show');

const text="به بهترین سرور،دراگون رول پلی خوش آمدید";
let i=0;
(function typing(){
  if(i<text.length){
    document.getElementById("typing").innerHTML+=text.charAt(i++);
    setTimeout(typing,60);
  }
})();
function copyIP() {
  const ip = document.getElementById("ip-text").innerText;
  navigator.clipboard.writeText(ip);
  
  const msg = document.getElementById("copy-msg");
  msg.style.opacity = "1";
  
  setTimeout(() => {
    msg.style.opacity = "0";
  }, 1500);
} 
</script>
<script>
const sliderImages = [
  "https://picsum.photos/900/450?random=1",
  "https://picsum.photos/900/450?random=2",
  "https://picsum.photos/900/450?random=3",
  "https://picsum.photos/900/450?random=4"
];

let sliderIndex = 0;
const sliderImg = document.getElementById("slider-img");

setInterval(() => {
  sliderIndex++;
  if(sliderIndex >= sliderImages.length) sliderIndex = 0;

  sliderImg.style.opacity = 0;

  setTimeout(() => {
    sliderImg.src = sliderImages[sliderIndex];
    sliderImg.style.opacity = 1;
  }, 300);

}, 5000);

</script>
</body>
</html>
