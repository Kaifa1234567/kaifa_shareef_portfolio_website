# KAIFA SHAREEF - PERSONAL PORTFOLIO DASHBOARD
# ==========================================

name = "Kaifa Shareef"
degree = "BS Mathematics"
university = "Bahauddin Zakariya University (BZU), Multan"
department = "CASPAM"
location = "Multan, Pakistan"
cgpa = "3.30"
academic_status = "6 semesters completed (latest shared update)"

linkedin = "https://www.linkedin.com/in/kaifa-shareef-b2ba92436/"
github = "https://github.com/Kaifa1234567"

tagline = (
    "Mathematics Student | Python | Machine Learning | Data Analysis"
)

about = (
    "I am a BS Mathematics student at Bahauddin Zakariya University, "
    "Multan. I am interested in Python programming, data analysis, "
    "machine learning, mathematical modelling and web development. "
    "My goal is to apply mathematical and computational thinking "
    "to practical, real-world problems."
)

skills = [
    "Mathematics",
    "Python Programming",
    "Machine Learning Fundamentals",
    "Data Analysis",
    "HTML",
    "CSS",
    "JavaScript Fundamentals",
    "Maple",
    "Problem Solving"
]

projects = [
    {
        "title": "Stockout Risk Prediction",
        "category": "Machine Learning",
        "status": "Course Project",
        "description": (
            "Predicting inventory stockout risk to help identify "
            "products that may become unavailable. Industry context: "
            "PND (Pak National Distributors)."
        ),
        "tools": "Python, Pandas, Scikit-learn"
    },
    {
        "title": "Expiry / Waste Risk Prediction",
        "category": "Machine Learning",
        "status": "Project Direction",
        "description": (
            "A project concept for identifying inventory at risk "
            "of expiry or waste and supporting better stock decisions."
        ),
        "tools": "Python, Data Analysis, Classification"
    },
    {
        "title": "Personal Portfolio Dashboard",
        "category": "Web Development",
        "status": "Portfolio Project",
        "description": (
            "A responsive dashboard for presenting education, "
            "technical skills, projects and professional profiles."
        ),
        "tools": "Python, HTML, CSS"
    },
    {
        "title": "Library Management System",
        "category": "Programming",
        "status": "Learning Project",
        "description": (
            "A programming project concept for organizing books, "
            "library records and borrowing information."
        ),
        "tools": "Programming Fundamentals"
    }
]

def esc(value):
    return html.escape(str(value), quote=True)

skill_html = "".join(
    f'<span class="skill">{esc(skill)}</span>'
    for skill in skills
)

project_html = ""

for p in projects:
    project_html += f"""
    <article class="project">
      <span class="tag">{esc(p["category"])}</span>
      <h3>{esc(p["title"])}</h3>
      <p>{esc(p["description"])}</p>
      <div class="tools">Tools: {esc(p["tools"])}</div>
      <div class="status">{esc(p["status"])}</div>
    </article>
    """

# ==========================================
# WEBSITE DESIGN
# ==========================================

