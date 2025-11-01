<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Jocelyn Semillano - Enchanted Portfolio</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700;800&display=swap" rel="stylesheet">
<script src="https://cdn.tailwindcss.com"></script>

<style>
/* ✨ Body & Background */
body {
  font-family: 'Poppins', sans-serif;
  margin: 0;
  color: white;
  overflow-x: hidden;
  min-height: 100vh;
  background: radial-gradient(circle at top, #2b003a, #0a0015 80%);
}

/* ✨ Animated mist */
@keyframes swirl {0%{background-position:0 0;}100%{background-position:1000px 1000px;}}
.mist {
  position: fixed;top:0;left:0;width:100%;height:100%;
  background: radial-gradient(circle, rgba(255,182,193,0.2), transparent 70%), radial-gradient(circle, rgba(255,105,180,0.15), transparent 60%);
  background-size: 2000px 2000px;
  animation: swirl 60s linear infinite;
  z-index:-3;pointer-events:none;
}

/* ✨ Stars + sparkles */
.stars {position:fixed;width:100%;height:100%;background:transparent url('https://www.transparenttextures.com/patterns/stardust.png') repeat;opacity:.7;z-index:-2;}
.sparkles {position:fixed;top:0;left:0;width:100%;height:100%;background:transparent url() repeat;background-size:cover;mix-blend-mode:screen;opacity:.3;animation:drift 20s linear infinite;z-index:-1;}
@keyframes drift{0%{transform:translate(0,0);}50%{transform:translate(-20px,20px);}100%{transform:translate(20px,-20px);}}

/* ✨ Magical frame */
.magic-frame::before {
  content:"";position:fixed;top:0;left:0;width:100%;height:100%;
  border-radius:25px;box-shadow:0 0 40px 10px #ff66cc;
  animation:pulse 6s ease-in-out infinite alternate;
  pointer-events:none;z-index:-1;
}
@keyframes pulse{0%{opacity:.7;box-shadow:0 0 20px 5px #ff66cc;}100%{opacity:1;box-shadow:0 0 60px 20px #ff99ff;}}

/* ✨ Text glow */
.glow-text{text-shadow:0 0 10px #ff99ff,0 0 20px #ff66cc;}
.glow-border{box-shadow:0 0 15px 4px #ff66ff;transition:.3s;}
.glow-border:hover{box-shadow:0 0 30px 10px #ff99ff;transform:scale(1.03);}

/* ✨ Floating animation */
@keyframes float{0%,100%{transform:translateY(0);}50%{transform:translateY(-10px);}}
.float{animation:float 6s ease-in-out infinite;}

/* ✨ Pulse text */
@keyframes pulse-slow{0%,100%{text-shadow:0 0 5px #ff99ff;}50%{text-shadow:0 0 20px #ffccff;}}
.animate-pulse-slow{animation:pulse-slow 3s ease-in-out infinite;}

/* ✨ Scrollbar */
::-webkit-scrollbar{width:6px;}::-webkit-scrollbar-thumb{background:#ff66ff;border-radius:4px;}
section{scroll-margin-top:80px;}
</style>
</head>

<body class="relative min-h-screen">

<div class="mist"></div>
<div class="stars"></div>
<div class="sparkles"></div>
<div class="magic-frame"></div>

<!-- 🌙 NAV -->
<nav class="py-3 px-2 text-center text-white font-bold text-base sm:text-lg flex flex-wrap justify-center gap-4 sticky top-0 z-50 bg-pink-700/40 backdrop-blur-md">
  <a href="#home">Home</a>
  <a href="#about">About</a>
  <a href="#skills">Skills</a>
  <a href="#experience">Experience</a>
  <a href="#tutorials">Tutorials</a>
  <a href="#tools">Tools</a>
  <a href="#contact">Contact</a>
</nav>

<!-- 🏰 HOME -->
<section id="home" class="flex flex-col items-center text-center px-4 py-16 sm:py-20">
  <h1 class="text-3xl sm:text-5xl font-bold mb-6 glow-text">Welcome to My Enchanted Portfolio!</h1>
  <div class="relative mb-6">
    <img src="Just me.jpg" alt="Celyn" class="w-40 h-40 sm:w-48 sm:h-48 rounded-full border-4 border-pink-500 object-cover glow-border float">
  </div>
</section>

<!-- 📝 ABOUT -->
<section id="about" class="text-center px-4 py-12 sm:py-16">
  <h2 class="text-3xl sm:text-4xl font-bold mb-6 text-pink-400 glow-text">✨ About Me ✨</h2>
  <div class="max-w-md sm:max-w-2xl mx-auto text-base sm:text-lg text-gray-200 space-y-4">
    <p>Hi, it’s me <span class="font-bold text-white">Celyn</span>, a passionate <span class="text-pink-400 font-semibold">2nd Year BSIT Student</span>. I love blending creativity and technology to create projects that feel alive and magical.</p>
    <p> My goal is to use technology to solve real-world problems and create meaningful digital experiences. I’m constantly learning new tools and improving my skills in programming, web development, and creative design software.</p>
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

    <!-- 🎬 PNP Anniversary Contest -->
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
        <img src="film maker pro.png" class="w-16 h-16 rounded-lg glow-border" alt="Film Maker Pro">
        <img src="Kinemaster.png" class="w-16 h-16 rounded-lg glow-border" alt="Kinemaster">
      </div>
    </div>

    <!-- 🎨 Tarpapel Editor -->
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
        <img src="canva.jpeg" class="w-16 h-16 rounded-lg glow-border" alt="Canva">
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
