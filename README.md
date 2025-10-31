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
  position: relative;
  min-height: 100vh;
  background: radial-gradient(circle at top, #2b003a, #0a0015 80%);
}

/* ✨ Animated swirling pink mist */
@keyframes swirl {
  0% { background-position: 0 0; }
  100% { background-position: 1000px 1000px; }
}
.mist {
  position: fixed;
  top:0; left:0;
  width:100%; height:100%;
  background: radial-gradient(circle, rgba(255,182,193,0.2), transparent 70%), radial-gradient(circle, rgba(255,105,180,0.15), transparent 60%);
  background-size: 2000px 2000px;
  z-index: -3;
  animation: swirl 60s linear infinite;
  pointer-events: none;
}

/* ✨ Stars */
.stars {
  position: fixed;
  width:100%; height:100%;
  background: transparent url('https://www.transparenttextures.com/patterns/stardust.png') repeat;
  opacity: 0.7;
  z-index:-2;
  animation: twinkle 8s infinite alternate;
}
@keyframes twinkle { 0% {opacity:0.5;} 100% {opacity:1;} }

/* ✨ Floating sparkles */
.sparkles {
  position: fixed;
  top:0; left:0;
  width:100%; height:100%;
  background: transparent url('https://i.ibb.co/8gPswLp/fairy-dust.gif') repeat;
  background-size: cover;
  mix-blend-mode: screen;
  opacity:0.3;
  animation: drift 20s linear infinite;
  z-index:-1;
}
@keyframes drift {
  0% { transform: translate(0,0) scale(1); }
  50% { transform: translate(-20px,20px) scale(1.05);}
  100% { transform: translate(20px,-20px) scale(1);}
}

