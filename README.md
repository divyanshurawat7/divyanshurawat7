<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Divyanshu Rawat · AI/ML Developer</title>
  <!-- Font Awesome for icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" />
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: #0d1117;
      color: #e6edf3;
      font-family: 'Segoe UI', -apple-system, BlinkMacSystemFont, Roboto, 'Helvetica Neue', sans-serif;
      line-height: 1.6;
      padding: 2rem 1.5rem;
    }

    .container {
      max-width: 1000px;
      margin: 0 auto;
      background: #161b22;
      border-radius: 32px;
      padding: 2.5rem 2rem;
      box-shadow: 0 20px 40px -12px rgba(0, 0, 0, 0.8);
      border: 1px solid #30363d;
    }

    /* ---------- TYPOGRAPHY ---------- */
    h1, h2, h3, h4 {
      font-weight: 600;
      letter-spacing: -0.02em;
    }

    h1 {
      font-size: 2.8rem;
      background: linear-gradient(135deg, #f0883e, #f6a85b);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      display: inline-block;
      margin-bottom: 0.25rem;
    }

    h2 {
      font-size: 1.8rem;
      margin: 2rem 0 1rem 0;
      border-bottom: 2px solid #30363d;
      padding-bottom: 0.5rem;
      color: #f0e6d0;
    }

    h3 {
      font-size: 1.4rem;
      color: #f0e6d0;
      margin: 1.2rem 0 0.6rem 0;
    }

    .center {
      text-align: center;
    }

    .tagline {
      font-size: 1.2rem;
      color: #b1bac4;
      margin-top: -0.2rem;
      font-weight: 400;
      letter-spacing: 0.3px;
    }

    .badge-group {
      margin: 1.2rem 0 0.8rem 0;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 0.8rem;
    }

    .badge-group a {
      text-decoration: none;
    }

    .badge-group img {
      height: 32px;
      border-radius: 6px;
      transition: transform 0.15s ease;
    }

    .badge-group img:hover {
      transform: scale(1.04);
    }

    .view-count {
      margin: 0.8rem 0 1.5rem 0;
    }

    hr {
      border: 0;
      height: 1px;
      background: #30363d;
      margin: 2.5rem 0;
    }

    /* ---------- CARDS / PROJECTS ---------- */
    .project-card {
      background: #0d1117;
      border-radius: 20px;
      padding: 1.5rem 1.8rem;
      margin: 1.8rem 0;
      border: 1px solid #30363d;
      transition: border-color 0.2s, box-shadow 0.2s;
    }

    .project-card:hover {
      border-color: #f0883e;
      box-shadow: 0 8px 24px rgba(240, 136, 62, 0.06);
    }

    .project-title {
      font-size: 1.6rem;
      font-weight: 600;
      color: #f0e6d3;
      display: flex;
      align-items: center;
      gap: 8px;
      flex-wrap: wrap;
    }

    .project-title i {
      color: #f0883e;
      font-size: 1.5rem;
    }

    .project-sub {
      font-weight: 400;
      color: #b1bac4;
      font-size: 1rem;
      margin: 0.2rem 0 0.6rem 0;
    }

    .project-desc {
      margin: 0.6rem 0 0.8rem 0;
      color: #d1d9e6;
    }

    .highlight-list {
      list-style: none;
      display: flex;
      flex-wrap: wrap;
      gap: 0.4rem 1rem;
      margin: 0.6rem 0 0.8rem 0;
      padding-left: 0;
    }

    .highlight-list li {
      background: #21262d;
      padding: 0.1rem 0.8rem;
      border-radius: 30px;
      font-size: 0.85rem;
      color: #c9d1d9;
      border: 1px solid #30363d;
    }

    .stack-tag {
      display: inline-block;
      background: #1c2333;
      padding: 0.15rem 0.9rem;
      border-radius: 30px;
      font-size: 0.8rem;
      color: #b1bac4;
      border: 1px solid #30363d;
      margin-right: 0.4rem;
      margin-bottom: 0.3rem;
    }

    .repo-link {
      display: inline-block;
      margin-top: 0.7rem;
      background: #238636;
      color: #ffffff;
      padding: 0.4rem 1.2rem;
      border-radius: 30px;
      font-weight: 500;
      text-decoration: none;
      font-size: 0.9rem;
      transition: background 0.2s;
    }

    .repo-link:hover {
      background: #2ea043;
    }

    .repo-link i {
      margin-right: 6px;
    }

    /* ---------- TECH GRID ---------- */
    .tech-group {
      display: flex;
      flex-wrap: wrap;
      gap: 0.6rem 1rem;
      margin: 0.8rem 0 1.2rem 0;
    }

    .tech-group img {
      height: 34px;
      border-radius: 8px;
      transition: transform 0.15s;
    }

    .tech-group img:hover {
      transform: scale(1.04);
    }

    /* ---------- WHAT I BUILD TABLE ---------- */
    .build-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
      gap: 1rem;
      margin: 1rem 0 1.8rem 0;
    }

    .build-col {
      background: #0d1117;
      border-radius: 16px;
      padding: 1.2rem 1rem;
      border: 1px solid #30363d;
    }

    .build-col h4 {
      color: #f0883e;
      font-size: 1.1rem;
      margin-bottom: 0.6rem;
    }

    .build-col ul {
      list-style: none;
      padding-left: 0;
    }

    .build-col ul li {
      padding: 0.2rem 0;
      color: #c9d1d9;
      font-size: 0.95rem;
      border-bottom: 1px solid #21262d;
    }

    .build-col ul li:last-child {
      border-bottom: 0;
    }

    /* ---------- CODE BLOCK ---------- */
    .code-flow {
      background: #0d1117;
      border-radius: 16px;
      padding: 1.2rem 1.8rem;
      font-family: 'Fira Code', 'Cascadia Code', monospace;
      font-size: 0.95rem;
      border: 1px solid #30363d;
      color: #b1bac4;
      margin: 1rem 0;
      white-space: pre-wrap;
      line-height: 1.7;
    }

    /* ---------- STATS CARDS ---------- */
    .stats-grid {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 1.2rem;
      margin: 1.5rem 0;
    }

    .stats-grid img {
      max-width: 100%;
      height: auto;
      border-radius: 12px;
      border: 1px solid #30363d;
      background: #0d1117;
    }

    /* ---------- RESPONSIVE ---------- */
    @media (max-width: 640px) {
      .container {
        padding: 1.5rem 1rem;
      }
      h1 {
        font-size: 2.2rem;
      }
      .project-title {
        font-size: 1.3rem;
      }
      .build-grid {
        grid-template-columns: 1fr;
      }
      .badge-group img {
        height: 28px;
      }
      .code-flow {
        font-size: 0.8rem;
        padding: 1rem;
      }
    }

    /* ---------- MISC ---------- */
    .footer-wave {
      margin-top: 2.5rem;
    }

    .footer-wave img {
      width: 100%;
      max-width: 600px;
      border-radius: 0 0 30px 30px;
    }

    .connect-links {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 1rem;
      margin: 1.5rem 0 1rem 0;
    }

    .connect-links a {
      text-decoration: none;
    }

    .connect-links img {
      height: 38px;
      border-radius: 8px;
      transition: transform 0.15s;
    }

    .connect-links img:hover {
      transform: scale(1.05);
    }

    .quote {
      font-size: 1.2rem;
      font-weight: 300;
      color: #b1bac4;
      margin: 1.2rem 0 0.8rem 0;
      letter-spacing: 0.5px;
    }

    /* inline icon spacing */
    .icon-mr {
      margin-right: 6px;
    }
  </style>
