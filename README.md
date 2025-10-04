<!doctype html>
<html lang="fr">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Portfolio | Développeur Full-Stack</title>
  <meta name="description" content="Portfolio d'un développeur full-stack maîtrisant C, Java, Laravel, Flutter et React." />
  <meta property="og:title" content="Portfolio | Développeur Full-Stack" />
  <meta property="og:description" content="Développement web et mobile avec Laravel, Flutter, React, ainsi que C et Java." />
  <link rel="icon" href="data:;base64,iVBORw0KGgo=" />

  <style>
    :root{
      --bg:#0f1724;
      --card:#0b1220;
      --accent:#16a34a;
      --muted:#94a3b8;
      --glass: rgba(255,255,255,0.04);
      color-scheme: dark;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family:Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
      background:linear-gradient(180deg,var(--bg),#071022);
      color:#e6eef8;
      line-height:1.5
    }
    .container{max-width:1000px;margin:40px auto;padding:24px}
    header{display:flex;align-items:center;justify-content:space-between;gap:12px}
    .brand{display:flex;gap:12px;align-items:center}
    .logo{
      width:48px;height:48px;border-radius:10px;
      background:linear-gradient(135deg,var(--accent),#15803d);
      display:flex;align-items:center;justify-content:center;font-weight:700
    }
    nav a{color:var(--muted);text-decoration:none;margin-left:16px}
    nav a:hover{color:white}
    .hero{display:grid;grid-template-columns:1fr 340px;gap:24px;margin-top:28px}
    .card{
      background:var(--card);padding:22px;border-radius:12px;
      backdrop-filter: blur(6px);box-shadow:0 6px 18px rgba(2,6,23,0.6)
    }
    h1,h2,h3,h4{margin-top:0}
    h1{font-size:32px;margin-bottom:8px}
    p.lead{margin:0 0 18px;color:var(--muted)}
    .actions{display:flex;gap:12px;margin-bottom:12px}
    .btn{padding:10px 14px;border-radius:10px;border:0;cursor:pointer;font-weight:600}
    .btn-primary{background:linear-gradient(90deg,var(--accent),#15803d);color:white}
    .btn-light{background:var(--glass);color:var(--muted)}
    .features{display:grid;grid-template-columns:repeat(auto-fill,minmax(220px,1fr));gap:12px;margin-top:18px}
    .feature{
      padding:14px;border-radius:8px;
      background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);
      border:1px solid rgba(255,255,255,0.03)
    }
    footer{margin-top:28px;color:var(--muted);font-size:14px;text-align:center}

    @media (max-width:880px){
      .hero{grid-template-columns:1fr;}
      nav{display:none}
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="logo">DEV</div>
        <div>
          <div style="font-weight:700">Portfolio Full-Stack</div>
          <div style="font-size:13px;color:var(--muted)">C | Java | Laravel | Flutter | React</div>
        </div>
      </div>
      <nav>
        <a href="#about">À propos</a>
        <a href="#skills">Compétences</a>
        <a href="#projects">Projets</a>
        <a href="#contact">Contact</a>
      </nav>
    </header>

    <main class="hero">
      <section class="card">
        <h1>Salut, je suis Développeur Full-Stack</h1>
        <p class="lead">Je conçois et développe des applications web et mobiles en utilisant Laravel, Flutter et React, tout en maîtrisant la programmation en C et Java.</p>

        <div class="actions">
          <button class="btn btn-primary" onclick="document.getElementById('projects').scrollIntoView()">Voir mes projets</button>
          <button class="btn btn-light" onclick="document.getElementById('contact').scrollIntoView()">Me contacter</button>
        </div>

        <h2 id="skills">Compétences</h2>
        <div class="features">
          <div class="feature">
            <strong>C</strong>
            <div style="color:var(--muted);font-size:13px">Programmation système et algorithmique.</div>
          </div>
          <div class="feature">
            <strong>Java</strong>
            <div style="color:var(--muted);font-size:13px">Applications desktop et backend robuste.</div>
          </div>
          <div class="feature">
            <strong>Laravel</strong>
            <div style="color:var(--muted);font-size:13px">Framework PHP pour APIs et backends sécurisés.</div>
          </div>
          <div class="feature">
            <strong>Flutter</strong>
            <div style="color:var(--muted);font-size:13px">Applications mobiles multiplateformes modernes.</div>
          </div>
          <div class="feature">
            <strong>React</strong>
            <div style="color:var(--muted);font-size:13px">Interfaces web dynamiques et SPA.</div>
          </div>
        </div>
      </section>

      <aside class="card" id="about">
        <h3>À propos de moi</h3>
        <p style="color:var(--muted);font-size:14px">
          Je suis un passionné du développement logiciel. J'aime créer des solutions efficaces pour le web, le mobile et le desktop, avec une solide base en algorithmique et en programmation orientée objet.
        </p>

        <h4 style="margin-top:12px">Mon approche</h4>
        <ul style="color:var(--muted);padding-left:18px">
          <li>Code maintenable et évolutif</li>
          <li>Performance et expérience utilisateur</li>
          <li>Intégration continue et bonnes pratiques</li>
        </ul>
      </aside>
    </main>

    <section id="projects" class="card" style="margin-top:20px">
      <h2>Projets récents</h2>
      <div class="features">
        <div class="feature">
          <strong>App Médicale</strong>
          <div style="color:var(--muted);font-size:13px">Système complet avec Laravel (backend), Flutter (mobile) et React (web) pour gérer les patients et rendez-vous.</div>
        </div>
        <div class="feature">
          <strong>Shop Mobile</strong>
          <div style="color:var(--muted);font-size:13px">Application Flutter pour une supérette avec gestion de panier et API produits.</div>
        </div>
        <div class="feature">
          <strong>Dashboard Admin</strong>
          <div style="color:var(--muted);font-size:13px">Interface React pour superviser les données d’entreprise en temps réel.</div>
        </div>
        <div class="feature">
          <strong>Librairie en C & Java</strong>
          <div style="color:var(--muted);font-size:13px">Outils et algorithmes développés pour l’apprentissage et l’optimisation.</div>
        </div>
      </div>
    </section>

    <section id="contact" class="card" style="margin-top:20px">
      <h2>Contact</h2>
      <p style="color:var(--muted);font-size:14px">
        Vous pouvez m'écrire à <code>votre.email@exemple.com</code> ou visiter mon 
        <a href="https://github.com/" style="color:var(--accent)">GitHub</a>.
      </p>
    </section>

    <footer>
      <div>© <span id="year"></span> Développeur Full-Stack | C, Java, Laravel, Flutter, React</div>
    </footer>
  </div>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
