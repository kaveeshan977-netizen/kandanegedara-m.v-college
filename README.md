<!DOCTYPE html>
<html lang="si">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Kandanegedara M.V. College | කඳානේගෙදර මහා විද්‍යාලය</title>
  <meta name="description" content="Kandanegedara M.V. College official website – academics, news, gallery, staff, contact." />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+Sinhala:wght@400;600;700&family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --primary:#0A4DA3; /* Royal blue */
      --primary-600:#083e83;
      --accent:#00B5D8; /* cyan */
      --bg:#F4F7FB;
      --text:#102233;
      --muted:#6b7a90;
      --card:#ffffff;
      --shadow:0 10px 25px rgba(0,0,0,.08);
      --radius:18px;
    }
    *{box-sizing:border-box}
    html,body{margin:0;padding:0;background:var(--bg);color:var(--text);font-family:"Inter","Noto Sans Sinhala",system-ui,-apple-system,Segoe UI,Roboto;}
    a{color:inherit;text-decoration:none}
    img{max-width:100%;display:block}
    .container{width:min(1120px,92%);margin:auto}
    /* NAV */
    .topbar{position:sticky;top:0;z-index:50;background:rgba(255,255,255,.7);backdrop-filter:saturate(1.4) blur(10px);border-bottom:1px solid #e9eef5}
    .nav{display:flex;align-items:center;justify-content:space-between;padding:.8rem 0}
    .brand{display:flex;align-items:center;gap:.8rem}
    .brand .logo{width:42px;height:42px;border-radius:12px;background:linear-gradient(135deg,var(--primary),#3c7ee7);display:grid;place-items:center;color:#fff;font-weight:800;box-shadow:var(--shadow)}
    .brand .titles{line-height:1}
    .brand .titles .en{font-weight:700}
    .brand .titles .si{font-size:.9rem;color:var(--muted)}
    .nav-links{display:flex;gap:1rem;align-items:center}
    .nav-links a{padding:.55rem .8rem;border-radius:12px}
    .nav-links a:hover{background:#edf3ff}
    .menu-btn{display:none;border:0;background:transparent;font-size:1.6rem}

    /* HERO */
    .hero{padding:clamp(2rem,6vw,4.5rem) 0;}
    .hero-card{background:linear-gradient(180deg,#ffffff, #f8fbff);border:1px solid #e8eef7;box-shadow:var(--shadow);border-radius:28px;display:grid;grid-template-columns:1.1fr .9fr;gap:2rem;padding:clamp(1.2rem,4vw,2.2rem)}
    .hero h1{font-size:clamp(1.6rem,3.4vw,2.6rem);margin:.4rem 0 0}
    .badge{display:inline-flex;gap:.5rem;align-items:center;background:#ecf3ff;color:var(--primary);border:1px solid #d8e6ff;padding:.4rem .7rem;border-radius:999px;font-weight:600;font-size:.85rem}
    .hero p{color:var(--muted);line-height:1.7}
    .cta{display:flex;gap:.8rem;flex-wrap:wrap;margin-top:1rem}
    .btn{display:inline-flex;align-items:center;gap:.5rem;padding:.7rem 1rem;border-radius:14px;border:1px solid #d9e3f1;font-weight:600}
    .btn.primary{background:var(--primary);border-color:var(--primary);color:#fff}
    .btn.primary:hover{background:var(--primary-600)}
    .stats{display:grid;grid-template-columns:repeat(3,1fr);gap:1rem;margin-top:1.2rem}
    .stat{background:var(--card);border:1px solid #e8eef7;border-radius:16px;padding:1rem;text-align:center}
    .stat .num{font-weight:800;font-size:1.4rem;color:var(--primary)}

    .hero-visual{position:relative}
    .hero-img{aspect-ratio:4/3;border-radius:22px;object-fit:cover;border:1px solid #e8eef7;box-shadow:var(--shadow)}
    .floating{position:absolute;right:-8px;bottom:-8px;background:#fff;border:1px solid #e8eef7;border-radius:16px;padding:.8rem;box-shadow:var(--shadow)}

    /* SECTIONS */
    section{padding:clamp(1.8rem,4vw,3rem) 0}
    .section-head{display:flex;justify-content:space-between;align-items:end;gap:1rem;margin-bottom:1rem}
    .section-head h2{margin:0;font-size:clamp(1.3rem,2.2vw,1.8rem)}
    .muted{color:var(--muted)}

    /* PROGRAMS */
    .grid-3{display:grid;grid-template-columns:repeat(3,1fr);gap:1rem}
    .card{background:var(--card);border:1px solid #e8eef7;border-radius:var(--radius);padding:1rem;box-shadow:var(--shadow)}

    /* NEWS */
    .news-list{display:grid;grid-template-columns:repeat(3,1fr);gap:1rem}
    .news{padding:1rem;background:#fff;border:1px solid #e8eef7;border-radius:16px;display:flex;gap:1rem}
    .news .date{min-width:64px;text-align:center;background:#f1f6ff;border:1px solid #dfe9ff;border-radius:12px;padding:.5rem}
    .news .date .d{font-weight:800;font-size:1.2rem;color:var(--primary)}
    .news img{width:96px;height:80px;object-fit:cover;border-radius:12px;border:1px solid #e8eef7}

    /* GALLERY */
    .gallery{display:grid;grid-template-columns:repeat(4,1fr);gap:.6rem}
    .gallery img{aspect-ratio:1/1;object-fit:cover;border-radius:14px;border:1px solid #e8eef7}

    /* STAFF */
    .staff{display:grid;grid-template-columns:repeat(4,1fr);gap:1rem}
    .person{background:#fff;border:1px solid #e8eef7;border-radius:16px;padding:1rem;text-align:center}
    .avatar{width:84px;height:84px;margin:auto;border-radius:50%;object-fit:cover;border:2px solid #e8eef7}
    .role{font-size:.9rem;color:var(--muted)}

    /* CONTACT */
    .contact{display:grid;grid-template-columns:1.2fr .8fr;gap:1rem}
    form{display:grid;gap:.7rem}
    input,textarea{padding:.8rem;border-radius:12px;border:1px solid #dbe3f2;background:#fff;font:inherit}
    textarea{min-height:120px;resize:vertical}

    .map{height:100%;min-height:260px;border-radius:16px;overflow:hidden;border:1px solid #e8eef7}
    .footer{padding:1.4rem 0;margin-top:1.4rem;border-top:1px solid #e8eef7;color:var(--muted)}
    .foot-grid{display:grid;grid-template-columns:1.2fr 1fr 1fr;gap:1rem}
    .foot-grid ul{list-style:none;padding:0;margin:0}
    .foot-grid li{margin:.4rem 0}

    /* RESPONSIVE */
    @media (max-width: 960px){
      .hero-card{grid-template-columns:1fr}
      .stats{grid-template-columns:repeat(3,1fr)}
      .news-list{grid-template-columns:repeat(2,1fr)}
      .staff{grid-template-columns:repeat(3,1fr)}
      .gallery{grid-template-columns:repeat(3,1fr)}
      .contact{grid-template-columns:1fr}
      .foot-grid{grid-template-columns:1fr 1fr}
    }
    @media (max-width: 640px){
      .nav-links{display:none}
      .menu-btn{display:block}
      .news-list{grid-template-columns:1fr}
      .staff{grid-template-columns:repeat(2,1fr)}
      .gallery{grid-template-columns:repeat(2,1fr)}
      .foot-grid{grid-template-columns:1fr}
    }
  </style>
</head>
<body>
  <!-- NAVBAR -->
  <div class="topbar">
    <div class="container nav">
      <div class="brand">
        <div class="logo" aria-hidden="true">KMV</div>
        <div class="titles">
          <div class="en">Kandanegedara M.V. College</div>
          <div class="si">කඳානේගෙදර මහා විද්‍යාලය</div>
        </div>
      </div>
      <nav class="nav-links" aria-label="Primary">
        <a href="#about">About</a>
        <a href="#programs">Academic</a>
        <a href="#news">News</a>
        <a href="#gallery">Gallery</a>
        <a href="#staff">Staff</a>
        <a href="#contact">Contact</a>
      </nav>
      <button class="menu-btn" aria-label="Open menu" onclick="toggleMenu()">☰</button>
    </div>
  </div>

  <!-- HERO -->
  <header class="hero">
    <div class="container hero-card">
      <div>
        <span class="badge">Official Website • නිල වෙබ් අඩවිය</span>
        <h1>Kandanegedara M.V. College<br><span class="muted" style="font-size:1rem">කඳානේගෙදර මහා විද්‍යාලය</span></h1>
        <p>
          Quality education for every child – discipline, compassion, and excellence.
          <br>සපිරුණු අනාගතයක් සඳහා පූර්ණාවයවී සෞදු අධ්‍යාපනයක්.
        </p>
        <div class="cta">
          <a class="btn primary" href="#contact">Apply / දරුවා ඇතුළත් කරන්න</a>
          <a class="btn" href="#news">Latest News</a>
        </div>
        <div class="stats">
          <div class="stat"><div class="num">1,200+</div><div>Students</div></div>
          <div class="stat"><div class="num">75+</div><div>Teachers</div></div>
          <div class="stat"><div class="num">1992</div><div>Established</div></div>
        </div>
      </div>
      <div class="hero-visual">
        <!-- Replace src with your own hero image in /images/hero.jpg -->
        <img class="hero-img" src="https://images.unsplash.com/photo-1529078155058-5d716f45d604?q=80&w=1200&auto=format&fit=crop" alt="School building and students" />
        <div class="floating">
          <strong>Upcoming:</strong> Annual Sports Meet • October 2025
        </div>
      </div>
    </div>
  </header>

  <!-- ABOUT -->
  <section id="about">
    <div class="container">
      <div class="section-head">
        <h2>About Us | අප ගැන</h2>
        <p class="muted">Location: Kandanegedara, Sri Lanka</p>
      </div>
      <div class="card" style="line-height:1.8">
        Kandanegedara M.V. College is a leading educational institution dedicated to holistic student development. 
        We offer classes from Grade 1 to Advanced Level with a focus on academics, sports, and aesthetic education.
        <br><br>
        කඳානේගෙදර මහා විද්‍යාලය, පළාතේ පිහිටා ඇති කැපී පෙනෙන පාසලකි. 
        ශ්‍රේණි 1 සිට උසස් පෙළ දක්වා අධ්‍යාපනය ලබා දෙන අතර, විද්‍යා, වාණිජ, කලා දැනුම සමඟ ක්‍රීඩා සහ අලංකාර අධ්‍යාපනය ද වර්ධනය කරයි.
      </div>
    </div>
  </section>

  <!-- PROGRAMS -->
  <section id="programs">
    <div class="container">
      <div class="section-head">
        <h2>Academic Programs | අධ්‍යාපන වැඩසටහන්</h2>
        <a class="btn" href="#">Download Prospectus (PDF)</a>
      </div>
      <div class="grid-3">
        <div class="card">
          <h3>Primary (Grade 1–5)</h3>
          <p class="muted">Foundational literacy, numeracy, and character building.</p>
          <ul>
            <li>English & Sinhala Medium</li>
            <li>STEAM Activities</li>
            <li>Clubs & Societies</li>
          </ul>
        </div>
        <div class="card">
          <h3>Junior Secondary (6–9)</h3>
          <p class="muted">Core subjects with exploratory learning.</p>
          <ul>
            <li>ICT Lab Sessions</li>
            <li>Sports & Aesthetics</li>
            <li>Student Counseling</li>
          </ul>
        </div>
        <div class="card">
          <h3>Senior Secondary (10–13)</h3>
          <p class="muted">O/L and A/L streams.</p>
          <ul>
            <li>Science • Commerce • Arts</li>
            <li>Career Guidance</li>
            <li>University Readiness</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <!-- NEWS & EVENTS -->
  <section id="news">
    <div class="container">
      <div class="section-head">
        <h2>News & Events | පුවත් හා ඉසව්</h2>
        <p class="muted">School notices, achievements, and upcoming events.</p>
      </div>
      <div class="news-list">
        <article class="news">
          <div class="date"><div class="d">25</div><div>AUG</div></div>
          <div>
            <h3>Grade 5 Scholarship Workshop</h3>
            <p class="muted">Parents and students are invited to the seminar at the main hall. Time: 9.00 AM</p>
          </div>
          <img src="https://images.unsplash.com/photo-1513258496099-48168024aec0?q=80&w=600&auto=format&fit=crop" alt="workshop" />
        </article>
        <article class="news">
          <div class="date"><div class="d">10</div><div>SEP</div></div>
          <div>
            <h3>ICT Lab Upgrade Completed</h3>
            <p class="muted">New computers and smart boards installed for enhanced learning.</p>
          </div>
          <img src="https://images.unsplash.com/photo-1519389950473-47ba0277781c?q=80&w=600&auto=format&fit=crop" alt="lab" />
        </article>
        <article class="news">
          <div class="date"><div class="d">05</div><div>OCT</div></div>
          <div>
            <h3>Annual Sports Meet 2025</h3>
            <p class="muted">All houses to participate – opening parade starts at 8.30 AM.</p>
          </div>
          <img src="https://images.unsplash.com/photo-1547347298-4074fc3086f0?q=80&w=600&auto=format&fit=crop" alt="sports" />
        </article>
      </div>
    </div>
  </section>

  <!-- GALLERY -->
  <section id="gallery">
    <div class="container">
      <div class="section-head">
        <h2>Gallery | පින්තූර ශාලාව</h2>
        <p class="muted">Highlights from school life.</p>
      </div>
      <div class="gallery">
        <img src="https://images.unsplash.com/photo-1509062522246-3755977927d7?q=80&w=600&auto=format&fit=crop" alt="Assembly" />
        <img src="https://images.unsplash.com/photo-1497633762265-9d179a990aa6?q=80&w=600&auto=format&fit=crop" alt="Library" />
        <img src="https://images.unsplash.com/photo-1517849845537-4d257902454a?q=80&w=600&auto=format&fit=crop" alt="Sports" />
        <img src="https://images.unsplash.com/photo-1476480862126-209bfaa8edc8?q=80&w=600&auto=format&fit=crop" alt="Science Lab" />
        <img src="https://images.unsplash.com/photo-1523580846011-d3a5bc25702b?q=80&w=600&auto=format&fit=crop" alt="Music" />
        <img src="https://images.unsplash.com/photo-1513258496099-48168024aec0?q=80&w=600&auto=format&fit=crop" alt="Workshop" />
        <img src="https://images.unsplash.com/photo-1522071820081-009f0129c71c?q=80&w=600&auto=format&fit=crop" alt="Classroom" />
        <img src="https://images.unsplash.com/photo-1510936111840-65e151ad71bb?q=80&w=600&auto=format&fit=crop" alt="Art" />
      </div>
    </div>
  </section>

  <!-- STAFF -->
  <section id="staff">
    <div class="container">
      <div class="section-head">
        <h2>Our Staff | අපගේ කාර්ය මණ්ඩලය</h2>
        <p class="muted">Dedicated leadership and experienced teachers.</p>
      </div>
      <div class="staff">
        <div class="person">
          <img class="avatar" src="https://images.unsplash.com/photo-1544005313-94ddf0286df2?q=80&w=400&auto=format&fit=crop" alt="Principal" />
          <h3>Mrs. S. Perera</h3>
          <div class="role">Principal</div>
        </div>
        <div class="person">
          <img class="avatar" src="https://images.unsplash.com/photo-1547425260-76bcadfb4f2c?q=80&w=400&auto=format&fit=crop" alt="Deputy Principal" />
          <h3>Mr. K. Herath</h3>
          <div class="role">Deputy Principal</div>
        </div>
        <div class="person">
          <img class="avatar" src="https://images.unsplash.com/photo-1548142813-c348350df52b?q=80&w=400&auto=format&fit=crop" alt="Section Head" />
          <h3>Ms. R. Fernando</h3>
          <div class="role">Head of Science</div>
        </div>
        <div class="person">
          <img class="avatar" src="https://images.unsplash.com/photo-1544005313-94ddf0286df2?q=80&w=400&auto=format&fit=crop" alt="Teacher" />
          <h3>Mr. I. Silva</h3>
          <div class="role">ICT Instructor</div>
        </div>
      </div>
    </div>
  </section>

  <!-- DOWNLOADS / LINKS -->
  <section id="downloads">
    <div class="container">
      <div class="section-head">
        <h2>Downloads | බාගත කිරීම්</h2>
        <p class="muted">Timetables, application forms, and notices.</p>
      </div>
      <div class="grid-3">
        <a class="card" href="#" download>
          <strong>School Timetable (PDF)</strong>
          <p class="muted">2025 – All Grades</p>
        </a>
        <a class="card" href="#" download>
          <strong>Admission Application</strong>
          <p class="muted">Download & submit to office</p>
        </a>
        <a class="card" href="#" download>
          <strong>Annual Report</strong>
          <p class="muted">Academic Year 2024/25</p>
        </a>
      </div>
    </div>
  </section>

  <!-- CONTACT -->
  <section id="contact">
    <div class="container">
      <div class="section-head">
        <h2>Contact Us | අප හා සම්බන්ධ වන්න</h2>
        <p class="muted">Call, email or send a message.</p>
      </div>
      <div class="contact">
        <form action="https://formspree.io/f/your-id" method="POST">
          <!-- TIP: Replace action with your Formspree ID to receive emails -->
          <input name="name" placeholder="ඔබගේ නම / Your Name" required />
          <input type="email" name="email" placeholder="Email" required />
          <textarea name="message" placeholder="ඔබගේ පණිවිඩය / Message" required></textarea>
          <button class="btn primary" type="submit">Send Message / පණිවිඩය යවන්න</button>
          <small class="muted">☎ Phone: 011-1234567 • ✉ Email: info@kandanegedara.lk</small>
        </form>
        <div class="map">
          <!-- Replace src with your Google Map embed link -->
          <iframe title="School map" src="https://maps.google.com/maps?q=Sri%20Lanka&t=&z=7&ie=UTF8&iwloc=&output=embed" width="100%" height="100%" frameborder="0" style="border:0" allowfullscreen></iframe>
        </div>
      </div>
    </div>
  </section>

  <footer class="footer">
    <div class="container foot-grid">
      <div>
        <div class="brand" style="margin-bottom:.6rem">
          <div class="logo">KMV</div>
          <div class="titles">
            <div class="en">Kandanegedara M.V. College</div>
            <div class="si">කඳානේගෙදර මහා විද්‍යාලය</div>
          </div>
        </div>
        <p class="muted">© <span id="year"></span> Kandanegedara M.V. College. All rights reserved.</p>
      </div>
      <div>
        <h4>Quick Links</h4>
        <ul>
          <li><a href="#about">About</a></li>
          <li><a href="#programs">Programs</a></li>
          <li><a href="#news">News</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </div>
      <div>
        <h4>Contact</h4>
        <ul>
          <li>Kandanegedara, Sri Lanka</li>
          <li>☎ 011-1234567</li>
          <li>✉ info@kandanegedara.lk</li>
        </ul>
      </div>
    </div>
  </footer>

  <script>
    // Mobile menu (very simple)
    function toggleMenu(){
      const links = document.querySelector('.nav-links');
      if(!links) return;
      links.style.display = (links.style.display === 'flex') ? 'none' : 'flex';
      links.style.flexDirection = 'column';
      links.style.gap = '0.4rem';
      links.style.background = '#fff';
      links.style.padding = '0.5rem';
      links.style.position = 'absolute';
      links.style.right = '1rem';
      links.style.top = '60px';
      links.style.border = '1px solid #e8eef7';
      links.style.borderRadius = '12px';
      links.style.boxShadow = 'var(--shadow)';
    }
    // Current year in footer
    document.getElementById('year').textContent = new Date().ge
