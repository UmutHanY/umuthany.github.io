<html lang="tr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1,viewport-fit=cover" />
  <title>umut.hany | CV</title>
  <meta name="description" content="Mobil öncelikli CV & Portfolyo — Umuthan “.exe” Yalçınkaya" />

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
    .sheet h3{margin:6px 8px 10px;font-size:14px;color:var(--muted);font-weight:800;letter-spacing:.04em;text-transform:uppercase}
    .closeRow{display:flex;justify-content:flex-end;padding:4px 6px 10px}
    .closeBtn{
      padding:10px 12px;border-radius:14px;
      border:1px solid var(--line);
      background:rgba(255,255,255,.05);
      color:var(--text);
      cursor:pointer;
      min-height:44px;
    }
    .menu{display:grid; gap:10px; padding:0 6px 6px;}
    .menu a{
      padding:12px 12px;border-radius:16px;
      border:1px solid var(--line);
      background:rgba(255,255,255,.05);
      min-height:44px;
      display:flex;align-items:center;
    }

    .inlineNav{display:none}
    @media (min-width: 920px){
      .wrap{padding:18px 18px 70px}
      .burger{display:none}
      .inlineNav{display:flex;gap:10px;flex-wrap:wrap}
      .inlineNav a{padding:8px 10px;border-radius:999px;color:var(--muted)}
      .inlineNav a:hover{background:rgba(255,255,255,.06);color:var(--text)}
    }

    /* HERO */
    .hero{margin-top:14px;padding:18px 16px;position:relative;overflow:hidden}
    .hero:before{
      content:""; position:absolute; inset:-120px -160px auto auto;
      width:340px;height:340px;border-radius:50%;
      background:radial-gradient(circle at 30% 30%, rgba(34,211,238,.26), transparent 55%);
      transform:rotate(18deg);
    }
    .heroTop{
      display:flex; align-items:flex-start; gap:12px; justify-content:space-between;
      margin-bottom:10px;
    }
    .kicker{
      font-size:12px;color:var(--muted);
      letter-spacing:.02em;
      font-weight:900;
    }

    .profileWrap{
      display:flex;
      flex-direction:column;
      align-items:flex-end;
      gap:8px;
      flex:0 0 auto;
    }
    .profile{
      width:78px;height:78px;border-radius:18px;
      border:1px solid var(--line);
      background:rgba(255,255,255,.04);
      overflow:hidden;
      box-shadow:0 10px 26px rgba(0,0,0,.25);
    }
    .profile img{
      width:100%;
      height:100%;
      object-fit:cover;       /* maksimum kutuya sığacak şekilde kırp */
      object-position:center; /* ortadan */
      display:block;
    }
    .rolesUnderPhoto{
      margin:0;
      font-size:11.5px;
      color:rgba(233,237,255,.75);
      text-align:right;
      line-height:1.35;
      font-weight:800;
    }

    h1{margin:10px 0 6px;font-size:30px;line-height:1.12}
    @media (min-width:920px){ h1{font-size:44px} .hero{padding:26px 22px} .profile{width:92px;height:92px} }
    .subtitle{margin:0;color:rgba(233,237,255,.86);line-height:1.6;font-size:14px}
    .subtitle2{margin:10px 0 0;color:var(--muted);line-height:1.7;font-size:13.5px}

    .badges{
      display:flex;
      flex-direction:column;   /* alt alta */
      gap:10px;
      margin:14px 0 14px;
      align-items:flex-start;
    }
    .badge{
      padding:9px 11px;border-radius:14px;
      border:1px solid var(--line);
      background:rgba(255,255,255,.04);
      font-size:12.5px;color:rgba(233,237,255,.9);
      width:100%;
      max-width: 100%;
    }

    .cta{display:flex;flex-wrap:wrap;gap:10px}
    .btn{
      display:inline-flex;align-items:center;justify-content:center;
      padding:12px 14px;border-radius:14px;
      border:1px solid var(--line);
      background:rgba(255,255,255,.04);
      font-weight:800;
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
      font-weight:950;
    }
    @media (min-width:920px){ .btn{flex:0 0 auto} }

    /* Sections */
    .section{margin-top:14px;padding:16px}
    .section h2{margin:0 0 10px;font-size:18px}
    .p{margin:0;line-height:1.78;color:rgba(233,237,255,.90);font-size:14px}

    /* Timeline */
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
    .tTitle{margin:0;font-weight:950;font-size:14px}
    .tMeta{margin:6px 0 0;color:var(--muted);font-size:12.5px}
    .tDesc{margin:10px 0 0;line-height:1.65;color:rgba(233,237,255,.86);font-size:13.5px}

    /* Chips */
    .chips{display:flex;flex-wrap:wrap;gap:10px}
    .chip{
      padding:10px 12px;border-radius:999px;
      border:1px solid var(--line);
      background:rgba(255,255,255,.04);
      font-size:13px;color:rgba(233,237,255,.9);
      min-height:40px; display:flex; align-items:center;
    }

    /* Read more blocks */
    .fadeClamp{
      position:relative;
      max-height:170px;
      overflow:hidden;
    }
    .fadeClamp:after{
      content:"";
      position:absolute; left:0; right:0; bottom:0; height:64px;
      background:linear-gradient(180deg, rgba(11,16,32,0), rgba(11,16,32,.92));
      pointer-events:none;
    }
    .expanded{max-height:none !important;}
    .expanded:after{display:none !important;}

    .moreRow{display:flex;justify-content:flex-start;margin-top:12px}
    .moreBtn{
      min-height:44px;
      padding:12px 14px;
      border-radius:14px;
      border:1px solid var(--line);
      background:rgba(255,255,255,.05);
      color:var(--text);
      font-weight:900;
      cursor:pointer;
    }

    /* Contact icons */
    .iconRow{display:flex;gap:12px;flex-wrap:wrap;margin-top:10px}
    .iconBtn{
      display:inline-flex;align-items:center;gap:10px;
      padding:12px 14px;border-radius:16px;
      border:1px solid var(--line);
      background:rgba(255,255,255,.04);
      min-height:44px;
      font-weight:900;
      flex:1 1 auto;
    }
    .icon{width:20px;height:20px;opacity:.95;flex:0 0 auto;}
    .note{
      margin-top:12px;
      color:var(--muted);
      font-size:13px;
      line-height:1.7;
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
        <strong>umut.hany</strong>
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
      <div class="heroTop">
        <div class="kicker">Portfolyoma Hoşgeldiniz</div>

        <!-- Fotoğraf: assets/profile.jpg (attığın foto burada) -->
        <div class="profileWrap">
          <div class="profile" title="Profil Fotoğrafı">
            <img src="assets/profile.jpg" alt="Umuthan .exe Yalçınkaya"
              onerror="this.style.display='none'; this.parentElement.style.display='grid'; this.parentElement.style.placeItems='center'; this.parentElement.innerHTML='<span style=&quot;color:rgba(233,237,255,.65);font-weight:950;font-size:12px;padding:0 10px;text-align:center;line-height:1.2;&quot;>Fotoğraf<br/>Yükle</span>';">
          </div>
          <p class="rolesUnderPhoto">
            Öğrenci • Öğretmen • Asistan<br/>
            Araştırmacı • Proje Danışmanı<br/>
            Mentör • E-Sporcu
          </p>
        </div>
      </div>

      <h1>Umuthan “.exe” Yalçınkaya</h1>

      <p class="subtitle">
        Yazılım, Robotik, Otomasyon, Gömülü Sistemler, Yapay Zeka, 3D Modelleme, Tarih, Jeoloji ve Coğrafya, Din ve Dinler Tarihi,
        Felsefe ve Düşünce Biçimi, Şiir ve Hikâye Yazarı, Astronomi, Kuantum Fiziği, Uzay-Zaman, Hayvan Moleküler Genetiği,
        Bitki Moleküler Genetiği, Oyun ve Animasyon Yapımı, Anatomi, Kimya ve Atom Yapısı
      </p>

      <!-- Tagler alt alta -->
      <div class="badges" aria-label="Etiketler">
        <span class="badge">Marmara Üniversitesi - Kontrol ve Otomasyon</span>
        <span class="badge">Anadolu Üniversitesi - Bilgisayar Programcılığı</span>
        <span class="badge">Dijital İkiz ve Otonom Teknolojiler - Kulüp Başkanı</span>
        <span class="badge">Team Flux - Takım Kaptanı</span>
        <span class="badge">Marmara Üniversitesi - Asistan</span>
        <span class="badge">Marmara Üniversitesi - Proje Danışmanı</span>
        <span class="badge">Team Simurg - Takım Kaptanı</span>
        <span class="badge">SIMURG Öğrenci Topluluğu - Başkan</span>
        <span class="badge">Techno-Rob Takım Kaptanı</span>
        <span class="badge">DeeX3D Baskı - Kurucu</span>
        <span class="badge">TUBİTAK - Araştırmacı</span>
        <span class="badge">T3 Vakfı - Eğitmen</span>
        <span class="badge">İst-İnka - Takım Kaptanı</span>
        <span class="badge">İngilizce - B2</span>
        <span class="badge">Arapça - B1</span>
        <span class="badge">Latince - B1</span>
        <span class="badge">Farsca - B2</span>
        <span class="badge">Rusca - B2</span>
        <span class="badge">Azerice - C1</span>
      </div>

      <div class="cta">
        <a class="btn primary" href="#contact">İletişim</a>
        <a class="btn" href="https://github.com/YOUR_GITHUB_USERNAME" target="_blank" rel="noreferrer">GitHub</a>
        <a class="btn" href="https://www.instagram.com/umut.hany" target="_blank" rel="noreferrer">Instagram</a>
      </div>
    </section>

    <!-- ABOUT -->
    <section id="about" class="section card reveal">
      <h2>Hakkımda</h2>

      <div id="aboutClamp" class="fadeClamp">
        <p class="p">
          Merhaba, ben Umuthan Yalçınkaya. 21 Ağustos 2005 tarihinde doğdum. Doğduğum günden itibaren alışılmışın dışında olmam,
          sıradan bir hayatım olmayacağını belli ediyordu.
        </p>
        <p class="p" style="margin-top:10px">
          İlkokul yıllarında bilime dair ilk adımlarımı attım. Henüz 9 yaşımdayken Kocaeli’de düzenlenen Darobotica Ortaokul/Lise
          robotik yarışmasına dört dalda, dört robotla katıldım ve üç birincilik ile bir ikincilik kazanarak ilimizde önde gelen
          liseleri ve ortaokulları geride bıraktım.
        </p>
        <p class="p" style="margin-top:10px">
          8. sınıfta kimyaya olan merakım ve Oktanyum hocamızın eğitimiyle TEKNOFEST’te birincilik kazandıran “En Verimli Roket Yakıtı”
          ödülünü elde ettim. 14 yaşımda, fizik hocamın yönlendirmesiyle TÜBİTAK’ta gönüllü araştırmacı olarak çalışmaya başladım.
          Aynı yıl okulun FRC takımı Techno-Rob’da programmer olarak görev aldım. İki yıl üst üste FRC yarışmasına katıldık; bir yıl
          şampiyon, diğer yıl finalist olarak tamamladık.
        </p>
        <p class="p" style="margin-top:10px">
          16 yaşımda KodeLig ve hackathon yarışmalarını üst üste birinciliklerle tamamladım. 17 yaşımda ise okulun alt sınıflarından
          oluşan ekiplere mentörlük desteği vererek yarışmalara hazırladım; toplamda dokuz takıma, on iki kupa kazandırarak okulumuzun
          başarı grafiğine katkı sağladım.
        </p>
        <p class="p" style="margin-top:10px">
          18 yaşımda “Geri Dönüştürülmüş Malzemelerden Elektrikli Araba” projesini hayata geçirdim ve neredeyse sıfır maliyetle
          elektrikli bir araç inşa ettim. Bu proje ile TEKNOFEST “Bağımsız Projeler” dalında ikincilik kazandım.
        </p>
        <p class="p" style="margin-top:10px">
          20 yaşıma kadar geçen süreçte onlarca farklı makale ve tez yazarak araştırmacı kimliğimi güçlendirdim. 20 yaşımda Marmara
          Üniversitesi’nde DIOT Kulübü’nü, hem eğitim veren hem de yarışmalara hazırlayan bir yapı olarak kurdum. Ardından SIMURG
          Öğrenci Topluluğu’nu kurarak İTÜ, YTÜ, GTÜ, Yeditepe Üniversitesi, Bahçeşehir Üniversitesi ve Marmara Üniversitesi arasında
          bir network ağı oluşturdum; öğrencilerin ve kulüplerin kaynaşmasını sağladım.
        </p>
        <p class="p" style="margin-top:10px">
          Bu topluluklardan önde gelen başarılı öğrencilerle Team Simurg ve İst-İnka TEKNOFEST ekiplerini kurdum. Aynı yıl üniversite
          idaresinden gelen asistan öğrencilik teklifini kabul ettim; laboratuvar derslerinde ve öğrenci projelerinde destek veren
          yarı-eğitmen sorumluluğunu üstlendim.
        </p>
        <p class="p" style="margin-top:10px">
          2025–2026 sezonunda, batarya verimliliğini artırmaya yönelik kendi tasarımım bir projenin patentini aldım; proje Bayraktar
          İHA’larında kullanılması için revize edildi. Ayrıca “Nörolojik Duygu Ağına Sahip Yapay Zeka” projemin lisansını ve patentini
          TÜBİTAK’tan aldım. Bu yıl içinde okulun TEKNOFEST, bitirme, ders ve bağımsız projelerini desteklemek adına “Proje Danışmanı”
          olarak göreve başladım. Yine aynı yıl içinde Team Flux başta olmak üzere beş TEKNOFEST takımı kurdum.
        </p>

        <p class="p" style="margin-top:10px">
          Bunca yıl ve proje süreci içerisinde, aynı zamanda 15 yıllık Counter-Strike oyun serüvenimin son 5 yılını profesyonel
          e-sporcu olarak geçirdim. Goliath Gaming ve Eternal Fire Academy gibi takımlarda forma giymemin yanı sıra, CS:GO döneminde
          ESEA League 21, 22 ve 23 sezonlarında şampiyonluklar elde ettim. CS2 European Pro League’de ise takımımın da katkılarıyla
          şampiyonluk başarısı yakaladık.
        </p>
      </div>

      <div class="moreRow">
        <button class="moreBtn" data-toggle="aboutClamp" data-label-open="Devamını Oku" data-label-close="Kısalt">
          Devamını Oku
        </button>
      </div>
    </section>

    <!-- EDUCATION -->
    <section id="edu" class="section card reveal">
      <h2>Eğitim</h2>

      <div id="eduClamp" class="fadeClamp">
        <div class="timeline">
          <div class="tItem">
            <span class="tDot"></span><span class="tLink"></span>
            <p class="tTitle">15 Temmuz Şehitler Fen Lisesi - Sayısal</p>
            <p class="tMeta">10 Eylül 2019 – 1 Kasım 2022 • GNO: 89.05</p>
            <p class="tDesc">Sayısal alan, yarışma ve proje odaklı dönem.</p>
          </div>

          <div class="tItem">
            <span class="tDot"></span><span class="tLink"></span>
            <p class="tTitle">MEB Açıköğretim Lisesi</p>
            <p class="tMeta">1 Aralık 2022 – 1 Haziran 2023 • GNO: 99.5</p>
            <p class="tDesc">Lise tamamlandı.</p>
          </div>

          <div class="tItem">
            <span class="tDot"></span><span class="tLink"></span>
            <p class="tTitle">Marmara Üniversitesi - Kontrol ve Otomasyon Teknolojisi</p>
            <p class="tMeta">23 Ağustos 2024 – Devam • GNO: 85/100</p>
            <p class="tDesc">Kontrol, otomasyon, uygulamalı mühendislik altyapısı.</p>
          </div>

          <div class="tItem">
            <span class="tDot"></span><span class="tLink"></span>
            <p class="tTitle">Anadolu Üniversitesi - Bilgisayar Programcılığı (AÖF)</p>
            <p class="tMeta">13 Eylül 2025 – Devam</p>
            <p class="tDesc">Yazılım temelleri + pratik geliştirme odağı.</p>
          </div>
        </div>
      </div>

      <div class="moreRow">
        <button class="moreBtn" data-toggle="eduClamp" data-label-open="Devamını Oku" data-label-close="Kısalt">
          Devamını Oku
        </button>
      </div>
    </section>

    <!-- EXPERIENCE -->
    <section id="exp" class="section card reveal">
      <h2>Deneyim</h2>

      <div id="expClamp" class="fadeClamp">
        <div class="timeline">
          <div class="tItem">
            <span class="tDot"></span><span class="tLink"></span>
            <p class="tTitle">Kulüp Başkanı — Dijital İkiz ve Otonom Teknolojiler</p>
            <p class="tMeta">Kasım 2024 – Devam</p>
            <p class="tDesc">Kulüp operasyonu, ekip koordinasyonu, proje ve etkinlik süreçleri.</p>
          </div>

          <div class="tItem">
            <span class="tDot"></span><span class="tLink"></span>
            <p class="tTitle">Asistan — Marmara Üniversitesi</p>
            <p class="tMeta">Kasım 2024 – Devam</p>
            <p class="tDesc">Laboratuvar dersleri ve öğrenci projelerinde teknik destek.</p>
          </div>

          <div class="tItem">
            <span class="tDot"></span><span class="tLink"></span>
            <p class="tTitle">Eğitmen — T3 Vakfı</p>
            <p class="tMeta">Aralık 2025 – Devam</p>
            <p class="tDesc">Deneyap Atölyelerinde eğitmenlik.</p>
          </div>

          <div class="tItem">
            <span class="tDot"></span><span class="tLink"></span>
            <p class="tTitle">Araştırmacı / Proje Uzmanı — TÜBİTAK</p>
            <p class="tMeta">2019 – Devam</p>
            <p class="tDesc">Uzmanlık alanları hakkında TÜBİTAK adına bilimsel çalıştaylara katılım ve projeler yürütülmesi.</p>
          </div>

          <div class="tItem">
            <span class="tDot"></span><span class="tLink"></span>
            <p class="tTitle">Kurucu — DeeX 3D Baskı</p>
            <p class="tMeta">Nisan 2022 – Ağustos 2023</p>
            <p class="tDesc">3D baskı ve modelleme atölyesi kurmak.</p>
          </div>
        </div>
      </div>

      <div class="moreRow">
        <button class="moreBtn" data-toggle="expClamp" data-label-open="Devamını Oku" data-label-close="Kısalt">
          Devamını Oku
        </button>
      </div>
    </section>

    <!-- AWARDS -->
    <section id="awards" class="section card reveal">
      <h2>Ödüller / Yarışmalar</h2>

      <div id="awardsClamp" class="fadeClamp">
        <div class="timeline">
          <div class="tItem">
            <span class="tDot"></span><span class="tLink"></span>
            <p class="tTitle">Darobotica — Mini Sumo (1.’lik)</p>
            <p class="tMeta">~ 2014–2016 (yaklaşık)</p>
            <p class="tDesc">Robotik yarışması kapsamında birincilik.</p>
          </div>

          <div class="tItem">
            <span class="tDot"></span><span class="tLink"></span>
            <p class="tTitle">Darobotica — Çizgi İzleyen (1.’lik)</p>
            <p class="tMeta">~ 2014–2016 (yaklaşık)</p>
            <p class="tDesc">Robotik yarışması kapsamında birincilik.</p>
          </div>

          <div class="tItem">
            <span class="tDot"></span><span class="tLink"></span>
            <p class="tTitle">Darobotica — Labirent Çözen (1.’lik)</p>
            <p class="tMeta">~ 2014–2016 (yaklaşık)</p>
            <p class="tDesc">Robotik yarışması kapsamında birincilik.</p>
          </div>

          <div class="tItem">
            <span class="tDot"></span><span class="tLink"></span>
            <p class="tTitle">Darobotica — (2.’lik)</p>
            <p class="tMeta">~ 2014–2016 (yaklaşık)</p>
            <p class="tDesc">Robotik yarışması kapsamında ikincilik.</p>
          </div>

          <div class="tItem">
            <span class="tDot"></span><span class="tLink"></span>
            <p
