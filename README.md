<!doctype html>
<html lang="tr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Umut Pasha | CV</title>
  <meta name="description" content="Umut Pasha - CV & Portfolyo" />

  <style>
    :root{
      --bg:#0b1020;
      --panel: rgba(255,255,255,.06);
      --panel2: rgba(255,255,255,.09);
      --text:#e8ecff;
      --muted: rgba(232,236,255,.7);
      --line: rgba(232,236,255,.18);
      --accent:#7c5cff;
      --accent2:#22d3ee;
      --shadow: 0 14px 40px rgba(0,0,0,.35);
      --radius: 18px;
    }

    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, "Helvetica Neue", Arial;
      color:var(--text);
      background:
        radial-gradient(1200px 700px at 20% 10%, rgba(124,92,255,.25), transparent 60%),
        radial-gradient(900px 600px at 80% 25%, rgba(34,211,238,.18), transparent 55%),
        radial-gradient(900px 600px at 60% 90%, rgba(124,92,255,.12), transparent 55%),
        var(--bg);
      overflow-x:hidden;
    }

    .container{max-width:1100px;margin:0 auto;padding:28px 18px 70px}
    a{color:inherit;text-decoration:none}
    .topbar{
      display:flex;align-items:center;justify-content:space-between;
      padding:14px 16px;border:1px solid var(--line);
      border-radius:999px;background:rgba(255,255,255,.04);
      backdrop-filter: blur(10px);
      position:sticky;top:14px;z-index:10;
    }
    .brand{display:flex;gap:10px;align-items:center}
    .dot{
      width:12px;height:12px;border-radius:99px;
      background:linear-gradient(135deg,var(--accent),var(--accent2));
      box-shadow:0 0 24px rgba(124,92,255,.6);
    }
    .nav{display:flex;gap:14px;flex-wrap:wrap;justify-content:flex-end}
    .nav a{
      padding:8px 10px;border-radius:999px;color:var(--muted);
      transition:.2s ease;
    }
    .nav a:hover{background:rgba(255,255,255,.06);color:var(--text)}
    .hero{
      margin-top:22px;
      display:grid;grid-template-columns: 1.2fr .8fr;gap:18px;
      align-items:stretch;
    }
    @media (max-width:900px){ .hero{grid-template-columns:1fr} }

    .card{
      border:1px solid var(--line);
      background:linear-gradient(180deg, rgba(255,255,255,.06), rgba(255,255,255,.03));
      border-radius:var(--radius);
      box-shadow:var(--shadow);
      backdrop-filter: blur(10px);
    }
    .hero-main{padding:26px 22px;position:relative;overflow:hidden}
    .hero-main:before{
      content:"";position:absolute;inset:-120px -180px auto auto;
      width:380px;height:380px;border-radius:50%;
      background:radial-gradient(circle at 30% 30%, rgba(34,211,238,.28), transparent 55%);
      transform:rotate(18deg);
    }
    .kicker{color:var(--muted);letter-spacing:.12em;text-transform:uppercase;font-size:12px}
    h1{margin:10px 0 8px;font-size:44px;line-height:1.08}
    .title{
      font-size:16px;color:var(--muted);line-height:1.6;max-width:62ch;
      margin-bottom:16px;
    }
    .badges{display:flex;gap:10px;flex-wrap:wrap;margin:10px 0 18px}
    .badge{
      font-size:12px;color:var(--text);
      border:1px solid var(--line);
      padding:8px 10px;border-radius:999px;
      background:rgba(255,255,255,.04);
    }
    .cta{display:flex;gap:10px;flex-wrap:wrap}
    .btn{
      display:inline-flex;gap:8px;align-items:center;
      padding:11px 14px;border-radius:12px;
      border:1px solid var(--line);
      background:rgba(255,255,255,.04);
      color:var(--text);
      transition:.2s ease;
    }
    .btn:hover{transform:translateY(-2px);background:rgba(255,255,255,.08)}
    .btn.primary{
      border-color: transparent;
      background:linear-gradient(135deg,var(--accent),var(--accent2));
      color:#071022;
      font-weight:700;
    }

    .hero-side{padding:20px 18px;display:flex;flex-direction:column;gap:12px}
    .mini{
      padding:14px 14px;border-radius:16px;border:1px solid var(--line);
      background:rgba(255,255,255,.04);
    }
    .mini h3{margin:0 0 6px;font-size:14px;color:var(--muted);font-weight:600}
    .mini p{margin:0;font-size:14px;line-height:1.6}

    .section{margin-top:22px}
    .section h2{
      margin:0 0 10px;font-size:20px;letter-spacing:.02em;
    }
    .grid2{display:grid;grid-template-columns:1fr 1fr;gap:14px}
    @media (max-width:900px){ .grid2{grid-template-columns:1fr} }

    /* Timeline */
    .timeline{
      position:relative;padding:10px 0 0 0;
    }
    .timeline:before{
      content:"";position:absolute;left:20px;top:0;bottom:0;width:2px;
      background:linear-gradient(180deg, rgba(124,92,255,.7), rgba(34,211,238,.25));
      opacity:.9;
    }
    .t-item{
      position:relative;
      margin-left:58px;
      padding:14px 16px;
      border-radius:16px;
      border:1px solid var(--line);
      background:rgba(255,255,255,.04);
      transition:.2s ease;
    }
    .t-item:hover{transform:translateY(-2px);background:rgba(255,255,255,.07)}
    .t-item + .t-item{margin-top:12px}
    .t-dot{
      position:absolute;left:-44px;top:18px;
      width:14px;height:14px;border-radius:999px;
      background:linear-gradient(135deg,var(--accent),var(--accent2));
      box-shadow:0 0 18px rgba(124,92,255,.55);
    }
    .t-connector{
      position:absolute;left:-30px;top:25px;height:2px;width:18px;
      background:rgba(232,236,255,.25);
    }
    .t-title{margin:0;font-weight:700}
    .t-meta{margin:6px 0 0;color:var(--muted);font-size:13px}
    .t-desc{margin:10px 0 0;line-height:1.65;color:rgba(232,236,255,.85)}

    /* Skills */
    .chips{display:flex;flex-wrap:wrap;gap:10px}
    .chip{
      padding:10px 12px;border-radius:999px;
      border:1px solid var(--line);
      background:rgba(255,255,255,.04);
      font-size:13px;color:rgba(232,236,255,.9);
      transition:.2s ease;
    }
    .chip:hover{transform:translateY(-2px);background:rgba(255,255,255,.07)}
    footer{margin-top:30px;color:var(--muted);font-size:13px;text-align:center}

    /* Reveal animation */
    .reveal{opacity:0;transform: translateY(14px);transition: .65s cubic-bezier(.2,.8,.2,1);}
    .reveal.on{opacity:1;transform:none;}

    /* Small nice selection */
    ::selection{background:rgba(124,92,255,.35)}
  </style>
