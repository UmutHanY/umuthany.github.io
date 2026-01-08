<!doctype html>
<html lang="tr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1,viewport-fit=cover" />
  <title>Umuthan Yalçınkaya (Umut Pasha) | CV</title>
  <meta name="description" content="Mobil öncelikli CV & Portfolyo — Umuthan Yalçınkaya (Umut Pasha)" />
  <style>
    :root{
      --bg:#0b1020;
      --panel:rgba(255,255,255,.06);
      --text:#e9edff;
      --muted:rgba(233,237,255,.72);
      --line:rgba(233,237,255,.16);
      --accent:#7c5cff;
      --accent2:#22d3ee;
      --radius:18px;
      --shadow:0 14px 40px rgba(0,0,0,.35);
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Arial;
      color:var(--text);
      background:
        radial-gradient(900px 600px at 25% 10%, rgba(124,92,255,.26), transparent 60%),
        radial-gradient(800px 550px at 80% 25%, rgba(34,211,238,.18), transparent 55%),
        radial-gradient(900px 650px at 55% 95%, rgba(124,92,255,.12), transparent 55%),
        var(--bg);
      overflow-x:hidden;
      -webkit-tap-highlight-color: transparent;
    }
    a{color:inherit;text-decoration:none}
    .wrap{max-width:980px;margin:0 auto;padding:16px 14px 60px}
    .topbar{
      position:sticky; top:12px; z-index:20;
      display:flex; align-items:center; justify-content:space-between;
      padding:12px 12px;
      border:1px solid var(--line);
      border-radius:999px;
      background:rgba(255,255,255,.04);
      backdrop-filter: blur(10px);
      box-shadow:0 10px 30px rgba(0,0,0,.25);
    }
    .brand{display:flex;align-items:center;gap:10px;min-width:0}
    .dot{
      width:12px;height:12px;border-radius:999px;
      background:linear-gradient(135deg,var(--accent),var(--accent2));
      box-shadow:0 0 20px rgba(124,92,255,.6);
      flex:0 0 auto;
    }
    .brand strong{font-size:14px;white-space:nowrap;overflow:hidden;text-overflow:ellipsis}
    .burger{
      width:42px;height:38px;border-radius:999px;
      border:1px solid var(--line);
      background:rgba(255,255,255,.04);
      display:grid; place-items:center;
      cursor:pointer;
      transition:.2s ease;
    }
    .burger:active{transform:scale(.98)}
    .burger span{
      display:block;width:18px;height:2px;background:rgba(233,237,255,.85);
      position:relative;border-radius:999px;
    }
    .burger span:before,.burger span:after{
      content:"";position:absolute;left:0;width:18px;height:2px;border-radius:999px;
      background:rgba(233,237,255,.85);
    }
    .burger span:before{top:-6px}
    .burger span:after{top:6px}

    .drawer{position:fixed; inset:0; z-index:50; display:none;}
    .drawer.on{display:block}
    .backdrop{position:absolute; inset:0; background:rgba(0,0,0,.55); backdrop-filter: blur(2px);}
    .card{
      border:1px solid var(--line);
      background:linear-gradient(180deg, rgba(255,255,255,.06), rgba(255,255,255,.03));
      border-radius:var(--radius);
      box-shadow:var(--shadow);
      backdrop-filter: blur(10px);
    }
    .sheet{
      position:absolute; right:10px; top:10px; left:10px;
      padding:14px;
      background:rgba(16,21,45,.88);
      transform: translateY(-6px);
      animation: pop .18s ease-out forwards;
    }
    @keyframes pop{to{transform:none}}
    .sheet h3{margin:6px 8px 10px;font-size:14px;color:var(--muted);font-weight:700;letter-spacing:.04em;text-transform:uppercase}
    .closeRow{display:flex;justify-content:flex-end;padding:4px 6px 10px}
    .closeBtn{
      padding:10px 12px;border-radius:14px;
      border:1px solid var(--line);
      background:rgba(255,255,255,.05);
      color:var(--text);
      cursor:pointer;
    }
    .menu{display:grid; gap:10px; padding:0 6px 6px;}
    .menu a{
      padding:12px 12px;border-radius:16px;
      border:1px solid var(--line);
      background:rgba(255,255,255,.05);
    }

    .inlineNav{display:none}
    @media (min-width: 920px){
      .wrap{padding:18px 18px 70px}
      .burger{display:none}
      .inlineNav{display:flex;gap:10px;flex-wrap:wrap}
      .inlineNav a{padding:8px 10px;border-radius:999px;color:var(--muted)}
      .inlineNav a:hover{background:rgba(255,255,255,.06);color:var(--text)}
    }

    .hero{margin-top:14px;padding:18px 16px;position:relative;overflow:hidden}
    .hero:before{
      content:""; position:absolute; inset:-120px -160px auto auto;
      width:340px;height:340px;border-radius:50%;
      background:radial-gradient(circle at 30% 30%, rgba(34,211,238,.26), transparent 55%);
      transform:rotate(18deg);
    }
    .kicker{font-size:12px;color:var(--muted);letter-spacing:.12em;text-transform:uppercase}
    h1{margin:10px 0 6px;font-size:30px;line-height:1.12}
    @media (min-width:920px){ h1{font-size:44px} .hero{padding:26px 22px} }
    .subtitle{margin:0;color:var(--muted);line-height:1.6;font-size:14px}
    .badges{display:flex;flex-wrap:wrap;gap:10px;margin:14px 0 14px}
    .badge{
      padding:9px 11px;border-radius:999px;
      border:1px solid var(--line);
      background:rgba(255,255,255,.04);
      font-size:12px;color:rgba(233,237,255,.9);
    }
    .cta{display:flex;flex-wrap:wrap;gap:10px}
    .btn{
      display:inline-flex;align-items:center;justify-content:center;
      padding:12px 14px;border-radius:14px;
      border:1px solid var(--line);
      background:rgba(255,255,255,.04);
      font-weight:650;
      min-height:44px;
      transition:.2s ease;
      flex:1 1 auto;
      text-align:center;
    }
    .btn:active{transform:scale(.99)}
    .btn.primary{
      border-color:transparent;
      background:linear-gradient(135deg,var(--accent),var(--accent2));
      color:#071022;
      font-weight:800;
    }
    @media (min-width:920px){ .btn{flex:0 0 auto} }

    .section{margin-top:14px;padding:16px}
    .section h2{margin:0 0 10px;font-size:18px}
    .p{margin:0;line-height:1.75;color:rgba(233,237,255,.88);font-size:14px}

    .timeline{position:relative;padding:4px 0 0}
    .timeline:before{
      content:"";position:absolute;left:16px;top:0;bottom:0;width:2px;
      background:linear-gradient(180deg, rgba(124,92,255,.7), rgba(34,211,238,.25));
    }
    .tItem{
      position:relative;margin-left:46px;
      padding:14px 14px;border-radius:16px;
      border:1px solid var(--line);
      background:rgba(255,255,255,.04);
      transition:.2s ease;
    }
    .tItem + .tItem{margin-top:12px}
    .tDot{
      position:absolute;left:-38px;top:18px;
      width:12px;height:12px;border-radius:999px;
      background:linear-gradient(135deg,var(--accent),var(--accent2));
      box-shadow:0 0 18px rgba(124,92,255,.55);
    }
    .tLink{
      position:absolute;left:-26px;top:24px;height:2px;width:14px;
      background:rgba(233,237,255,.25);
    }
    .tTitle{margin:0;font-weight:800;font-size:14px}
    .tMeta{margin:6px 0 0;color:var(--muted);font-size:12.5px}
    .tDesc{margin:10px 0 0;line-height:1.65;color:rgba(233,237,255,.86);font-size:13.5px}

    .chips{display:flex;flex-wrap:wrap;gap:10px}
    .chip{
      padding:10px 12px;border-radius:999px;
      border:1px solid var(--line);
      background:rgba(255,255,255,.04);
      font-size:13px;color:rgba(233,237,255,.9);
      min-height:40px; display:flex; align-items:center;
    }

    .reveal{opacity:0;transform: translateY(12px);transition:.65s cubic-bezier(.2,.8,.2,1);}
    .reveal.on{opacity:1;transform:none;}
    footer{margin-top:18px;text-align:center;color:var(--muted);font-size:12.5px}
    ::selection{background:rgba(124,92,255,.35)}
  </style>