page = r"""
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Kaifa Shareef | Portfolio Dashboard</title>

<style>
:root {
  --navy: #171b34;
  --purple: #7357e8;
  --bg: #f5f6fc;
  --white: #ffffff;
  --text: #252b43;
  --muted: #747d95;
  --border: #e7e9f2;
}
* { box-sizing: border-box; }
html { scroll-behavior: smooth; }
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: var(--bg);
  color: var(--text);
}
.layout { display: flex; min-height: 100vh; }
.sidebar {
  width: 240px;
  flex-shrink: 0;
  background: var(--navy);
  color: white;
  padding: 28px 20px;
}
.brand { font-size: 24px; font-weight: 800; margin-bottom: 35px; }
.brand span { color: #b8a8ff; }
.menu-title { color: #aeb4cc; font-size: 11px; letter-spacing: 2px; }
nav { margin-top: 15px; }
nav a {
  display: block;
  padding: 13px;
  margin: 5px 0;
  border-radius: 9px;
  color: #e4e6f1;
  text-decoration: none;
}
nav a:hover { background: #353252; }
main { flex: 1; min-width: 0; padding: 30px; }
.topbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 15px;
  margin-bottom: 25px;
}
.topbar h2 { margin: 0 0 6px; }
.muted { color: var(--muted); font-size: 13px; line-height: 1.8; }
.pill {
  background: white;
  border: 1px solid var(--border);
  padding: 10px 13px;
  border-radius: 10px;
  font-size: 12px;
}
.hero {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 20px;
  flex-wrap: wrap;
  padding: 34px;
  border-radius: 20px;
  color: white;
  background: linear-gradient(120deg, #222344, #7357e8);
}
.overline {
  color: #d7d0ff;
  font-size: 12px;
  letter-spacing: 2px;
  text-transform: uppercase;
}
.hero h1 { font-size: clamp(29px, 4vw, 43px); margin: 14px 0; }
.hero p { line-height: 1.8; color: #e7e3ff; }
.avatar {
  width: 100px;
  height: 100px;
  display: grid;
  place-items: center;
  border-radius: 28px;
  border: 1px solid #ffffff65;
  background: #ffffff20;
  font-size: 36px;
  font-weight: 800;
}
.btn {
  display: inline-block;
  padding: 12px 16px;
  margin: 8px 8px 0 0;
  border-radius: 9px;
  font-size: 13px;
  font-weight: bold;
  text-decoration: none;
}
.btn-light { background: white; color: #4935ad; }
.btn-outline { border: 1px solid #ddd5ff; color: white; }
.section { margin-top: 28px; scroll-margin-top: 20px; }
.section-title { font-size: 20px; margin: 0 0 16px; }
.stats {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 15px;
}
.card, .project {
  background: var(--white);
  border: 1px solid var(--border);
  border-radius: 15px;
  padding: 22px;
}
.stat-label { color: var(--muted); font-size: 13px; }
.stat-value { font-size: 24px; font-weight: 800; margin: 12px 0 5px; }
.two-col {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 18px;
}
.info {
  padding: 13px 0;
  border-bottom: 1px solid var(--border);
  line-height: 1.7;
  overflow-wrap: anywhere;
}
.info:last-child { border-bottom: 0; }
.info-label { color: var(--muted); font-size: 12px; }
.info-value { font-size: 14px; font-weight: 600; }
.skills { display: flex; flex-wrap: wrap; gap: 10px; }
.skill, .tag {
  display: inline-block;
  background: #f0edff;
  color: #5541bb;
  border-radius: 8px;
  padding: 9px 11px;
  font-size: 12px;
}
.projects {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 16px;
}
.project h3 { margin: 14px 0 8px; }
.project p { color: var(--muted); font-size: 13px; line-height: 1.8; }
.tools {
  border-top: 1px solid var(--border);
  padding-top: 12px;
  font-size: 12px;
  overflow-wrap: anywhere;
}
.status { margin-top: 12px; color: var(--muted); font-size: 11px; }
.links { display: flex; flex-wrap: wrap; gap: 10px; }
.links a {
  color: var(--purple);
  text-decoration: none;
  border: 1px solid var(--border);
  border-radius: 9px;
  padding: 12px 14px;
  font-size: 13px;
  font-weight: bold;
}
.links a:hover { background: #f0edff; }
footer { text-align: center; padding: 30px 0 5px; color: var(--muted); font-size: 12px; }
@media(max-width: 850px) {
  .layout { display: block; }
  .sidebar { width: 100%; padding: 18px; }
  .brand { margin-bottom: 15px; }
  .menu-title { display: none; }
  nav { display: flex; flex-wrap: wrap; margin-top: 5px; }
  nav a { padding: 10px; font-size: 13px; }
  main { padding: 18px; }
}
@media(max-width: 600px) {
  .stats, .two-col, .projects { grid-template-columns: 1fr; }
  .hero { padding: 24px; }
  .pill { display: none; }
}
</style>
</head>

<body>
<div class="layout">

<aside class="sidebar">
  <div class="brand">Kaifa<span>.</span></div>
  <div class="menu-title">PORTFOLIO MENU</div>
  <nav>
    <a href="#home">⌂ Overview</a>
    <a href="#about">♙ About Me</a>
    <a href="#education">🎓 Education</a>
    <a href="#skills">⚙ Skills</a>
    <a href="#projects">▤ Projects</a>
    <a href="#contact">✉ Contact</a>
  </nav>
</aside>

<main>
<header class="topbar">
  <div>
    <h2>Portfolio Dashboard</h2>
    <div class="muted">My academic and technical journey</div>
  </div>
  <span class="pill">Mathematics • Technology</span>
</header>

<section class="hero" id="home">
  <div>
    <div class="overline">Welcome to my portfolio</div>
    <h1>Hi, I'm __NAME__</h1>
    <p>__TAGLINE__</p>
    <a class="btn btn-light" href="#projects">Explore Projects ↗</a>
    <a class="btn btn-outline" href="#contact">Connect With Me</a>
  </div>
  <div class="avatar">KS</div>
</section>

<section class="section">
  <h2 class="section-title">Dashboard Overview</h2>
  <div class="stats">
    <div class="card">
      <div class="stat-label">Degree</div>
      <div class="stat-value">BS Math</div>
      <div class="muted">Mathematics Student</div>
    </div>
    <div class="card">
      <div class="stat-label">Academic Progress</div>
      <div class="stat-value">6 Semesters</div>
      <div class="muted">At latest shared update</div>
    </div>
    <div class="card">
      <div class="stat-label">Featured Work</div>
      <div class="stat-value">04</div>
      <div class="muted">Projects and learning concepts</div>
    </div>
  </div>
</section>

<section class="section two-col" id="about">
  <div class="card">
    <h2 class="section-title">About Me</h2>
    <p class="muted">__ABOUT__</p>
    <div class="info">
      <div class="info-label">Location</div>
      <div class="info-value">__LOCATION__</div>
    </div>
    <div class="info">
      <div class="info-label">Main Interests</div>
      <div class="info-value">Mathematics, ML, Data Analysis</div>
    </div>
  </div>

  <div class="card" id="education">
    <h2 class="section-title">Education</h2>
    <div class="info">
      <div class="info-label">Degree</div>
      <div class="info-value">__DEGREE__</div>
    </div>
    <div class="info">
      <div class="info-label">University</div>
      <div class="info-value">__UNIVERSITY__</div>
    </div>
    <div class="info">
      <div class="info-label">Department</div>
      <div class="info-value">__DEPARTMENT__</div>
    </div>
    <div class="info">
      <div class="info-label">Academic Status</div>
      <div class="info-value">__STATUS__</div>
    </div>
    <div class="info">
      <div class="info-label">CGPA after Semester 6</div>
      <div class="info-value">__CGPA__</div>
    </div>
  </div>
</section>

<section class="section card" id="skills">
  <h2 class="section-title">Skills & Interests</h2>
  <div class="skills">__SKILLS__</div>
  <p class="muted">Skills listed reflect my learning areas and interests.</p>
</section>

<section class="section" id="projects">
  <h2 class="section-title">Projects & Learning Work</h2>
  <div class="projects">__PROJECTS__</div>
</section>

<section class="section card" id="contact">
  <h2 class="section-title">Professional Profiles</h2>
  <p class="muted">Connect with me for academic networking and project collaboration.</p>
  <div class="links">
    <a href="__LINKEDIN__" target="_blank" rel="noopener">My LinkedIn ↗</a>
    <a href="__GITHUB__" target="_blank" rel="noopener">My GitHub ↗</a>
  </div>
</section>

<footer>© 2026 __NAME__ | Personal Portfolio Dashboard</footer>
</main>
</div>
</body>
</html>