</head>
<body>
<div class="container">

  <!-- HEADER -->
  <div align="center">
    <h1>👋 Hey, I'm Divyanshu Rawat</h1>
    <div class="tagline">🤖 AI/ML Developer · 📊 Data Analyst · 💻 Full-Stack Builder</div>
    <p style="color:#b1bac4; margin-top:0.2rem;"><strong>I build intelligent applications, analyze real-world data, and turn ideas into working products.</strong></p>

    <div class="badge-group">
      <a href="https://github.com/divyanshurawat7"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
      <a href="https://www.linkedin.com/in/divyanshurawat07/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
    </div>

    <div class="view-count">
      <img src="https://komarev.com/ghpvc/?username=divyanshurawat7&style=for-the-badge&color=blueviolet" alt="Profile views" />
    </div>
  </div>

  <!-- ABOUT -->
  <h2>🧠 About Me</h2>
  <p>I'm <strong>Divyanshu Rawat</strong>, a developer focused on building at the intersection of <strong>Artificial Intelligence, Machine Learning, Data Analytics, and Full-Stack Development</strong>.</p>
  <p>I enjoy taking a problem from <strong>raw data → analysis → intelligence → product</strong>.</p>
  <p>Currently, my work revolves around:</p>
  <ul style="margin-left:1.5rem; color:#d1d9e6;">
    <li>🤖 Building <strong>AI-powered applications</strong> using LLM APIs</li>
    <li>🧠 Developing <strong>Machine Learning models</strong> with Python</li>
    <li>📊 Creating <strong>interactive data analytics dashboards</strong></li>
    <li>💻 Building modern <strong>full-stack web applications</strong></li>
    <li>🔌 Integrating APIs, authentication, voice interfaces &amp; AI systems</li>
    <li>📈 Turning complex datasets into <strong>clear, actionable insights</strong></li>
  </ul>
  <blockquote style="border-left:4px solid #f0883e; padding-left:1.2rem; color:#b1bac4; font-style:italic; margin:0.8rem 0;">
    <strong>My goal:</strong> Build technology that is not only technically impressive, but actually useful.
  </blockquote>

  <hr />

  <!-- FEATURED PROJECTS -->
  <h2>🚀 Featured Projects</h2>

  <!-- FLAVORAX -->
  <div class="project-card">
    <div class="project-title"><i class="fas fa-utensils"></i> FlavoraX</div>
    <div class="project-sub"><strong>AI-Powered Recipe Generator &amp; Cooking Assistant</strong></div>
    <div class="project-desc">An intelligent cooking platform that combines <strong>LLM-powered recipe generation, multilingual voice interaction, food imagery, authentication, and conversational AI</strong>.</div>
    <ul class="highlight-list">
      <li>🤖 Groq LLM API</li><li>🎙️ Voice I/O (English+Hindi)</li><li>💬 AI assistant</li>
      <li>🖼️ Pexels API</li><li>🔐 Google OAuth</li><li>⚡ Flask</li>
    </ul>
    <div>
      <span class="stack-tag">Python</span><span class="stack-tag">Flask</span><span class="stack-tag">Groq API</span>
      <span class="stack-tag">Pexels API</span><span class="stack-tag">Google OAuth</span><span class="stack-tag">JavaScript</span>
    </div>
    <a href="https://github.com/divyanshurawat7/FlavoraX" class="repo-link"><i class="fab fa-github"></i> View Repository →</a>
  </div>

  <!-- AGRICULTURAL -->
  <div class="project-card">
    <div class="project-title"><i class="fas fa-seedling"></i> Agricultural Production Analysis</div>
    <div class="project-sub"><strong>Data Analysis + Machine Learning</strong></div>
    <div class="project-desc">A complete data science project analyzing Indian agricultural production and applying ML for crop production prediction.</div>
    <ul class="highlight-list">
      <li>🧹 Data cleaning</li><li>📊 EDA</li><li>🌱 Crop analysis</li>
      <li>🗺️ State/district</li><li>🔥 Correlation</li><li>🤖 Linear Regression</li>
    </ul>
    <div>
      <span class="stack-tag">Python</span><span class="stack-tag">Pandas</span><span class="stack-tag">NumPy</span>
      <span class="stack-tag">Matplotlib</span><span class="stack-tag">Seaborn</span><span class="stack-tag">Scikit-learn</span>
    </div>
    <a href="https://github.com/divyanshurawat7/Agricultural-Production-Analysis" class="repo-link"><i class="fab fa-github"></i> View Repository →</a>
  </div>

  <!-- AIR TRAFFIC -->
  <div class="project-card">
    <div class="project-title"><i class="fas fa-plane"></i> Air Traffic Passenger Analysis</div>
    <div class="project-sub"><strong>Power BI Analytics Dashboard</strong></div>
    <div class="project-desc">Interactive business intelligence dashboard designed to explore historical air passenger traffic across airlines, regions and countries.</div>
    <ul class="highlight-list">
      <li>🧹 Power Query</li><li>📊 Power BI</li><li>🧮 DAX KPIs</li>
      <li>🌍 Geographic analysis</li><li>✈️ Airline comparison</li><li>🔎 Drill-down</li>
    </ul>
    <div><span class="stack-tag">Power BI</span><span class="stack-tag">Power Query</span><span class="stack-tag">DAX</span><span class="stack-tag">Data Visualization</span></div>
    <a href="https://github.com/divyanshurawat7/Air-Traffic-Passenger-Analysis-Dashboard" class="repo-link"><i class="fab fa-github"></i> View Repository →</a>
  </div>

  <!-- MOVIE DASHBOARD -->
  <div class="project-card">
    <div class="project-title"><i class="fas fa-film"></i> Movie Analytics Dashboard</div>
    <div class="project-sub"><strong>IMDb Data × Power BI</strong></div>
    <div class="project-desc">Multi-page analytics dashboard exploring movie ratings, revenue, budgets, genres, languages and countries.</div>
    <ul class="highlight-list">
      <li>💰 Revenue &amp; budget</li><li>⭐ IMDb rating</li><li>🎭 Genre performance</li>
      <li>🌍 Country &amp; language</li><li>📅 Release filtering</li><li>📊 DAX KPIs</li>
    </ul>
    <div><span class="stack-tag">Power BI</span><span class="stack-tag">Power Query</span><span class="stack-tag">DAX</span><span class="stack-tag">Business Intelligence</span></div>
    <div style="margin:0.4rem 0; color:#b1bac4; font-size:0.9rem;"><strong>Key Metrics</strong> <span style="background:#21262d; padding:0.1rem 0.7rem; border-radius:20px;">$2.92B</span> — Highest Revenue &nbsp;|&nbsp; <span style="background:#21262d; padding:0.1rem 0.7rem; border-radius:20px;">6.46</span> — Avg IMDb Rating</div>
    <a href="https://github.com/divyanshurawat7/Movie-Analytics-Dashboard" class="repo-link"><i class="fab fa-github"></i> View Repository →</a>
  </div>

  <!-- PORTFOLIO -->
  <div class="project-card">
    <div class="project-title"><i class="fas fa-code"></i> Developer Portfolio</div>
    <div class="project-sub"><strong>Next.js × TypeScript × Tailwind</strong></div>
    <div class="project-desc">My personal developer portfolio showcasing projects, skills, experience and technical work.</div>
    <ul class="highlight-list">
      <li>⚡ Next.js</li><li>🧩 TypeScript</li><li>🎨 Tailwind CSS</li>
      <li>🚀 Netlify</li><li>🔄 Continuous iteration</li>
    </ul>
    <div><span class="stack-tag">Next.js</span><span class="stack-tag">TypeScript</span><span class="stack-tag">Tailwind CSS</span><span class="stack-tag">Netlify</span></div>
    <a href="https://github.com/divyanshurawat7/divyanshu_portfolio" class="repo-link"><i class="fab fa-github"></i> View Repository →</a>
  </div>

  <hr />

  <!-- TECH ARSENAL -->
  <h2>🛠️ Tech Arsenal</h2>

  <h3>👨‍💻 Languages</h3>
  <div class="tech-group">
    <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
    <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
    <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
    <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
    <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  </div>

  <h3>🤖 AI / Machine Learning</h3>
  <div class="tech-group">
    <img src="https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" alt="scikit-learn" />
    <img src="https://img.shields.io/badge/Groq_API-FF6B35?style=for-the-badge&logoColor=white" alt="Groq API" />
  </div>

  <h3>📊 Data Science</h3>
  <div class="tech-group">
    <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas" />
    <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy" />
    <img src="https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge" alt="Matplotlib" />
    <img src="https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge" alt="Seaborn" />
    <img src="https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI" />
  </div>

  <h3>💻 Development</h3>
  <div class="tech-group">
    <img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white" alt="Flask" />
    <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white" alt="Next.js" />
    <img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind CSS" />
  </div>

  <h3>⚙️ Tools</h3>
  <div class="tech-group">
    <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git" />
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
    <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter" />
    <img src="https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white" alt="VS Code" />
    <img src="https://img.shields.io/badge/Netlify-00C7B7?style=for-the-badge&logo=netlify&logoColor=white" alt="Netlify" />
  </div>

  <hr />

  <!-- WHAT I BUILD -->
  <h2>🧩 What I Build</h2>
  <div class="build-grid">
    <div class="build-col"><h4>🤖 AI &amp; ML</h4><ul><li>LLM Applications</li><li>AI Assistants</li><li>Machine Learning</li><li>Voice AI</li><li>Predictive Models</li></ul></div>
    <div class="build-col"><h4>📊 Data Analytics</h4><ul><li>Exploratory Data Analysis</li><li>Data Visualization</li><li>Power BI Dashboards</li><li>Business Intelligence</li><li>DAX &amp; Power Query</li></ul></div>
    <div class="build-col"><h4>💻 Full Stack</h4><ul><li>Flask</li><li>Next.js</li><li>TypeScript</li><li>REST APIs</li><li>OAuth Integration</li></ul></div>
  </div>

  <hr />

  <!-- GITHUB STATS -->
  <h2>📈 GitHub Analytics</h2>
  <div align="center" class="stats-grid">
    <img src="https://github-readme-stats.vercel.app/api?username=divyanshurawat7&show_icons=true&theme=tokyonight&hide_border=true&rank_icon=github" alt="GitHub Stats" />
    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=divyanshurawat7&layout=compact&theme=tokyonight&hide_border=true" alt="Top Languages" />
    <img src="https://github-readme-streak-stats-eight.vercel.app?user=divyanshurawat7&theme=tokyonight&hide_border=true" alt="GitHub Streak" />
  </div>

  <hr />

  <!-- CURRENT DIRECTION -->
  <h2>🎯 Current Direction</h2>
  <p>I'm currently focused on becoming stronger across the complete <strong>AI application development lifecycle</strong>:</p>
  <div class="code-flow">