</head>

<body>
  <div class="container">

    <header class="topbar card">
      <div class="brand">
        <span class="dot"></span>
        <strong>Umut Pasha</strong>
      </div>
      <nav class="nav">
        <a href="#about">Hakkımda</a>
        <a href="#edu">Eğitim</a>
        <a href="#exp">Projeler</a>
        <a href="#skills">Yetenekler</a>
        <a href="#contact">İletişim</a>
      </nav>
    </header>

    <section class="hero">
      <div class="card hero-main reveal">
        <div class="kicker">CV • Portfolyo</div>
        <h1>Umuthan “Umut Pasha” Yalçınkaya</h1>
        <div class="title">
          Kontrol & Otomasyon • Robotik • Gömülü Sistemler • Yapay Zeka / Veri Analizi
          <br/>Teknofest / yarışma projeleri, ekip çalışması, hızlı prototipleme.
        </div>
        <div class="badges">
          <span class="badge">İstanbul, TR</span>
          <span class="badge">Öğrenci • Asistan</span>
          <span class="badge">Open to: Proje / Staj</span>
        </div>
        <div class="cta">
          <a class="btn primary" href="#contact">İletişime Geç</a>
          <a class="btn" href="https://github.com/USERNAME" target="_blank" rel="noreferrer">GitHub</a>
          <a class="btn" href="assets/cv.pdf" target="_blank" rel="noreferrer">CV PDF</a>
        </div>
      </div>

      <aside class="card hero-side reveal">
        <div class="mini">
          <h3>Öne Çıkan</h3>
          <p>Robotik prototipler • Sensör entegrasyonu • ESP32/Arduino • Takım liderliği</p>
        </div>
        <div class="mini">
          <h3>İletişim</h3>
          <p>
            Mail: <a href="mailto:mail@ornek.com">mail@ornek.com</a><br/>
            LinkedIn: <a href="https://linkedin.com/in/USERNAME" target="_blank" rel="noreferrer">@USERNAME</a>
          </p>
        </div>
        <div class="mini">
          <h3>Not</h3>
          <p>Bu site GitHub Pages için tek dosya template. Bilgilerini at, içeriği tamamen sana göre doldurayım.</p>
        </div>
      </aside>
    </section>

    <section id="about" class="section card reveal" style="padding:18px 18px;">
      <h2>Hakkımda</h2>
      <p style="margin:0;line-height:1.75;color:rgba(232,236,255,.88)">
        Buraya kısa bir “kimsin + ne yapıyorsun + ne arıyorsun” paragrafı gelecek.
        (Sen verince ben düzgün, profesyonel, etkili şekilde yazıp yerleştiririm.)
      </p>
    </section>

    <section id="edu" class="section card reveal" style="padding:18px 18px;">
      <h2>Eğitim</h2>
      <div class="timeline">
        <div class="t-item">
          <span class="t-dot"></span><span class="t-connector"></span>
          <p class="t-title">Marmara Üniversitesi — Kontrol ve Otomasyon Teknolojisi</p>
          <p class="t-meta">2024 – Devam • İstanbul</p>
          <p class="t-desc">Dersler / odak alanları / notlar (ör. kontrol sistemleri, sayısal devreler, gömülü sistemler).</p>
        </div>
        <div class="t-item">
          <span class="t-dot"></span><span class="t-connector"></span>
          <p class="t-title">Lise / Diğer Okul</p>
          <p class="t-meta">Yıl Aralığı • Şehir</p>
          <p class="t-desc">Kısa açıklama (kulüp, proje, başarı).</p>
        </div>
      </div>
    </section>

    <section id="exp" class="section grid2">
      <div class="card reveal" style="padding:18px 18px;">
        <h2>Projeler</h2>
        <div class="timeline">
          <div class="t-item">
            <span class="t-dot"></span><span class="t-connector"></span>
            <p class="t-title">Proje Adı — Kısa Rol</p>
            <p class="t-meta">Teknolojiler: ESP32, Python, vs.</p>
            <p class="t-desc">2-3 madde: ne yaptın, sonuç, metrik/çıktı (varsa).</p>
          </div>
          <div class="t-item">
            <span class="t-dot"></span><span class="t-connector"></span>
            <p class="t-title">Proje Adı 2</p>
            <p class="t-meta">Teknolojiler: …</p>
            <p class="t-desc">Kısa özet.</p>
          </div>
        </div>
      </div>

      <div class="card reveal" style="padding:18px 18px;">
        <h2>Başarılar / Yarışmalar</h2>
        <div class="timeline">
          <div class="t-item">
            <span class="t-dot"></span><span class="t-connector"></span>
            <p class="t-title">Teknofest — Derece</p>
            <p class="t-meta">Yıl • Kategori</p>
            <p class="t-desc">Takım/rol ve kısa açıklama.</p>
          </div>
          <div class="t-item">
            <span class="t-dot"></span><span class="t-connector"></span>
            <p class="t-title">TÜBİTAK / Hackathon / MEB Robot</p>
            <p class="t-meta">Yıl • Sonuç</p>
            <p class="t-desc">Kısa açıklama.</p>
          </div>
        </div>
      </div>
    </section>

    <section id="skills" class="section card reveal" style="padding:18px 18px;">
      <h2>Yetenekler</h2>
      <div class="chips">
        <span class="chip">C / C++</span>
        <span class="chip">Python</span>
        <span class="chip">Arduino</span>
        <span class="chip">ESP32</span>
        <span class="chip">Sensör Entegrasyonu</span>
        <span class="chip">Kontrol Sistemleri</span>
        <span class="chip">Veri Analizi</span>
        <span class="chip">CAD / Mekanik Tasarım</span>
      </div>
    </section>

    <section id="contact" class="section card reveal" style="padding:18px 18px;">
      <h2>İletişim</h2>
      <p style="margin:0;color:rgba(232,236,255,.88);line-height:1.75">
        Mail: <a href="mailto:mail@ornek.com">mail@ornek.com</a> •
        LinkedIn: <a href="https://linkedin.com/in/USERNAME" target="_blank" rel="noreferrer">@USERNAME</a> •
        GitHub: <a href="https://github.com/USERNAME" target="_blank" rel="noreferrer">@USERNAME</a>
      </p>
    </section>

    <footer>
      © <span id="year"></span> Umut Pasha • GitHub Pages üzerinde yayınlanır.
    </footer>
  </div>

  <script>
    // Smooth scroll
    document.querySelectorAll('a[href^="#"]').forEach(a=>{
      a.addEventListener('click', (e)=>{
        const id = a.getAttribute('href');
        const el = document.querySelector(id);
        if(!el) return;
        e.preventDefault();
        el.scrollIntoView({behavior:'smooth', block:'start'});
      });
    });

    // Reveal on scroll
    const obs = new IntersectionObserver((entries)=>{
      entries.forEach(en=>{
        if(en.isIntersecting) en.target.classList.add('on');
      });
    }, {threshold:.12});
    document.querySelectorAll('.reveal').forEach(el=>obs.observe(el));

    // Year
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