/* ✨ Magical pink glowing frame */
.magic-frame::before {
  content:"";
  position: fixed;
  top:0; left:0;
  width:100%; height:100%;
  border:5px solid transparent;
  border-radius:25px;
  box-shadow: 0 0 40px 10px #ff66cc;
  animation: pulse 6s ease-in-out infinite alternate;
  pointer-events:none;
  z-index:-1;
}
@keyframes pulse {
  0% { opacity:0.7; box-shadow:0 0 20px 5px #ff66cc, inset 0 0 30px #ff99cc; }
  100% { opacity:1; box-shadow:0 0 60px 20px #ff99ff, inset 0 0 50px #ff66ff; }
}

/* ✨ Glowing text & borders */
.glow-text { text-shadow:0 0 10px #ff99ff,0 0 20px #ff66cc;}
.glow-border { box-shadow:0 0 20px 5px #ff66ff; transition:0.3s; }
.glow-border:hover { box-shadow:0 0 30px 10px #ff99ff; transform:scale(1.02); }

/* ✨ Floating animation */
@keyframes float {
  0% { transform: translateY(0px); }
  50% { transform: translateY(-10px); }
  100% { transform: translateY(0px); }
}
.float { animation: float 6s ease-in-out infinite; }
.float-hover:hover { transform: translateY(-15px) scale(1.03); transition:0.5s ease; }

/* ✨ Slow pulse animation for skill and skull names */
@keyframes pulse-slow {
  0% { text-shadow: 0 0 5px #ff99ff, 0 0 10px #ff66cc; opacity: 0.7; }
  50% { text-shadow: 0 0 20px #ffccff, 0 0 30px #ff99ff; opacity: 1; }
  100% { text-shadow: 0 0 5px #ff99ff, 0 0 10px #ff66cc; opacity: 0.7; }
}
.animate-pulse-slow { animation: pulse-slow 3s ease-in-out infinite; }

/* ✨ Navigation */
nav {
  background: rgba(255,0,170,0.6);
  backdrop-filter: blur(12px);
  box-shadow:0 0 25px #ff66ff;
}
nav a { transition:0.3s ease; }
nav a:hover { color:#ffd6f7; text-shadow:0 0 8px #ffccff; }

::-webkit-scrollbar { width:8px; }
::-webkit-scrollbar-thumb { background:#ff66ff; border-radius:4px; }
::-webkit-scrollbar-thumb:hover { background:#ff99ff; }

section { scroll-margin-top:100px; }
</style>
</head>

<body class="min-h-screen relative">
  <!-- ✨ Layers -->
  <div class="mist"></div>
  <div class="stars"></div>
  <div class="sparkles"></div>
  <div class="magic-frame"></div>

  <!-- 🌙 NAV -->
  <nav class="py-4 text-center text-white font-bold text-lg flex justify-center space-x-8 sticky top-0 z-50">
    <a href="#home">Home</a>
    <a href="#about me">About Me</a>
    <a href="#skills">Skills</a>
    <a href="#videos">Videos</a>
    <a href="#tutorials">Tutorials</a>
    <a href="#tools">Tools</a>
    <a href="#contact">Contact</a>
  </nav>

  <!-- 🏰 HOME -->
  <section id="home" class="flex flex-col items-center text-center px-4 py-20">
    <h1 class="text-4xl sm:text-5xl font-bold mb-6 glow-text">Welcome to My Enchanted Portfolio!</h1>
    <div class="relative mb-8">
      <img src="Just me.jpg" alt="Celyn"
        class="w-48 h-48 rounded-full border-4 border-pink-500 shadow-lg object-cover glow-border float">
      <div class="absolute inset-0 rounded-full shadow-[0_0_50px_20px_rgba(255,105,180,0.4)] animate-pulse pointer-events-none"></div>
    </div>
  </section>

  <!-- 📝 ABOUT ME -->
  <section id="about" class="text-center px-4 py-16">
    <h2 class="text-4xl font-bold mb-8 text-pink-400 glow-text">✨ About Me ✨</h2>
    <div class="max-w-3xl mx-auto text-lg sm:text-xl text-gray-200 space-y-4">
      <p>
        Hi, it’s me <span class="font-bold text-white">Celyn</span>, a passionate <span class="text-pink-400 font-semibold">2nd Year BSIT Student</span>. 
        I love turning imagination into reality through creativity, technology, and design. My goal is to blend technical skills with artistic vision to create projects that feel alive and magical.
      </p>
      <p>
        Outside of coding and design, I enjoy exploring new tools, learning new techniques, and sharing my knowledge through tutorials. Every project I make has a sprinkle of enchantment ✨ to inspire and delight anyone who sees it.
      </p>
    </div>
  </section>


  <!-- 🛠️ MY SKILLS -->
  <section id="skills" class="text-center px-4 py-16">
    <h2 class="text-4xl font-bold mb-8 text-pink-400 glow-text">🛠️ My Skills</h2>
    <div class="flex flex-col items-center gap-8">
      <div class="flex flex-col items-center">
        <img src="banner.jpg" class="w-80 h-30 rounded-lg glow-border float" alt="Banner">
        <span class="mt-2 text-white font-semibold glow-text animate-pulse-slow">Creating Banner</span>
      </div>
      <div class="flex flex-col items-center">
        <img src="Chessboard.png" class="w-48 h-48 rounded-lg glow-border float" alt="Chessboard">
        <span class="mt-2 text-white font-semibold glow-text animate-pulse-slow"> Creating Chessboard</span>
      </div>
      <div class="flex flex-col items-center">
        <img src="figma ecommerce.jpg" class="w-30 h-80 rounded-lg glow-border float" alt="Figma Ecommerce">
        <span class="mt-2 text-white font-semibold glow-text animate-pulse-slow">Creating Figma Ecommerce</span>
      </div>
      <div class="flex flex-col items-center">
        <img src="Product Design.png" class="w-40 h-48 rounded-lg glow-border float" alt="Product Designing">
        <span class="mt-2 text-white font-semibold glow-text animate-pulse-slow">Product Designing</span>
      </div>
      <div class="flex flex-col items-center">
        <img src="tshirt layout.png" class="w-48 h-40 rounded-lg glow-border float" alt="T-shirt Layouting">
        <span class="mt-2 text-white font-semibold glow-text animate-pulse-slow">T-shirt Layouting</span>
      </div>
    </div>
  </section>


  <!-- 🌸 YOUTUBE TUTORIALS -->
  <section id="tutorials" class="text-center px-4 py-20">
    <h2 class="text-5xl font-extrabold mb-10 text-pink-300 glow-text animate-bounce">✨ YouTube Tutorials ✨</h2>
    <div class="grid grid-cols-1 md:grid-cols-2 gap-10 max-w-6xl mx-auto">
      <iframe class="rounded-2xl w-full h-64 glow-border float" src="https://www.youtube.com/embed/wCEtWz5imUs" allowfullscreen></iframe>
      <iframe class="rounded-2xl w-full h-64 glow-border float" src="https://www.youtube.com/embed/ezldKx-jPag" allowfullscreen></iframe>
      <iframe class="rounded-2xl w-full h-64 glow-border float" src="https://www.youtube.com/embed/61mkx_OV61s" allowfullscreen></iframe>
      <iframe class="rounded-2xl w-full h-64 glow-border float" src="https://www.youtube.com/embed/keoszhf4DZ8" allowfullscreen></iframe>
    </div>
  </section>

  <!-- 🧚‍♀️ TOOLS -->
  <section id="tools" class="text-center px-4 py-16">
    <h2 class="text-4xl font-bold mb-8 text-pink-400 glow-text">🪄 Tools I Used</h2>
    <div class="flex justify-center items-center flex-wrap gap-8">
      <img src="canva.jpeg" class="w-24 h-24 rounded-lg glow-border float" alt="Canva">
      <img src="figma.jpeg" class="w-24 h-24 rounded-lg glow-border float" alt="Figma">
      <img src="Adobe photoshop.jpeg" class="w-24 h-24 rounded-lg glow-border float" alt="Photoshop">
      <img src="Adobe premiere.jpeg" class="w-24 h-24 rounded-lg glow-border float" alt="Premiere">
    </div>
  </section>

  <!-- 💌 CONTACT -->
  <section id="contact" class="text-center px-4 py-16">
    <h2 class="text-4xl font-bold mb-8 text-pink-400 glow-text">💌 Let's Connect</h2>
    <div class="max-w-xl mx-auto p-8 bg-[#1a0033]/70 rounded-2xl shadow-xl border border-pink-600 glow-border">
      <form action="#" method="POST" class="space-y-6">
        <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
          <input type="text" placeholder="First Name" required
            class="w-full px-4 py-2 border-2 border-pink-400 rounded-lg bg-transparent text-white placeholder-gray-300 float-hover">
          <input type="text" placeholder="Last Name" required
            class="w-full px-4 py-2 border-2 border-pink-400 rounded-lg bg-transparent text-white placeholder-gray-300 float-hover">
        </div>
        <input type="email" placeholder="you@example.com" required
          class="w-full px-4 py-2 border-2 border-pink-400 rounded-lg bg-transparent text-white placeholder-gray-300 float-hover">
        <textarea rows="5" placeholder="Your message..." required
          class="w-full px-4 py-2 border-2 border-pink-400 rounded-lg bg-transparent text-white placeholder-gray-300 float-hover"></textarea>
        <button type="submit"
          class="w-full py-3 px-4 bg-pink-600 text-white font-bold rounded-lg hover:bg-pink-700 transition glow-border float-hover">Send Message</button>
      </form>
    </div>
  </section>
</body>
</html>
