<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>My Developer Portfolio</title>

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: "Poppins", sans-serif;
    }

    body {
      background: linear-gradient(to bottom right, #1f1c2c, #928dab);
      color: #fff;
      line-height: 1.6;
      scroll-behavior: smooth;
    }

    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 20px 60px;
      background: rgba(0,0,0,0.4);
      position: sticky;
      top: 0;
      z-index: 1000;
      backdrop-filter: blur(5px);
    }

    header h1 {
      font-size: 24px;
      font-weight: 700;
      color: #00d9ff;
    }

    nav a {
      color: #fff;
      text-decoration: none;
      margin-left: 20px;
      font-weight: 500;
      transition: color 0.3s ease;
    }

    nav a:hover {
      color: #00d9ff;
    }

    .hero {
      height: 90vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      padding: 0 20px;
    }

    .hero h2 {
      font-size: 48px;
      margin-bottom: 20px;
      color: #00d9ff;
      animation: fadeIn 2s ease-in-out;
    }

    .hero p {
      font-size: 20px;
      max-width: 600px;
    }

    @keyframes fadeIn {
      from {opacity: 0; transform: translateY(-20px);}
      to {opacity: 1; transform: translateY(0);}
    }

    section {
      padding: 60px 20px;
      max-width: 1100px;
      margin: 0 auto;
    }

    h3.section-title {
      text-align: center;
      font-size: 36px;
      margin-bottom: 40px;
      color: #00d9ff;
    }

    .skills, .projects {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 30px;
    }

    .card {
      background: rgba(255,255,255,0.08);
      padding: 25px;
      border-radius: 15px;
      text-align: center;
      transition: transform 0.3s ease, background 0.3s ease;
    }

    .card:hover {
      transform: translateY(-5px);
      background: rgba(255,255,255,0.12);
    }

    .card h4 {
      margin-bottom: 15px;
      color: #00d9ff;
    }

    footer {
      text-align: center;
      padding: 20px;
      background: rgba(0,0,0,0.4);
      margin-top: 40px;
    }

    footer a {
      color: #00d9ff;
      text-decoration: none;
      margin: 0 10px;
      font-weight: 500;
    }

    footer a:hover {
      text-decoration: underline;
    }
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

  <section class="hero" id="hero">
    <h2>👋 Hi Coders!</h2>
    <p>
      I’m a Full-Stack Developer skilled in C, Java, Laravel, Flutter, and React.  
      I love building modern web & mobile apps that solve real-world problems.
    </p>
  </section>

  <section id="skills">
    <h3 class="section-title">💻 Skills</h3>
    <div class="skills">
      <div class="card">
        <h4>Languages</h4>
        <p>C, Java, PHP, JavaScript, Dart</p>
      </div>
      <div class="card">
        <h4>Web Development</h4>
        <p>Laravel, React, HTML, CSS</p>
      </div>
      <div class="card">
        <h4>Mobile Apps</h4>
        <p>Flutter, REST APIs</p>
      </div>
      <div class="card">
        <h4>Databases</h4>
        <p>MySQL, SQLite</p>
      </div>
    </div>
  </section>

  <section id="projects">
    <h3 class="section-title">🚀 Projects</h3>
    <div class="projects">
      <div class="card">
        <h4>Medical Clinic App</h4>
        <p>Full