</head>

<body>
  <div class="wrap">
    <header class="topbar">
      <div class="brand">
        <span class="dot"></span>
        <strong>Umut Pasha</strong>
      </div>

      <nav class="inlineNav">
        <a href="#about">Hakkımda</a>
        <a href="#edu">Eğitim</a>
        <a href="#exp">Deneyim</a>
        <a href="#awards">Ödüller</a>
        <a href="#skills">Yetenekler</a>
        <a href="#contact">İletişim</a>
      </nav>

      <button class="burger" id="burger" aria-label="Menüyü aç">
        <span></span>
      </button>
    </header>

    <div class="drawer" id="drawer" aria-hidden="true">
      <div class="backdrop" id="backdrop"></div>
      <div class="sheet card">
        <div class="closeRow">
          <button class="closeBtn" id="closeBtn">Kapat</button>
        </div>
        <h3>Menü</h3>
        <div class="menu">
          <a href="#about" class="mLink">Hakkımda</a>
          <a href="#edu" class="mLink">Eğitim</a>
          <a href="#exp" class="mLink">Deneyim</a>
          <a href="#awards" class="mLink">Ödüller</a>
          <a href="#skills" class="mLink">Yetenekler</a>
          <a href="#contact" class="mLink">İletişim</a>
        </div>
      </div>
    </div>

    <!-- HERO -->
    <section class="hero card reveal">
      <div class="kicker">Mobil Öncelikli CV • Portfolyo</div>
      <h1>Umuthan Yalçınkaya <span style="opacity:.75">(“Umut Pasha”)</span></h1>
      <p class="subtitle">
        Kontrol & Otomasyon • Robotik • Gömülü Sistemler • Yazılım / Yapay Zeka • 3D Baskı & Prototipleme
      </p>

      <div class="badges">
        <span class="badge">Marmara Üniversitesi • Kontrol ve Otomasyon</span>
        <span class="badge">Kulüp Başkanı: Dijital İkiz & Otonom Teknolojiler</span>
        <span class="badge">İngilizce: Orta/İyi</span>
      </div>

      <div class="cta">
        <a class="btn primary" href="#contact">İletişim</a>
        <a class="btn" href="https://github.com/YOUR_GITHUB_USERNAME" target="_blank" rel="noreferrer">GitHub</a>
        <a class="btn" href="https://linktr.ee/umutpasha" target="_blank" rel="noreferrer">Linktree</a>
      </div>
    </section>

    <!-- ABOUT -->
    <section id="about" class="section card reveal">
      <h2>Hakkımda</h2>
      <p class="p">
        Marmara Üniversitesi Kontrol ve Otomasyon Teknolojisi öğrencisiyim. Robotik, otonom sistemler,
        gömülü yazılım ve prototipleme (3D baskı) alanlarında üretmeyi seviyorum. T3 Vakfı ve üniversite
        ekosisteminde farklı rollerde deneyim kazandım; takım/organizasyon içinde sorumluluk almayı ve
        proje teslim etmeyi önceliklerimden görüyorum.
      </p>
      <p class="p" style="margin-top:10px">
        Doğum tarihi: 21/08/2005. <!-- Kaynak: ARBIS ve özgeçmiş PDF -->
      </p>
    </section>

    <!-- EDUCATION -->
    <section id="edu" class="section card reveal">
      <h2>Eğitim</h2>
      <div class="timeline">
        <div class="tItem">
          <span class="tDot"></span><span class="tLink"></span>
          <p class="tTitle">Marmara Üniversitesi — Kontrol ve Otomasyon Teknolojisi (Ön Lisans)</p>
          <p class="tMeta">23 Ağustos 2024 – Devam • GNO: 70/100</p>
          <p class="tDesc">Teknik Bilimler MYO — kontrol, otomasyon, uygulamalı mühendislik altyapısı.</p>
        </div>

        <div class="tItem">
          <span class="tDot"></span><span class="tLink"></span>
          <p class="tTitle">Anadolu Üniversitesi — Bilgisayar Programcılığı (Açıköğretim)</p>
          <p class="tMeta">13 Eylül 2025 – Devam</p>
          <p class="tDesc">Yazılım temelleri + pratik geliştirme odağı.</p>
        </div>

        <div class="tItem">
          <span class="tDot"></span><span class="tLink"></span>
          <p class="tTitle">Açık Öğretim Lisesi</p>
          <p class="tMeta">01 Aralık 2022 – 01 Haziran 2023 • GNO: 79.05/100</p>
          <p class="tDesc">Lise öğrenimi.</p>
        </div>
      </div>
      <!-- citations -->
      <!-- Marmara/Anadolu/AÖL + doğum tarihi + linktree -->
      <div style="display:none">
        :contentReference[oaicite:0]{index=0}
      </div>
    </section>

    <!-- EXPERIENCE -->
    <section id="exp" class="section card reveal">
      <h2>Deneyim</h2>
      <div class="timeline">
        <div class="tItem">
          <span class="tDot"></span><span class="tLink"></span>
          <p class="tTitle">Başkan — Dijital İkiz ve Otonom Teknolojiler Kulübü</p>
          <p class="tMeta">Kasım 2024 – Devam • Yarı zamanlı</p>
          <p class="tDesc">Kulüp operasyonu, ekip koordinasyonu, proje ve etkinlik süreçleri.</p>
        </div>

        <div class="tItem">
          <span class="tDot"></span><span class="tLink"></span>
          <p class="tTitle">Üniversite Görevi — Marmara Üniversitesi (Öğretim/Asistan rolü)</p>
          <p class="tMeta">Kasım 2024 – Haziran 2025 • Yarı zamanlı</p>
          <p class="tDesc">Okul içinde uygulamalı süreçlere destek.</p>
        </div>

        <div class="tItem">
          <span class="tDot"></span><span class="tLink"></span>
          <p class="tTitle">Araştırma/Proje Rolü — T3 Vakfı</p>
          <p class="tMeta">Ekim 2023 – Devam • Yarı zamanlı</p>
          <p class="tDesc">Teknoloji ekosisteminde proje süreçleri ve saha deneyimi.</p>
        </div>

        <div class="tItem">
          <span class="tDot"></span><span class="tLink"></span>
          <p class="tTitle">Girişimci/Yönetici — DEEX 3D Baskı</p>
          <p class="tMeta">Nisan 2022 – Ağustos 2023 • Tam zamanlı</p>
          <p class="tDesc">Üretim/prototipleme, müşteri odaklı çözüm geliştirme.</p>
        </div>
      </div>

      <div style="display:none">
        :contentReference[oaicite:1]{index=1}
        :contentReference[oaicite:2]{index=2}
      </div>
    </section>

    <!-- AWARDS -->
    <section id="awards" class="section card reveal">
      <h2>Ödüller / Yarışmalar</h2>
      <div class="timeline">
        <div class="tItem">
          <span class="tDot"></span><span class="tLink"></span>
          <p class="tTitle">FRC Bosphorus Regional — Uluslararası 4.’lük (Finalist)</p>
          <p class="tMeta">10 Mart 2020</p>
          <p class="tDesc">FIRST Robotics Competition (FRC) kapsamında finalist başarı.</p>
        </div>

        <div class="tItem">
          <span class="tDot"></span><span class="tLink"></span>
          <p class="tTitle">KodeLig’22 — “Hedefi Bul (Yapay Zeka)” İkincilik</p>
          <p class="tMeta">29 Ekim 2022</p>
          <p class="tDesc">Yapay zeka temalı yarışma derecesi.</p>
        </div>

        <div class="tItem">
          <span class="tDot"></span><span class="tLink"></span>
          <p class="tTitle">Darobotica — Mini Sumo / Çizgi İzleyen / Labirent Çözen</p>
          <p class="tMeta">25 Nisan 2019</p>
          <p class="tDesc">Birincilikler + ikincilik (farklı kategoriler).</p>
        </div>
      </div>

      <div style="display:none">
        :contentReference[oaicite:3]{index=3}
      </div>
    </section>

    <!-- SKILLS -->
    <section id="skills" class="section card reveal">
      <h2>Yetenekler</h2>
      <div class="chips">
        <span class="chip">Python</span>
        <span class="chip">MATLAB</span>
        <span class="chip">AutoCAD</span>
        <span class="chip">Netcad</span>
        <span class="chip">Office (Word/Excel)</span>
        <span class="chip">HTML5</span>
        <span class="chip">Cisco (VPN / Wireless)</span>
        <span class="chip">Otomasyon Sistemleri Operatörlüğü</span>
        <span class="chip">3D Baskı / Prototipleme</span>
      </div>
      <p class="p" style="margin-top:12px">
        Sertifikalar: “Afet Anında İletişim / VSAT Çözümleri” (TURKSAT) ve “Sistem İzleme ve Müdahale Operasyonları” (Türk Telekom).
      </p>
      <p class="p" style="margin-top:10px">
        İngilizce: B2 dinleme, B1 okuma/konuşma/anlatım, A2 yazma.
      </p>

      <div style="display:none">
        :contentReference[oaicite:4]{index=4}
      </div>
    </section>

    <!-- CONTACT -->
    <section id="contact" class="section card reveal">
      <h2>İletişim</h2>
      <p class="p">
        Mail: <a href="mailto:umuthany@gmail.com">umuthany@gmail.com</a><br/>
        Kurumsal: <a href="mailto:umuthanyalcinkaya@marun.edu.tr">umuthanyalcinkaya@marun.edu.tr</a><br/>
        Telefon: <a href="tel:+905510167061">+90 551 016 70 61</a><br/>
        Linktree: <a href="https://linktr.ee/umutpasha" target="_blank" rel="noreferrer">linktr.ee/umutpasha</a>
      </p>

      <div style="display:none">
        :contentReference[oaicite:5]{index=5}
      </div>
    </section>

    <footer>
      © <span id="year"></span> Umut Pasha • GitHub Pages
    </footer>
  </div>

  <script>
    // Smooth scroll
    document.querySelectorAll('a[href^="#"]').forEach(a=>{
      a.addEventListener('click', (e)=>{
        const id=a.getAttribute('href');
        const el=document.querySelector(id);
        if(!el) return;
        e.preventDefault();
        el.scrollIntoView({behavior:'smooth', block:'start'});
      });
    });

    // Mobile drawer
    const drawer = document.getElementById('drawer');
    const burger = document.getElementById('burger');
    const backdrop = document.getElementById('backdrop');
    const closeBtn = document.getElementById('closeBtn');
    function openDrawer(){
      drawer.classList.add('on');
      drawer.setAttribute('aria-hidden','false');
      document.body.style.overflow='hidden';
    }
    function closeDrawer(){
      drawer.classList.remove('on');
      drawer.setAttribute('aria-hidden','true');
      document.body.style.overflow='';
    }
    burger.addEventListener('click', openDrawer);
    backdrop.addEventListener('click', closeDrawer);
    closeBtn.addEventListener('click', closeDrawer);
    document.querySelectorAll('.mLink').forEach(l=>l.addEventListener('click', closeDrawer));

    // Reveal animation
    const obs = new IntersectionObserver((entries)=>{
      entries.forEach(en=>{ if(en.isIntersecting) en.target.classList.add('on'); });
    }, {threshold:.12});
    document.querySelectorAll('.reveal').forEach(el=>obs.observe(el));

    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
