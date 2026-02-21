# Portfolio

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Valencia C. Davila — Data Scientist</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Fira+Code&display=swap" rel="stylesheet">
<style>
/* ---- COLORS: Change these to customize your look ---- */
:root {
  --accent: #2563eb;        /* Main color: try #7c3aed (purple) or #059669 (green) */
  --accent-bg: #eff6ff;     /* Light version of your accent */
  --dark: #0f172a;
  --text: #334155;
  --muted: #64748b;
  --border: #e2e8f0;
  --bg: #f8fafc;
}

* { box-sizing: border-box; margin: 0; padding: 0; }
html { scroll-behavior: smooth; }
body {
  font-family: 'Inter', sans-serif;
  background: #fff;
  color: var(--text);
  line-height: 1.6;
}

/* ---- NAVIGATION ---- */
nav {
  position: sticky;
  top: 0;
  background: rgba(255,255,255,0.95);
  backdrop-filter: blur(10px);
  border-bottom: 1px solid var(--border);
  padding: 1rem 2rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
  z-index: 100;
}
nav .logo { font-weight: 700; color: var(--dark); text-decoration: none; }
nav ul { list-style: none; display: flex; gap: 1.5rem; }
nav a { color: var(--muted); text-decoration: none; font-size: 0.9rem; font-weight: 500; }
nav a:hover { color: var(--accent); }

/* ---- HERO ---- */
.hero {
  min-height: 90vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 4rem 2rem;
  max-width: 900px;
  margin: 0 auto;
}
.hero-greeting { color: var(--accent); font-weight: 600; margin-bottom: 0.5rem; }
.hero h1 { font-size: clamp(2.5rem, 5vw, 4rem); color: var(--dark); line-height: 1.1; margin-bottom: 1rem; }
.hero h2 { font-size: 1.3rem; font-weight: 400; color: var(--muted); margin-bottom: 2rem; max-width: 600px; }
.hero-links { display: flex; gap: 1rem; flex-wrap: wrap; margin-bottom: 2.5rem; }
.btn {
  padding: 0.65rem 1.5rem;
  border-radius: 8px;
  font-weight: 600;
  text-decoration: none;
  font-size: 0.9rem;
  transition: all 0.2s;
}
.btn-primary { background: var(--accent); color: white; }
.btn-primary:hover { opacity: 0.85; transform: translateY(-1px); }
.btn-outline { border: 2px solid var(--border); color: var(--text); }
.btn-outline:hover { border-color: var(--accent); color: var(--accent); }
.hero-tools { color: var(--muted); font-size: 0.85rem; }
.hero-tools span { font-weight: 600; color: var(--dark); margin: 0 0.4rem; }

/* ---- SECTIONS ---- */
section { padding: 5rem 2rem; max-width: 900px; margin: 0 auto; }
.section-label {
  font-size: 0.75rem;
  font-weight: 700;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--accent);
  margin-bottom: 0.75rem;
}
h2 { font-size: 2rem; color: var(--dark); margin-bottom: 1.5rem; }
p { margin-bottom: 1rem; }

/* ---- SKILLS ---- */
.skills-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 1rem; margin-top: 1.5rem; }
.skill-group { background: var(--bg); border: 1px solid var(--border); border-radius: 10px; padding: 1.25rem; }
.skill-group h4 { font-size: 0.8rem; text-transform: uppercase; letter-spacing: 0.08em; color: var(--accent); margin-bottom: 0.75rem; }
.skill-tags { display: flex; flex-wrap: wrap; gap: 0.4rem; }
.skill-tag {
  background: white;
  border: 1px solid var(--border);
  border-radius: 4px;
  padding: 0.2rem 0.6rem;
  font-size: 0.8rem;
  color: var(--text);
}

/* ---- PROJECTS ---- */
.projects-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 1.5rem; }
.project-card {
  border: 1px solid var(--border);
  border-radius: 12px;
  padding: 1.5rem;
  transition: all 0.2s;
}
.project-card:hover { border-color: var(--accent); box-shadow: 0 4px 20px rgba(37,99,235,0.1); transform: translateY(-2px); }
.project-card h3 { font-size: 1.1rem; color: var(--dark); margin-bottom: 0.5rem; }
.project-card p { font-size: 0.88rem; color: var(--muted); margin-bottom: 1rem; }
.tech-tags { display: flex; flex-wrap: wrap; gap: 0.35rem; margin-bottom: 1rem; }
.tech-tag {
  background: var(--accent-bg);
  color: var(--accent);
  padding: 0.15rem 0.5rem;
  border-radius: 4px;
  font-size: 0.73rem;
  font-weight: 600;
}
.project-links { display: flex; gap: 0.75rem; }
.project-link {
  font-size: 0.82rem;
  font-weight: 600;
  color: var(--accent);
  text-decoration: none;
}
.project-link:hover { text-decoration: underline; }

