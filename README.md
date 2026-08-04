<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Mohammad Ibrahim Khan | Developer Profile</title>
  <meta name="description" content="Mohammad Ibrahim Khan — AI/ML, Full Stack, Cloud" />
  <style>
    :root{
      --bg:#0b0f14;
      --panel:#111823;
      --panel-2:#0f151d;
      --text:#e8eef7;
      --muted:#9fb0c5;
      --line:#223043;
      --accent:#6ea8fe;
      --accent-2:#8b5cf6;
    }
    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{
      margin:0;
      font-family:Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      background:
        radial-gradient(circle at top right, rgba(110,168,254,.10), transparent 32%),
        radial-gradient(circle at top left, rgba(139,92,246,.08), transparent 28%),
        var(--bg);
      color:var(--text);
      line-height:1.65;
    }
    a{color:inherit;text-decoration:none}
    .wrap{max-width:1100px;margin:auto;padding:28px 20px 70px}
    .hero{
      min-height:72vh;
      display:flex;
      flex-direction:column;
      justify-content:center;
      align-items:center;
      text-align:center;
      padding:60px 20px 40px;
    }
    .eyebrow{
      display:inline-flex;
      gap:8px;
      align-items:center;
      border:1px solid var(--line);
      background:rgba(17,24,35,.75);
      padding:8px 12px;
      border-radius:999px;
      color:var(--muted);
      font-size:14px;
      backdrop-filter: blur(10px);
    }
    h1{
      font-size:clamp(42px,7vw,78px);
      line-height:1.02;
      margin:20px 0 14px;
      letter-spacing:-2px;
    }
    .gradient{
      background:linear-gradient(90deg,var(--accent),var(--accent-2));
      -webkit-background-clip:text;
      background-clip:text;
      color:transparent;
    }
    .subtitle{
      max-width:780px;
      font-size:clamp(18px,2.2vw,25px);
      color:var(--muted);
      margin:0 auto 24px;
    }
    .typing{
      min-height:34px;
      font-family:"SFMono-Regular",Consolas,"Liberation Mono",monospace;
      color:#cdd9e5;
      font-size:16px;
      margin:10px 0 28px;
    }
    .cursor{display:inline-block;width:8px;animation:blink 1s steps(1) infinite}
    @keyframes blink{50%{opacity:0}}
    .actions{display:flex;gap:12px;flex-wrap:wrap;justify-content:center}
    .btn{
      border:1px solid var(--line);
      background:var(--panel);
      padding:11px 16px;
      border-radius:12px;
      font-weight:650;
      transition:.2s ease;
    }
    .btn:hover{transform:translateY(-2px);border-color:#47617f}
    .btn.primary{
      background:linear-gradient(135deg,#1d4ed8,#6d28d9);
      border-color:transparent;
    }
    section{margin-top:56px}
    .section-title{font-size:27px;margin:0 0 20px;letter-spacing:-.5px}
    .grid{display:grid;gap:16px}
    .grid.two{grid-template-columns:repeat(2,minmax(0,1fr))}
    .card{
      background:linear-gradient(180deg,rgba(17,24,35,.92),rgba(15,21,29,.92));
      border:1px solid var(--line);
      border-radius:18px;
      padding:22px;
      transition:.2s ease;
    }
    .card:hover{
      transform:translateY(-3px);
      border-color:#3c5370;
      box-shadow:0 12px 35px rgba(0,0,0,.22);
    }
    .muted{color:var(--muted)}
    pre{
      margin:0;
      overflow:auto;
      background:#0a0f15;
      border:1px solid #1b2838;
      border-radius:14px;
      padding:18px;
      color:#c8d6e5;
      font-size:14px;
    }
    .tech-grid{
      display:grid;
      grid-template-columns:repeat(6,minmax(0,1fr));
      border:1px solid var(--line);
      border-radius:16px;
      overflow:hidden;
      background:var(--panel-2);
    }
    .tech{
      padding:18px 8px;
      text-align:center;
      border-right:1px solid var(--line);
      border-bottom:1px solid var(--line);
    }
    .tech:nth-child(6n){border-right:none}
    .tech img{width:42px;height:42px;display:block;margin:0 auto 8px}
    .tech span{font-size:14px}
    .pills{display:flex;gap:10px;flex-wrap:wrap}
    .pill{
      border:1px solid var(--line);
      background:#0c1219;
      color:#c9d7e8;
      padding:7px 10px;
      border-radius:999px;
      font-size:13px;
    }
    .project h3{margin:0 0 8px;font-size:21px}
    .project .tagline{color:#c5d2e3;margin-bottom:12px}
    .stats{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:16px;
      align-items:start;
    }
    .stats img,.activity img{
      width:100%;
      border-radius:14px;
      border:1px solid var(--line);
      background:#0d1117;
    }
    .milestones{display:flex;flex-wrap:wrap;gap:10px}
    footer{
      text-align:center;
      margin-top:72px;
      padding-top:28px;
      border-top:1px solid var(--line);
      color:var(--muted);
    }
    .quote{
      font-family:"SFMono-Regular",Consolas,monospace;
      color:#d4def0;
      font-size:17px;
    }
    @media(max-width:850px){
      .grid.two,.stats{grid-template-columns:1fr}
      .tech-grid{grid-template-columns:repeat(3,minmax(0,1fr))}
      .tech:nth-child(6n){border-right:1px solid var(--line)}
      .tech:nth-child(3n){border-right:none}
    }
    @media(max-width:520px){
      .tech-grid{grid-template-columns:repeat(2,minmax(0,1fr))}
      .tech:nth-child(3n){border-right:1px solid var(--line)}
      .tech:nth-child(2n){border-right:none}
      h1{letter-spacing:-1px}
    }
  </style>
</head>
<body>
  <main class="wrap">
    <section class="hero">
      <div class="eyebrow">AI/ML · Full Stack · Cloud</div>
      <h1>Mohammad <span class="gradient">Ibrahim Khan</span></h1>
      <p class="subtitle">I like building things that think, scale, and solve actual problems.</p>
      <div class="typing"><span id="typed"></span><span class="cursor">▌</span></div>

      <div class="actions">
        <a class="btn primary" href="https://www.linkedin.com/in/MohammadIbrahimKhan" target="_blank">LinkedIn</a>
        <a class="btn" href="mailto:ibrahimhere0123@gmail.com">Email</a>
        <a class="btn" href="https://github.com/thisisibrahim" target="_blank">GitHub</a>
      </div>
    </section>

    <section>
      <h2 class="section-title">⚡ A Little About Me</h2>
      <div class="grid two">
        <div class="card">
<pre>ibrahim = {
  "focus": ["Artificial Intelligence", "RAG", "Full Stack", "Cloud"],
  "building": "AI systems that solve real-world problems",
  "interests": ["NLP", "Computer Vision", "Open Source"],
  "philosophy": "Build → Break → Learn → Improve"
}</pre>
        </div>
        <div class="card">
          <p>🎓 Computer Science at <strong>VIT Bhopal University</strong></p>
          <p>☁️ Specializing in <strong>Cloud Computing & Automation</strong></p>
          <p>🧠 Building with <strong>AI, RAG, NLP and Machine Learning</strong></p>
          <p>💻 Enjoy taking systems from backend → frontend → deployment</p>
          <p>🌱 Exploring and contributing to <strong>Open Source</strong></p>
        </div>
      </div>
    </section>

    <section>
      <h2 class="section-title">🛠️ Languages & Tools</h2>
      <div class="tech-grid">
        <div class="tech"><img src="https://skillicons.dev/icons?i=python" alt="Python"><span>Python</span></div>
        <div class="tech"><img src="https://skillicons.dev/icons?i=cpp" alt="C++"><span>C++</span></div>
        <div class="tech"><img src="https://skillicons.dev/icons?i=js" alt="JavaScript"><span>JavaScript</span></div>
        <div class="tech"><img src="https://skillicons.dev/icons?i=angular" alt="Angular"><span>Angular</span></div>
        <div class="tech"><img src="https://skillicons.dev/icons?i=react" alt="React"><span>React</span></div>
        <div class="tech"><img src="https://skillicons.dev/icons?i=nodejs" alt="Node.js"><span>Node.js</span></div>

        <div class="tech"><img src="https://skillicons.dev/icons?i=django" alt="Django"><span>Django</span></div>
        <div class="tech"><img src="https://skillicons.dev/icons?i=aws" alt="AWS"><span>AWS</span></div>
        <div class="tech"><img src="https://skillicons.dev/icons?i=docker" alt="Docker"><span>Docker</span></div>
        <div class="tech"><img src="https://skillicons.dev/icons?i=linux" alt="Linux"><span>Linux</span></div>
        <div class="tech"><img src="https://skillicons.dev/icons?i=mongodb" alt="MongoDB"><span>MongoDB</span></div>
        <div class="tech"><img src="https://skillicons.dev/icons?i=mysql" alt="MySQL"><span>MySQL</span></div>

        <div class="tech"><img src="https://skillicons.dev/icons?i=git" alt="Git"><span>Git</span></div>
        <div class="tech"><img src="https://skillicons.dev/icons?i=github" alt="GitHub"><span>GitHub</span></div>
        <div class="tech"><img src="https://skillicons.dev/icons?i=postman" alt="Postman"><span>Postman</span></div>
        <div class="tech"><img src="https://skillicons.dev/icons?i=html" alt="HTML"><span>HTML</span></div>
        <div class="tech"><img src="https://skillicons.dev/icons?i=css" alt="CSS"><span>CSS</span></div>
        <div class="tech"><img src="https://skillicons.dev/icons?i=mysql" alt="SQL"><span>SQL</span></div>
      </div>
    </section>

    <section>
      <h2 class="section-title">🧠 AI / ML Playground</h2>
      <div class="pills">
        <span class="pill">RAG Systems</span>
        <span class="pill">LangChain</span>
        <span class="pill">NLP</span>
        <span class="pill">Transformers</span>
        <span class="pill">Scikit-learn</span>
        <span class="pill">Pandas</span>
        <span class="pill">NumPy</span>
        <span class="pill">Computer Vision</span>
      </div>
    </section>

    <section>
      <h2 class="section-title">🚀 Things I've Built</h2>
      <div class="grid two">
        <article class="card project">
          <h3>🩺 MedSenseAI</h3>
          <div class="tagline">Safety-First Medical Report Explainer</div>
          <p class="muted">Turns complex medical reports into understandable explanations using a safety-first AI pipeline.</p>
          <div class="pills">
            <span class="pill">RAG</span><span class="pill">LangChain</span><span class="pill">Python</span><span class="pill">Pydantic</span>
          </div>
        </article>

        <article class="card project">
          <h3>🗣️ LearnX</h3>
          <div class="tagline">AI Debate Practice Platform</div>
          <p class="muted">Interactive debate practice with speech recognition, timed sessions, and structured feedback.</p>
          <div class="pills">
            <span class="pill">Angular</span><span class="pill">JavaScript</span><span class="pill">Web Speech API</span>
          </div>
        </article>

        <article class="card project" style="grid-column:1/-1">
          <h3>🫀 Coronary CT Microcalcification Detection</h3>
          <div class="tagline">Deep Learning for Medical Imaging</div>
          <p class="muted">Research-oriented computer vision project focused on detecting coronary microcalcifications from CT scans.</p>
          <div class="pills">
            <span class="pill">CNN</span><span class="pill">ResNet-50</span><span class="pill">U-Net</span><span class="pill">Python</span>
          </div>
        </article>
      </div>
    </section>

    <section>
      <h2 class="section-title">📊 GitHub, But Make It Visual</h2>
      <div class="stats">
        <img src="https://github-readme-stats.vercel.app/api?username=thisisibrahim&show_icons=true&hide_border=true&theme=github_dark&rank_icon=github" alt="GitHub stats">
        <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=thisisibrahim&layout=compact&hide_border=true&theme=github_dark" alt="Top languages">
      </div>
    </section>

    <section>
      <h2 class="section-title">🔥 GitHub Streak</h2>
      <div class="activity">
        <img src="https://github-readme-streak-stats.herokuapp.com/?user=thisisibrahim&theme=github-dark-blue&hide_border=true" alt="GitHub streak">
      </div>
    </section>

    <section>
      <h2 class="section-title">📈 Contribution Journey</h2>
      <div class="activity">
        <img src="https://github-readme-activity-graph.vercel.app/graph?username=thisisibrahim&theme=github-compact&hide_border=true&area=true" alt="Contribution graph">
      </div>
    </section>

    <section>
      <h2 class="section-title">🏆 A Few Milestones</h2>
      <div class="milestones">
        <span class="pill">☁️ OCI Developer Professional</span>
        <span class="pill">☁️ AWS Cloud Practitioner</span>
        <span class="pill">🌍 GSSoC Contributor</span>
        <span class="pill">📊 Accenture Data Analytics</span>
        <span class="pill">💻 Full-Stack Development</span>
      </div>
    </section>

    <footer>
      <div class="quote">while(alive) { learn(); build(); improve(); }</div>
      <p>Open to Open Source · AI Projects · Interesting Engineering Problems</p>
    </footer>
  </main>

  <script>
    const lines = [
      "Building AI-powered systems 🧠",
      "Exploring RAG & intelligent applications 🤖",
      "Full-Stack + Cloud Engineering ☁️",
      "Turning ideas into working software 🚀"
    ];

    const target = document.getElementById("typed");
    let line = 0, char = 0, deleting = false;

    function tick(){
      const text = lines[line];
      target.textContent = deleting ? text.slice(0, char--) : text.slice(0, char++);

      let delay = deleting ? 35 : 55;

      if (!deleting && char > text.length){
        deleting = true;
        delay = 1300;
      } else if (deleting && char < 0){
        deleting = false;
        line = (line + 1) % lines.length;
        char = 0;
        delay = 300;
      }

      setTimeout(tick, delay);
    }
    tick();
  </script>
</body>
</html>
