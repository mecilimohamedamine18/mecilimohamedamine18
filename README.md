<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Developer Portfolio</title>

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">

  <style>
    * { margin:0; padding:0; box-sizing:border-box; font-family:"Poppins",sans-serif; }
    body {
      background: linear-gradient(to bottom right, #1f1c2c, #928dab);
      color:#fff;
      line-height:1.6;
      scroll-behavior: smooth;
    }

    header {
      display:flex; justify-content:space-between; align-items:center;
      padding:20px 60px; background:rgba(0,0,0,0.4);
      position:sticky; top:0; z-index:1000; backdrop-filter:blur(5px);
    }
    header h1 { font-size:24px; font-weight:700; color:#00d9ff; }
    nav a {
      color:#fff; text-decoration:none; margin-left:20px; font-weight:500;
      transition:color .3s ease;
    }
    nav a:hover { color:#00d9ff; }

    .hero {
      height:90vh; display:flex; flex-direction:column;
      justify-content:center; align-items:center; text-align:center;
      padding:0 20px;
    }
    .hero h2 {
      font-size:48px; margin-bottom:20px; color:#00d9ff;
    }
    .hero p { font-size:20px; max-width:600px; }

    section { padding:60px 20px; max-width:1100px; margin:0 auto; }
    h3.section-title {
      text-align:center; font-size:36px; margin-bottom:40px; color:#00d9ff;
    }

    .badges {
      display:flex; flex-wrap:wrap; justify-content:center; gap:15px;
      margin-bottom:40px;
    }
    .badges img { height:32px; }

    .cards {
      display:grid; grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
      gap:30px;
    }
    .card {
      background:rgba(255,255,255,0.08); padding:25px; border-radius:15px;
      text-align:center; transition:transform .3s ease, background .3s ease;
    }
    .card:hover { transform:translateY(-5px); background:rgba(255,255,255,0.12); }
    .card h4 { margin-bottom:15px; color:#00d9ff; }

    footer {
      text-align:center; padding:20px; background:rgba(0,0,0,0.4);
      margin-top:40px;
    }
    footer a { color:#00d9ff; text-decoration:none; margin:0 10px; font-weight:500; }
    footer a:hover { text-decoration:underline; }
  </style>
</head>
<body>

  <header>
    <h1>👨‍💻 My Portfolio</h1>
    <nav>
      <a href="#hero">Home</a>
      <a href="#skills">Skills</a>
      <a href="#projects">Projects</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <!-- Hero Section with Animated Hi Coders -->
  <section class="hero" id="hero">
    <h2 id="hi-coders"></h2>
    <p>
      I’m a Full-Stack Developer skilled in C, Java, Laravel, Flutter, and React.  
      I love building modern web & mobile apps that solve real-world problems.
    </p>
  </section>

  <!-- Skills with Language Badges -->
  <section id="skills">
    <h3 class="section-title">💻 Skills & Languages</h3>

    <div class="badges">
      <img src="https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white" alt="C">
      <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java">
      <img src="https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel">
      <img src="https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white" alt="Flutter">
      <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React">
      <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">
      <img src="https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL">
    </div>

    <div class="cards">
      <div class="card">
        <h4>Web Development</h4>
        <p>Laravel, React, HTML, CSS</p>
      </div>
      <div class="card">
        <h4>Mobile Apps</h4>
        <p>Flutter, REST APIs</p>
      </div>
      <div class="card">
        <h4>Backend & APIs</h4>
        <p>Laravel, Node, REST</p>
      </div>
      <div class="card">
        <h4>Databases</h4>
        <p>MySQL, SQLite</p>
      </div>
    </div>
  </section>

  <!-- Projects -->
  <section id="projects">
    <h3 class="section-title">🚀 Projects</h3>
    <div class="cards">
      <div class="card">
        <h4>Medical Clinic App</h4>
        <p>Full clinic management system for doctors, assistants, and patients. (Flutter + Laravel + React)</p>
      </div>
      <div class="card">
        <h4>E-Commerce App</h4>
        <p>Shopping app with cart & checkout using Fake Store API. (Flutter)</p>
      </div>
      <div class="card">
        <h4>Admin Dashboard</h4>
        <p>Responsive dashboard for managing medical data. (React + Laravel)</p>
      </div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact">
    <h3 class="section-title">📫 Contact</h3>
    <p style="text-align:center;">
      <a href="https://github.com/USERNAME" target="_blank">GitHub</a> |
      <a href="https://linkedin.com/in/USERNAME" target="_blank">LinkedIn</a> |
      <a href="mailto:you@example.com">Email</a>
    </p>
  </section>

  <footer>
    &copy; 2025 Your Name — Built with ❤️ and deployed on GitHub Pages
  </footer>

  <!-- Animated Hi Coders Script -->
  <script>
    const text = "👋 Hi Coders!";
    let i = 0;
    const speed = 120; // typing speed in ms

    function typeWriter() {
      if (i < text.length) {
        document.getElementById("hi-coders").innerHTML += text.charAt(i);
        i++;
        setTimeout(typeWriter, speed);
      }
    }

    window.onload = typeWriter;
  </script>
</body>
</html>