/* ---- CONTACT ---- */
.contact-section { background: var(--dark); color: white; max-width: 100%; padding: 5rem 2rem; }
.contact-inner { max-width: 600px; margin: 0 auto; text-align: center; }
.contact-section h2 { color: white; margin-bottom: 1rem; }
.contact-section p { color: #94a3b8; margin-bottom: 2rem; }
.contact-links { display: flex; justify-content: center; gap: 1rem; flex-wrap: wrap; }

@media (max-width: 600px) {
  nav ul { display: none; }
  .hero h1 { font-size: 2.2rem; }
}
</style>
</head>
<body>

<!-- NAVIGATION -->
<nav>
  <a class="logo" href="#">Valencia</a>
  <ul>
    <li><a href="#about">About</a></li>
    <li><a href="#projects">Projects</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>

<!-- HERO: Replace all YOUR_... placeholders -->
<div class="hero">
  <div class="hero-greeting">Hi, I'm</div>
  <h1>Valencia.</h1>
  <h2>Results-driven Data Scientist experienced in end-to-end data pipelines, machine learning, and data visualization to solve complex business problems.
    <!-- Example: "Data scientist who turns messy business data into clear decisions." -->
  </h2>
  <div class="hero-links">
    <a class="btn btn-primary" href="#projects">See My Work</a>
    <a class="btn btn-outline" href="https://github.com/iamvalenciad" target="_blank">GitHub</a>
    <a class="btn btn-outline" href="https://linkedin.com/in//valencia-davila-3575b6a5/" target="_blank">LinkedIn</a>
  </div>
  <div class="hero-tools">
    Tools I work with:
    <span>Python</span> ·
    <span>SQL</span> ·
    <span>Tableau</span> ·
    <span>R</span>
  </div>
</div>

<!-- ABOUT -->
<section id="about">
  <div class="section-label">About Me</div>
  <h2>Background & Skills</h2>
  <p>I'm a data scientist focused on building models that drive real business decisions.
    I'm currently seeking full-time roles in data science, data analytics, and finance.
  </p>

  <div class="skills-grid">
    <div class="skill-group">
      <h4>Languages</h4>
      <div class="skill-tags">
        <span class="skill-tag">Python</span>
        <span class="skill-tag">SQL</span>
        <span class="skill-tag">R</span>
      </div>
    </div>
    <div class="skill-group">
      <h4>Libraries</h4>
      <div class="skill-tags">
        <span class="skill-tag">Pandas</span>
        <span class="skill-tag">Scikit-learn</span>
        <span class="skill-tag">Matplotlib</span>
        <span class="skill-tag">Seaborn</span>
      </div>
    </div>
    <div class="skill-group">
      <h4>Tools</h4>
      <div class="skill-tags">
        <span class="skill-tag">Git</span>
        <span class="skill-tag">Tableau</span>
      </div>
    </div>
  </div>
</section>

<!-- PROJECTS: Duplicate the .project-card div for each project -->
<section id="projects">
  <div class="section-label">Selected Projects</div>
  <h2>What I've Built</h2>
  <div class="projects-grid">

    <!-- PROJECT 1 -->
    <div class="project-card">
      <h3>YOUR_PROJECT_1_TITLE</h3>
      <p>YOUR_PROJECT_1_DESCRIPTION (2-3 sentences: problem, approach, result)</p>
      <div class="tech-tags">
        <span class="tech-tag">Python</span>
        <span class="tech-tag">YOUR_TECH</span>
      </div>
      <div class="project-links">
        <a class="project-link" href="YOUR_GITHUB_REPO_URL" target="_blank">→ GitHub</a>
        <!-- If you have a live demo, add: -->
        <!-- <a class="project-link" href="YOUR_DEMO_URL" target="_blank">→ Live Demo</a> -->
      </div>
    </div>

    <!-- PROJECT 2: Copy and paste the block above and replace -->
    <!-- PROJECT 3: Copy and paste again -->

  </div>
</section>

<!-- CONTACT -->
<section class="contact-section" id="contact">
  <div class="contact-inner">
    <h2>Let's Connect</h2>
    <p>Open to full-time roles and collaborations. Feel free to reach out!</p>
    <div class="contact-links">
      <a class="btn btn-primary" href="mailto:valencia.davila31@gmail.com">Email Me</a>
     <a class="btn btn-outline" style="border-color:#334155;color:#94a3b8" href="https://github.com/YOUR_GITHUB" target="_blank">GitHub</a>
    </div>
  </div>
</section>

</body>
</html>
