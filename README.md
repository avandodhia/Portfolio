<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Avan Dodhia - Portfolio</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    /* ---------- GOLD: two roles ---------- */
    .gold-accent-bg {
      background: linear-gradient(135deg, #d4af37 0%, #ffd700 100%);
    }
    .gold-accent-text {
      background: linear-gradient(135deg, #d4af37 0%, #ffd700 100%);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
      display: inline-block;
      vertical-align: middle;
      padding-left: 0.08rem;
      padding-right: 0.08rem;
    }

    /* Soft skill card fixes */
    .skill-card {
      white-space: normal;
      word-break: normal;
      overflow-wrap: break-word;
      min-width: 10rem;
    }
    .skill-card h4 {
      margin: 0;
      font-size: 0.95rem;
      line-height: 1.25;
      white-space: normal;
      word-break: normal;
      overflow-wrap: anywhere;
    }

    /* Reserve space for fixed nav */
    :root { --nav-height: 72px; }
    body { padding-top: var(--nav-height); }
    nav { height: var(--nav-height); }

    /* Hover card */
    .card-hover {
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    .card-hover:hover {
      transform: translateY(-6px);
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
    }
  </style>
</head>
<body class="bg-gray-50 text-gray-900">

  <!-- Navigation -->
  <nav class="fixed top-0 w-full bg-white/95 backdrop-blur-md z-50 shadow-sm border-b border-gray-100">
    <div class="max-w-6xl mx-auto px-6 py-4">
      <div class="flex justify-between items-center">
        <div class="text-2xl font-bold text-gray-800">
          <span class="text-blue-900">Avan</span> <span class="gold-accent-text">Dodhia</span>
        </div>
        <div class="space-x-6 hidden md:flex">
          <a href="#about" class="hover:text-blue-600">About</a>
          <a href="#skills" class="hover:text-blue-600">Skills</a>
          <a href="#projects" class="hover:text-blue-600">Projects</a>
          <a href="#contact" class="hover:text-blue-600">Contact</a>
        </div>
      </div>
    </div>
  </nav>

  <!-- Hero Section -->
  <section class="relative bg-gradient-to-br from-blue-50 via-white to-blue-100 py-28">
    <div class="max-w-6xl mx-auto px-6 text-center">
      <h1 class="text-4xl md:text-6xl font-bold mb-6">
        Hi, I’m <span class="text-blue-900">Avan</span> <span class="gold-accent-text">Dodhia</span>
      </h1>
      <p class="text-lg md:text-xl text-gray-600 max-w-2xl mx-auto">
        <span class="typing-animation gold-accent-text"></span>
      </p>
      <a href="#projects" class="mt-8 inline-block bg-blue-600 text-white px-6 py-3 rounded-xl shadow hover:bg-blue-700 transition">
        View My Work
      </a>
    </div>
  </section>

  <!-- Skills Section -->
  <section id="skills" class="py-20 bg-white">
    <div class="max-w-6xl mx-auto px-6">
      <h2 class="text-3xl font-bold text-center mb-12">Skills</h2>
      <div class="grid md:grid-cols-2 gap-12">
        <!-- Hard Skills -->
        <div>
          <h3 class="text-xl font-semibold mb-6">Hard Skills</h3>
          <div class="grid grid-cols-2 sm:grid-cols-3 gap-6">
            <div class="bg-gray-50 p-6 rounded-xl text-center card-hover">
              <div class="w-16 h-16 mx-auto rounded-full gold-accent-bg flex items-center justify-center text-white text-2xl font-bold mb-3">F</div>
              <h4 class="font-semibold text-gray-800">Finance</h4>
            </div>
            <div class="bg-gray-50 p-6 rounded-xl text-center card-hover">
              <div class="w-16 h-16 mx-auto rounded-full gold-accent-bg flex items-center justify-center text-white text-2xl font-bold mb-3">D</div>
              <h4 class="font-semibold text-gray-800">Data Analysis</h4>
            </div>
            <div class="bg-gray-50 p-6 rounded-xl text-center card-hover">
              <div class="w-16 h-16 mx-auto rounded-full gold-accent-bg flex items-center justify-center text-white text-2xl font-bold mb-3">S</div>
              <h4 class="font-semibold text-gray-800">Strategy</h4>
            </div>
          </div>
        </div>

        <!-- Soft Skills -->
        <div>
          <h3 class="text-xl font-semibold mb-6">Soft Skills</h3>
          <div class="grid grid-cols-2 sm:grid-cols-3 gap-6">
            <div class="bg-gray-50 p-6 rounded-xl text-center card-hover skill-card">
              <div class="text-4xl mb-3">👥</div>
              <h4 class="font-semibold text-gray-800 text-sm">Leadership</h4>
            </div>
            <div class="bg-gray-50 p-6 rounded-xl text-center card-hover skill-card">
              <div class="text-4xl mb-3">💡</div>
              <h4 class="font-semibold text-gray-800 text-sm">Problem Solving</h4>
            </div>
            <div class="bg-gray-50 p-6 rounded-xl text-center card-hover skill-card">
              <div class="text-4xl mb-3">🤝</div>
              <h4 class="font-semibold text-gray-800 text-sm">Collaboration</h4>
            </div>
            <div class="bg-gray-50 p-6 rounded-xl text-center card-hover skill-card">
              <div class="text-4xl mb-3">🕒</div>
              <h4 class="font-semibold text-gray-800 text-sm">Time Management</h4>
            </div>
            <div class="bg-gray-50 p-6 rounded-xl text-center card-hover skill-card">
              <div class="text-4xl mb-3">📢</div>
              <h4 class="font-semibold text-gray-800 text-sm">Communication</h4>
            </div>
            <div class="bg-gray-50 p-6 rounded-xl text-center card-hover skill-card">
              <div class="text-4xl mb-3">🎯</div>
              <h4 class="font-semibold text-gray-800 text-sm">Critical Thinking</h4>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="py-8 bg-gray-100 border-t text-center">
    <p class="text-gray-600">
      © 2025 <span class="text-blue-900">Avan</span> <span class="gold-accent-text">Dodhia</span>. All rights reserved.
    </p>
  </footer>

  <!-- Typing animation script -->
  <script>
    const roles = ["Finance Enthusiast", "Data Analyst", "Problem Solver", "Future IB Professional"];
    let roleIndex = 0;
    let charIndex = 0;
    const typingElement = document.querySelector(".typing-animation");

    function typeRole() {
      if (charIndex < roles[roleIndex].length) {
        typingElement.textContent += roles[roleIndex].charAt(charIndex);
        charIndex++;
        setTimeout(typeRole, 100);
      } else {
        setTimeout(eraseRole, 2000);
      }
    }

    function eraseRole() {
      if (charIndex > 0) {
        typingElement.textContent = roles[roleIndex].substring(0, charIndex - 1);
        charIndex--;
        setTimeout(eraseRole, 50);
      } else {
        roleIndex = (roleIndex + 1) % roles.length;
        setTimeout(typeRole, 500);
      }
    }

    document.addEventListener("DOMContentLoaded", () => {
      if (roles.length) typeRole();
    });
  </script>
</body>
</html>
