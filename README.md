<!--
  GitHub Profile README (HTML + CSS)
  - Paste this HTML into your README.md on GitHub (GitHub supports raw HTML inside Markdown)
  - Replace placeholders (NAME, BIO, PROJECT links, social links, avatar) with your own info
-->
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>GitHub Profile README</title>
  <style>
    :root{
      --bg:#0f1724; /* deep navy */
      --card:#0b1220; /* card background */
      --muted:#9aa8bf;
      --accent:#7c5cff; /* purple accent */
      --glass: rgba(255,255,255,0.04);
      --glass-2: rgba(255,255,255,0.02);
      --radius:14px;
      font-family: Inter, ui-sans-serif, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    }
    body{background:linear-gradient(180deg,#071027 0%, var(--bg) 100%); color:#e6eef8; margin:0; padding:36px;}
    .container{max-width:900px; margin:0 auto;}

    .profile-card{background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent); border:1px solid rgba(255,255,255,0.03); padding:26px; border-radius:var(--radius); display:flex; gap:22px; align-items:center;}
    .avatar{width:132px; height:132px; border-radius:16px; overflow:hidden; flex:0 0 132px; border:1px solid rgba(255,255,255,0.06); background:linear-gradient(135deg, rgba(124,92,255,0.12), rgba(124,92,255,0.04)); display:flex; align-items:center; justify-content:center}
    .avatar img{width:100%; height:100%; object-fit:cover}

    .hero{flex:1}
    h1{margin:0 0 6px 0; font-size:1.45rem; letter-spacing:0.2px}
    .handle{color:var(--muted); margin-bottom:8px}
    .bio{color:var(--muted); margin:8px 0 12px 0; line-height:1.4}
    .chips{display:flex; gap:8px; flex-wrap:wrap}
    .chip{background:var(--glass); padding:8px 10px; border-radius:999px; color: #dbe9ff; font-size:13px; border:1px solid rgba(255,255,255,0.02)}

    .actions{display:flex; gap:10px; margin-top:14px}
    .btn{padding:10px 14px; border-radius:12px; text-decoration:none; color:#fff; font-weight:600; font-size:14px; background:linear-gradient(90deg,var(--accent), #4ac7ff); box-shadow:0 6px 18px rgba(124,92,255,0.14)}

    .grid{display:grid; grid-template-columns: 1fr 320px; gap:20px; margin-top:20px}
    .card{background:var(--card); padding:18px; border-radius:12px; border:1px solid rgba(255,255,255,0.03)}
    .skills-list{display:flex; flex-direction:column; gap:10px}
    .skill{display:flex; justify-content:space-between; align-items:center}
    .skill-name{color:var(--muted); font-size:13px}
    .bar{height:10px; background:var(--glass-2); border-radius:999px; width:100%; margin-left:12px; position:relative; overflow:hidden}
    .bar > span{position:absolute; left:0; top:0; bottom:0; border-radius:999px}

    .projects{display:flex; flex-direction:column; gap:12px}
    .proj{display:flex; gap:12px; align-items:center}
    .proj img{width:64px; height:40px; object-fit:cover; border-radius:8px; border:1px solid rgba(255,255,255,0.04)}
    .proj a{color:#e6eef8; font-weight:600; text-decoration:none}
    .proj p{margin:3px 0 0 0; color:var(--muted); font-size:13px}

    .side{display:flex; flex-direction:column; gap:12px}
    .stat img{width:100%}

    footer{margin-top:22px; text-align:center; color:var(--muted); font-size:13px}

    /* Responsive */
    @media (max-width:880px){
      .grid{grid-template-columns:1fr;}
      .avatar{width:110px; height:110px}
    }

    /* small utility classes for inline bars */
    .w-95{width:95%; background:linear-gradient(90deg,#8be5ff, #7c5cff)}
    .w-90{width:90%; background:linear-gradient(90deg,#ffd27c, #7c5cff)}
    .w-85{width:85%; background:linear-gradient(90deg,#9cffb8, #7c5cff)}
    .w-75{width:75%; background:linear-gradient(90deg,#ff9cbc, #7c5cff)}
  </style>
</head>
<body>
  <div class="container">

    <div class="profile-card">
      <div class="avatar">
        <!-- Replace src with your avatar URL -->
        <img src="https://avatars.githubusercontent.com/u/583231?v=4" alt="avatar" />
      </div>

      <div class="hero">
        <h1>Madam Arya Akhade <span style="color:var(--accent); font-weight:700">• Frontend Engineer</span></h1>
        <div class="handle">React • HTML • CSS • JavaScript • Node.js • Java / Spring Boot • mySQL • MongoDB</div>
        <p class="bio">I build polished, accessible user interfaces and reliable back-end services. Passionate about performance, clean code, and mentoring juniors. Open to freelance and full-time roles.</p>

        <div class="chips">
          <div class="chip">React.js</div>
          <div class="chip">HTML &amp; CSS</div>
          <div class="chip">JavaScript (ES6+)</div>
          <div class="chip">Node.js</div>
          <div class="chip">Spring Boot</div>
          <div class="chip">mySQL • MongoDB</div>
        </div>

        <div class="actions">
          <a class="btn" href="#projects">Featured Projects</a>
          <a class="btn" href="#contact" style="background:linear-gradient(90deg,#0abf7a,#4ac7ff)">Contact</a>
        </div>
      </div>
    </div>

    <div class="grid">

      <!-- Left column -->
      <div>
        <div class="card">
          <h3 style="margin:0 0 10px 0">Key Skills</h3>
          <div class="skills-list">
            <div class="skill"><div class="skill-name">React.js</div><div style="flex:1; display:flex; align-items:center"><div class="bar"><span class="w-95" style="height:100%"></span></div></div></div>
            <div class="skill"><div class="skill-name">HTML &amp; CSS</div><div style="flex:1; display:flex; align-items:center"><div class="bar"><span class="w-90" style="height:100%"></span></div></div></div>
            <div class="skill"><div class="skill-name">JavaScript (ES6+)</div><div style="flex:1; display:flex; align-items:center"><div class="bar"><span class="w-85" style="height:100%"></span></div></div></div>
            <div class="skill"><div class="skill-name">Node.js</div><div style="flex:1; display:flex; align-items:center"><div class="bar"><span class="w-75" style="height:100%"></span></div></div></div>
            <div class="skill"><div class="skill-name">Java / Spring Boot</div><div style="flex:1; display:flex; align-items:center"><div class="bar"><span class="w-75" style="height:100%"></span></div></div></div>
            <div class="skill"><div class="skill-name">Databases</div><div style="flex:1; display:flex; align-items:center"><div class="bar"><span class="w-85" style="height:100%"></span></div></div></div>
          </div>
        </div>

        <div class="card" id="projects" style="margin-top:14px">
          <h3 style="margin:0 0 10px 0">Featured Projects</h3>
          <div class="projects">
            <div class="proj">
              <img src="https://via.placeholder.com/160x100.png?text=Project+1" alt="proj1">
              <div>
                <a href="#" target="_blank">E-Commerce UI (React)</a>
                <p>Product listing, cart, responsive design, optimized for performance.</p>
              </div>
            </div>

            <div class="proj">
              <img src="https://via.placeholder.com/160x100.png?text=Project+2" alt="proj2">
              <div>
                <a href="#" target="_blank">Task Manager (Node + MongoDB)</a>
                <p>REST API, authentication, MongoDB persistence.</p>
              </div>
            </div>

            <div class="proj">
              <img src="https://via.placeholder.com/160x100.png?text=Project+3" alt="proj3">
              <div>
                <a href="#" target="_blank">College Portal (Spring Boot + mySQL)</a>
                <p>Secure role-based system, CRUD operations, JDBC integration.</p>
              </div>
            </div>
          </div>
        </div>

        <div class="card" style="margin-top:14px">
          <h3 style="margin:0 0 10px 0">Open Source & Education</h3>
          <p style="color:var(--muted); margin:0">Contributor to small OSS projects. Completed multiple coursework and practical labs in Web Development and Backend APIs. Happy to mentor junior developers — DM me for guidance.</p>
        </div>

      </div>

      <!-- Right column (side) -->
      <aside class="side">
        <div class="card">
          <h4 style="margin:0 0 10px 0">Contact</h4>
          <p id="contact" style="color:var(--muted); margin:0 0 10px 0">Email: <strong style="color:#dfeaff">youremail@example.com</strong><br>Location: Mumbai, India</p>
          <div style="display:flex; gap:10px; margin-top:10px">
            <a class="chip" href="https://www.linkedin.com/" target="_blank">LinkedIn</a>
            <a class="chip" href="https://twitter.com/" target="_blank">Twitter</a>
          </div>
        </div>

        <div class="card stat">
          <h4 style="margin:0 0 10px 0">GitHub Stats</h4>
          <!-- You can replace these with your github-readme-stats links for dynamic images -->
          <img src="https://github-readme-stats.vercel.app/api?username=YOUR_GITHUB_USERNAME&show_icons=true&theme=radical" alt="github stats" />
        </div>

        <div class="card">
          <h4 style="margin:0 0 10px 0">Languages & Tools</h4>
          <div style="display:flex; flex-wrap:wrap; gap:8px">
            <div class="chip">VS Code</div>
            <div class="chip">Git</div>
            <div class="chip">Docker</div>
            <div class="chip">Figma</div>
            <div class="chip">Postman</div>
          </div>
        </div>

      </aside>

    </div>

    <footer>
      Built with ❤️ • React, Node.js, Java • mySQL &amp; MongoDB • Available for hire / freelance
    </footer>

  </div>
</body>
</html>
