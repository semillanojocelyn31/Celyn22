<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Jocelyn Semillano - Enchanted Portfolio</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700;800&display=swap" rel="stylesheet">
<script src="https://cdn.tailwindcss.com"></script>

<style>
/* 🌌 Base body and background */
body {
  font-family: 'Poppins', sans-serif;
  margin: 0;
  color: white;
  overflow-x: hidden;
  min-height: 100vh;
  background: radial-gradient(circle at top, #2b003a, #0a0015 80%);
  position: relative;
}

/* ✨ Floating mist & stars */
@keyframes swirl {0%{background-position:0 0;}100%{background-position:1000px 1000px;}}
.mist {
  position: fixed;top:0;left:0;width:100%;height:100%;
  background: radial-gradient(circle, rgba(255,182,193,0.15), transparent 70%), radial-gradient(circle, rgba(255,105,180,0.1), transparent 60%);
  background-size: 2000px 2000px;
  animation: swirl 80s linear infinite;
  z-index:-3;pointer-events:none;
}
.stars {
  position: fixed;width:100%;height:100%;
  background: url('https://www.transparenttextures.com/patterns/stardust.png') repeat;
  opacity: 0.9;mix-blend-mode:screen;z-index:-2;
}

/* 🌠 Floating sparkles */
.sparkles {
  position: fixed;top:0;left:0;width:100%;height:100%;
  background: radial-gradient(circle, rgba(255,255,255,0.25) 2px, transparent 3px);
  background-size: 100px 100px;
  animation: sparkleFloat 10s linear infinite;
  z-index:-1;pointer-events:none;
}
@keyframes sparkleFloat {
  0% {transform:translateY(0);}
  50% {transform:translateY(-20px);}
  100% {transform:translateY(0);}
}

/* 🪞 Glowing border frame */
.magic-frame::before {
  content:"";
  position: fixed;top:0;left:0;width:100%;height:100%;
  border-radius: 25px;
  box-shadow: 0 0 60px 10px rgba(255,105,180,0.8);
  animation: pulse 4s ease-in-out infinite alternate;
  pointer-events:none;z-index:-1;
}
@keyframes pulse {
  0% {opacity:.7; box-shadow:0 0 30px 5px #ff66cc;}
  100% {opacity:1; box-shadow:0 0 80px 25px #ff99ff;}
}

/* 💫 Glow text and elements */
.glow-text {
  text-shadow: 0 0 10px #ff99ff, 0 0 25px #ff66cc, 0 0 35px #ffb3ff;
}
.glow-border {
  box-shadow: 0 0 25px 6px rgba(255,105,180,0.7), 0 0 45px 10px rgba(255,182,193,0.5);
  transition: 0.3s;
}
.glow-border:hover {
  box-shadow: 0 0 40px 12px #ff99ff, 0 0 60px 18px #ffb3ff;
  transform: scale(1.05);
}

/* ✨ Float animation */
@keyframes float {
  0%,100%{transform:translateY(0);}
  50%{transform:translateY(-10px);}
}
.float {animation: float 6s ease-in-out infinite;}

/* 🌸 Soft glowing hover for buttons */
button:hover {
  background: linear-gradient(90deg, #ff66cc, #ff99ff);
  box-shadow: 0 0 25px 6px #ff99ff;
  transform: scale(1.03);
}

/* 🌈 Scrollbar */
::-webkit-scrollbar{width:6px;}
::-webkit-scrollbar-thumb{background:#ff66ff;border-radius:4px;}
section{scroll-margin-top:80px;}

/* 🌷 Section aura */
section {
  position: relative;
}
section::before {
  content: "";
  position: absolute;
  top:0; left:50%; transform:translateX(-50%);
  width: 80%;
  height: 100%;
  background: radial-gradient(circle at top, rgba(255,105,180,0.1), transparent 70%);
  filter: blur(30px);
  z-index: -1;
}
</style>
</head>

<body class="relative min-h-screen">
<div class="mist"></div>
<div class="stars"></div>
<div class="sparkles"></div>
<div class="magic-frame"></div>

<!-- 🌙 NAV -->
<nav class="py-3 px-2 text-center text-white font-bold text-base sm:text-lg flex flex-wrap justify-center gap-4 sticky top-0 z-50 bg-pink-700/30 backdrop-blur-md shadow-lg shadow-pink-500/40">
  <a href="#home" class="hover:text-pink-300 glow-text">Home</a>
  <a href="#about" class="hover:text-pink-300 glow-text">About</a>
  <a href="#skills" class="hover:text-pink-300 glow-text">Skills</a>
  <a href="#experience" class="hover:text-pink-300 glow-text">Experience</a>
  <a href="#tutorials" class="hover:text-pink-300 glow-text">Tutorials</a>
  <a href="#tools" class="hover:text-pink-300 glow-text">Tools</a>
  <a href="#contact" class="hover:text-pink-300 glow-text">Contact</a>
</nav>

<!-- 🏰 HOME -->
<section id="home" class="flex flex-col items-center text-center px-4 py-16 sm:py-20">
  <h1 class="text-3xl sm:text-5xl font-bold mb-6 glow-text animate-pulse">Welcome to My Enchanted Portfolio!</h1>
  <div class="relative mb-6">
    <div class="absolute -inset-2 bg-pink-500/30 blur-xl rounded-full"></div>
    <img src="Just me.jpg" alt="Celyn" class="relative w-40 h-40 sm:w-48 sm:h-48 rounded-full border-4 border-pink-500 object-cover glow-border float">
  </div>
</section>

<!-- 📝 ABOUT -->
<section id="about" class="text-center px-4 py-12 sm:py-16">
  <h2 class="text-3xl sm:text-4xl font-bold mb-6 text-pink-400 glow-text">✨ About Me ✨</h2>
  <div class="max-w-md sm:max-w-2xl mx-auto text-base sm:text-lg text-gray-200 space-y-4">
    <p>Hi, it’s me <span class="font-bold text-white">Celyn</span>, a passionate <span class="text-pink-400 font-semibold">2nd Year BSIT Student</span>. I love blending creativity and technology to create projects that feel alive and magical.</p>
    <p>My goal is to use technology to solve real-world problems and create meaningful digital experiences. I’m constantly learning new tools and improving my skills in programming, web development, and creative design software.</p>
  </div>
</section>

<!-- 🛠️ SKILLS -->
<section id="skills" class="text-center px-4 py-12 sm:py-16">
  <h2 class="text-3xl sm:text-4xl font-bold mb-8 text-pink-400 glow-text">🛠️ My Skills</h2>
  <div class="flex flex-col items-center gap-6 sm:gap-8">
    <img src="banner.jpg" class="w-65 rounded-lg glow-border float" alt="Banner">
    <img src="Chessboard.png" class="w-40 rounded-lg glow-border float" alt="Chessboard">
    <img src="figma ecommerce.jpg" class="w-40 rounded-lg glow-border float" alt="Figma Ecommerce">
    <img src="Product Design.png" class="w-40 rounded-lg glow-border float" alt="Product Design">
    <img src="tshirt layout.png" class="w-60 rounded-lg glow-border float" alt="T-shirt Layout">
  </div>
</section>

<!-- 🏆 EXPERIENCE -->
<section id="experience" class="text-center px-4 py-12 sm:py-16">
  <h2 class="text-3xl sm:text-4xl font-bold mb-8 text-pink-400 glow-text animate-bounce">🏆 My Experience</h2>
  <div class="max-w-md sm:max-w-3xl mx-auto space-y-8">

    <div class="bg-[#1a0033]/70 border border-pink-500 rounded-2xl p-6 glow-border float">
      <h3 class="text-2xl font-semibold text-pink-300 glow-text mb-2">
        Champion in PNP Anniversary Video Editing Contest
      </h3>
      <p class="text-gray-300 mb-2">🏅 Year: 2021</p>
      <p class="text-gray-200 text-sm leading-relaxed">
        Awarded for outstanding creativity and editing skills using 
        <span class="text-pink-400 font-medium">Film Maker Pro</span> and 
        <span class="text-pink-400 font-medium">Kinemaster</span>.
      </p>
      <div class="mt-4 flex justify-center gap-3">
        <img src="film maker pro.png" class="w-16 h-16 rounded-lg glow-border">
        <img src="Kinemaster.png" class="w-16 h-16 rounded-lg glow-border">
      </div>
    </div>

    <div class="bg-[#1a0033]/70 border border-pink-500 rounded-2xl p-6 glow-border float">
      <h3 class="text-2xl font-semibold text-pink-300 glow-text mb-2">
        Tarpapel Editor in Birthdays
      </h3>
      <p class="text-gray-300 mb-2">🎨 Year: 2020</p>
      <p class="text-gray-200 text-sm leading-relaxed">
        Designed creative and personalized tarpapel layouts using 
        <span class="text-pink-400 font-medium">Canva</span>.
      </p>
      <div class="mt-4 flex justify-center">
        <img src="canva.jpeg" class="w-16 h-16 rounded-lg glow-border">
      </div>
    </div>

  </div>
</section>

<!-- 🌸 TUTORIALS -->
<section id="tutorials" class="text-center px-4 py-12 sm:py-16">
  <h2 class="text-3xl sm:text-5xl font-extrabold mb-10 text-pink-300 glow-text animate-bounce">✨ YouTube Tutorials ✨</h2>
  <div class="grid grid-cols-1 sm:grid-cols-2 gap-6 max-w-5xl mx-auto">
    <iframe class="rounded-2xl w-full h-56 sm:h-64 glow-border" src="https://www.youtube.com/embed/wCEtWz5imUs" allowfullscreen></iframe>
    <iframe class="rounded-2xl w-full h-56 sm:h-64 glow-border" src="https://www.youtube.com/embed/ezldKx-jPag" allowfullscreen></iframe>
    <iframe class="rounded-2xl w-full h-56 sm:h-64 glow-border" src="https://www.youtube.com/embed/61mkx_OV61s" allowfullscreen></iframe>
    <iframe class="rounded-2xl w-full h-56 sm:h-64 glow-border" src="https://www.youtube.com/embed/keoszhf4DZ8" allowfullscreen></iframe>
  </div>
</section>

<!-- 🧚 TOOLS -->
<section id="tools" class="text-center px-4 py-12 sm:py-16">
  <h2 class="text-3xl sm:text-4xl font-bold mb-8 text-pink-400 glow-text">🪄 Tools I Used</h2>
  <div class="flex flex-wrap justify-center items-center gap-6 sm:gap-8">
    <img src="canva.jpeg" class="w-20 h-20 rounded-lg glow-border">
    <img src="figma.jpeg" class="w-20 h-20 rounded-lg glow-border">
    <img src="Adobe photoshop.jpeg" class="w-20 h-20 rounded-lg glow-border">
    <img src="Adobe premiere.jpeg" class="w-20 h-20 rounded-lg glow-border">
  </div>
</section>

<!-- 💌 CONTACT -->
<section id="contact" class="text-center px-4 py-12 sm:py-16">
  <h2 class="text-3xl sm:text-4xl font-bold mb-8 text-pink-400 glow-text">💌 Let's Connect</h2>
  <div class="max-w-sm sm:max-w-lg mx-auto p-6 bg-[#1a0033]/70 rounded-2xl border border-pink-600 glow-border">
    <form action="#" method="POST" class="space-y-4">
      <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
        <input type="text" placeholder="First Name" class="w-full px-4 py-2 border-2 border-pink-400 rounded-lg bg-transparent text-white placeholder-gray-300">
        <input type="text" placeholder="Last Name" class="w-full px-4 py-2 border-2 border-pink-400 rounded-lg bg-transparent text-white placeholder-gray-300">
      </div>
      <input type="email" placeholder="you@example.com" class="w-full px-4 py-2 border-2 border-pink-400 rounded-lg bg-transparent text-white placeholder-gray-300">
      <textarea rows="5" placeholder="Your message..." class="w-full px-4 py-2 border-2 border-pink-400 rounded-lg bg-transparent text-white placeholder-gray-300"></textarea>
      <button type="submit" class="w-full py-3 px-4 bg-pink-600 text-white font-bold rounded-lg hover:bg-pink-700 transition glow-border">Send Message</button>
    </form>
  </div>
</section>

</body>
</html>