Data
  ↓
Analysis
  ↓
Machine Learning
  ↓
LLMs / AI
  ↓
Backend APIs
  ↓
Frontend
  ↓
Production Application
  </div>
  <p>The long-term goal is to build <strong>production-ready AI systems</strong> that combine strong engineering with practical machine learning and data-driven decision making.</p>

  <hr />

  <!-- LEARNING -->
  <h2>📚 Learning &amp; Growth</h2>
  <p>Currently deepening my skills in:</p>
  <ul style="margin-left:1.5rem; color:#d1d9e6;">
    <li>🧠 Machine Learning &amp; Model Evaluation</li>
    <li>🤖 Generative AI &amp; LLM Applications</li>
    <li>📊 Advanced Data Analytics</li>
    <li>⚡ Full-Stack Application Architecture</li>
    <li>🔗 API &amp; AI Integration</li>
    <li>🚀 Production-oriented development</li>
  </ul>

  <hr />

  <!-- CONNECT -->
  <h2>🌐 Let's Connect</h2>
  <div align="center">
    <div class="connect-links">
      <a href="https://github.com/divyanshurawat7"><img src="https://img.shields.io/badge/GitHub-divyanshurawat7-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
      <a href="https://www.linkedin.com/in/divyanshurawat07/"><img src="https://img.shields.io/badge/LinkedIn-Divyanshu_Rawat-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
    </div>
    <p style="color:#b1bac4; margin-top:0.4rem;"><strong>⭐ If you find something interesting, feel free to explore the repositories!</strong></p>
  </div>

  <!-- FOOTER -->
  <div align="center" style="margin-top:2.5rem;">
    <div class="quote"><strong>"Build. Analyze. Learn. Repeat."</strong></div>
    <div class="footer-wave">
      <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=100&section=footer" alt="footer wave" style="width:100%; max-width:600px; border-radius:0 0 30px 30px;" />
    </div>
  </div>

</div>
<!-- end container -->
</body>
</html>
