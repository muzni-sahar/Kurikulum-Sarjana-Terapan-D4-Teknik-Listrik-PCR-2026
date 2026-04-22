[index2.html](https://github.com/user-attachments/files/26980256/index2.html)

<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
  <title>Kurikulum OBE | D4 Teknik Listrik - PNC</title>
  <!-- Google Fonts & Font Awesome -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,600;14..32,700;14..32,800&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Inter', sans-serif;
      background-color: #f8fafc;
      color: #0f172a;
      line-height: 1.5;
      scroll-behavior: smooth;
    }

    .container {
      max-width: 1280px;
      margin: 0 auto;
      padding: 0 24px;
    }

    /* header & navbar */
    .navbar {
      background: white;
      box-shadow: 0 4px 20px rgba(0,0,0,0.03);
      position: sticky;
      top: 0;
      z-index: 100;
      backdrop-filter: blur(2px);
      background: rgba(255,255,255,0.96);
    }
    .nav-container {
      display: flex;
      align-items: center;
      justify-content: space-between;
      flex-wrap: wrap;
      padding: 16px 24px;
      max-width: 1280px;
      margin: 0 auto;
    }
    .logo {
      display: flex;
      align-items: center;
      gap: 12px;
    }
    .logo-icon {
      background: #1e3a5f;
      color: white;
      width: 42px;
      height: 42px;
      display: flex;
      align-items: center;
      justify-content: center;
      border-radius: 12px;
      font-weight: 800;
      font-size: 20px;
    }
    .logo-text h1 {
      font-size: 1.25rem;
      font-weight: 700;
      line-height: 1.2;
    }
    .logo-text p {
      font-size: 0.7rem;
      color: #2563eb;
      font-weight: 600;
    }
    .nav-links {
      display: flex;
      gap: 28px;
      flex-wrap: wrap;
    }
    .nav-links a {
      text-decoration: none;
      font-weight: 500;
      color: #1e293b;
      transition: 0.2s;
    }
    .nav-links a:hover {
      color: #2563eb;
    }
    /* Hero */
    .hero {
      background: linear-gradient(135deg, #eef2ff 0%, #ffffff 100%);
      padding: 60px 0 48px;
      border-bottom: 1px solid #e2e8f0;
    }
    .hero-content {
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
    }
    .badge {
      background: #dbeafe;
      color: #1e40af;
      padding: 6px 14px;
      border-radius: 40px;
      font-size: 0.8rem;
      font-weight: 600;
      display: inline-block;
      margin-bottom: 20px;
    }
    .hero h1 {
      font-size: 2.5rem;
      font-weight: 800;
      background: linear-gradient(135deg, #0f2b3d, #1e4a76);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
      max-width: 800px;
    }
    .hero p {
      font-size: 1.1rem;
      color: #334155;
      max-width: 700px;
      margin-top: 20px;
    }
    /* sections */
    section {
      padding: 64px 0;
      border-bottom: 1px solid #e2e8f0;
    }
    .section-title {
      font-size: 1.8rem;
      font-weight: 700;
      margin-bottom: 12px;
      position: relative;
      display: inline-block;
    }
    .section-sub {
      color: #475569;
      margin-bottom: 40px;
      border-left: 4px solid #2563eb;
      padding-left: 16px;
      font-weight: 500;
    }
    .grid-cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 28px;
      margin-top: 20px;
    }
    .card {
      background: white;
      border-radius: 24px;
      padding: 24px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.02), 0 2px 4px rgba(0,0,0,0.05);
      transition: transform 0.2s, box-shadow 0.2s;
      border: 1px solid #eef2ff;
    }
    .card:hover {
      transform: translateY(-4px);
      box-shadow: 0 20px 25px -12px rgba(0,0,0,0.1);
      border-color: #cbdff2;
    }
    .card-icon {
      font-size: 2rem;
      color: #2563eb;
      margin-bottom: 16px;
    }
    .card h3 {
      font-size: 1.35rem;
      margin-bottom: 12px;
      font-weight: 700;
    }
    .card p, .card li {
      color: #334155;
      font-size: 0.95rem;
    }
    .poe-list, .cpl-list {
      padding-left: 1.2rem;
      margin-top: 12px;
    }
    .poe-list li, .cpl-list li {
      margin-bottom: 8px;
    }
    .profil-flex {
      display: flex;
      flex-wrap: wrap;
      gap: 24px;
    }
    .profil-card {
      flex: 1;
      background: linear-gradient(145deg, #ffffff, #f9fcff);
    }
    .tag {
      display: inline-block;
      background: #e0f2fe;
      padding: 4px 12px;
      border-radius: 20px;
      font-size: 0.7rem;
      font-weight: 700;
      color: #0369a1;
      margin-bottom: 12px;
    }
    .matrix-link {
      background: #f1f5f9;
      border-radius: 20px;
      padding: 24px;
      text-align: center;
      margin-top: 24px;
    }
    footer {
      background: #0f172a;
      color: #cbd5e1;
      padding: 32px 0;
      text-align: center;
    }
    @media (max-width: 760px) {
      .nav-container {
        flex-direction: column;
        gap: 12px;
      }
      .hero h1 {
        font-size: 1.8rem;
      }
      .section-title {
        font-size: 1.5rem;
      }
    }
    .btn-outline {
      border: 1px solid #2563eb;
      background: transparent;
      padding: 8px 20px;
      border-radius: 40px;
      font-weight: 500;
      transition: 0.2s;
      display: inline-block;
      margin-top: 12px;
      color: #2563eb;
      text-decoration: none;
    }
    .btn-outline:hover {
      background: #2563eb;
      color: white;
    }
    .text-small {
      font-size: 0.8rem;
    }
  </style>
</head>
<body>
  <div class="navbar">
    <div class="nav-container">
      <div class="logo">
        <div class="logo-icon"><i class="fas fa-bolt"></i></div>
        <div class="logo-text">
          <h1>D4 Teknik Listrik</h1>
          <p>Politeknik Caltex Riau</p>
        </div>
      </div>
      <div class="nav-links">
        <a href="#profil">Profil Lulusan</a>
        <a href="#poe">POE</a>
        <a href="#cpl">CPL</a>
        <a href="#kurikulum">Kurikulum OBE</a>
      </div>
    </div>
  </div>

  <div class="hero">
    <div class="container hero-content">
      <span class="badge"><i class="fas fa-graduation-cap"></i> Kurikulum OBE | Outcome-Based Education</span>
      <h1>Sarjana Terapan Teknik Listrik <br> Menuju Engineer Profesional Ketenagalistrikan</h1>
      <p>Berbasis standar kompetensi global, nilai IDEAL, dan pembangunan berkelanjutan. Lulusan unggul, inovatif, adaptif, siap bersaing nasional & internasional.</p>
    </div>
  </div>

  <main>
    <!-- PROFIL LULUSAN (Graduate Profiles) -->
    <section id="profil">
      <div class="container">
        <h2 class="section-title">🎓 Profil Lulusan</h2>
        <div class="section-sub">Kompetensi utama yang dibentuk melalui kurikulum terapan</div>
        <div class="profil-flex">
          <div class="card profil-card">
            <div class="card-icon"><i class="fas fa-drafting-compass"></i></div>
            <div class="tag">Electrical Systems Designer & Operational Engineer</div>
            <p>Mampu merencanakan, merancang, dan mengoperasikan sistem tenaga listrik (instalasi, proteksi, otomasi) sesuai standar teknik. Menganalisis, mendiagnosis, mengoptimalkan kinerja sistem secara komprehensif dengan etika, integritas, kepemimpinan, serta solusi inovatif berdaya saing global.</p>
          </div>
          <div class="card profil-card">
            <div class="card-icon"><i class="fas fa-microchip"></i></div>
            <div class="tag">Electrical Installation, Automation & Maintenance Engineer</div>
            <p>Menginstalasi, mengotomasi, dan memelihara sistem tenaga listrik secara sistematis, efektif, efisien. Ahli troubleshooting, optimasi lapangan, menjamin keandalan, keselamatan & keberlanjutan industri. Karakter unggul, inovatif, adaptif.</p>
          </div>
        </div>
      </div>
    </section>

    <!-- POE / PLO (Program Outcomes / Program Learning Outcomes) -->
    <section id="poe" style="background: #fefce8;">
      <div class="container">
        <h2 class="section-title">⚡ Program Outcomes (POE)</h2>
        <div class="section-sub">Capaian Pembelajaran Program Studi – Lulusan mampu menjadi Engineer Profesional Ketenagalistrikan</div>
        <div class="grid-cards">
          <div class="card">
            <div class="card-icon"><i class="fas fa-chalkboard-user"></i></div>
            <h3>POE 1 – Kompetensi Teknik & Keberlanjutan</h3>
            <p>Menguasai prinsip ketenagalistrikan: perancangan, instalasi, proteksi, otomasi, pemeliharaan, pengoperasian sistem tenaga listrik sesuai K3 & pembangunan berkelanjutan. Menghasilkan solusi teknik inovatif dan berdaya saing.</p>
          </div>
          <div class="card">
            <div class="card-icon"><i class="fas fa-hand-sparkles"></i></div>
            <h3>POE 2 – Etika, Pancasila & Nilai IDEAL</h3>
            <p>Menjunjung tinggi Pancasila, etika akademik & profesi, nilai IDEAL (Integrity, Dignity, Excellence, Agility, Loyalty). Jiwa kepemimpinan, tanggung jawab, kerja tim, komunikasi efektif, karakter unggul, inovatif & adaptif.</p>
          </div>
          <div class="card">
            <div class="card-icon"><i class="fas fa-globe"></i></div>
            <h3>POE 3 – Daya Saing Global & Teknologi Terkini</h3>
            <p>Bersaing nasional & global: kompetensi troubleshooting, optimalisasi, pemeliharaan sistem tenaga listrik di industri. Mengadopsi teknologi ketenagalistrikan terkini, efektif, efisien, menjamin keandalan & keselamatan operasi.</p>
          </div>
        </div>
      </div>
    </section>

    <!-- CPL (Course Learning Outcomes) – 10 CPL -->
    <section id="cpl">
      <div class="container">
        <h2 class="section-title">📚 Capaian Pembelajaran Lulusan (CPL)</h2>
        <div class="section-sub">Kompetensi sikap, pengetahuan, dan keterampilan terapan</div>
        <div class="grid-cards" style="grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));">
          <div class="card"><i class="fas fa-pray card-icon"></i><h3>CPL 1</h3><p>Bertakwa, Pancasila, cinta tanah air, etika akademik & profesi, tanggung jawab, semangat kemandirian & kewirausahaan.</p></div>
          <div class="card"><i class="fas fa-gem card-icon"></i><h3>CPL 2</h3><p>Karakter IDEAL (Integrity, Dignity, Excellence, Agility, Loyalty), anti korupsi, budaya melayu, pembelajar mandiri & kritis.</p></div>
          <div class="card"><i class="fas fa-comments card-icon"></i><h3>CPL 3</h3><p>Komunikasi tertulis, lisan, grafis efektif & inklusif, kerja tim multidisiplin, kepemimpinan beragam.</p></div>
          <div class="card"><i class="fas fa-drafting-compass card-icon"></i><h3>CPL 4</h3><p>Merancang sistem/komponen/proses sesuai kebutuhan, perhatikan K3, lingkungan & pembangunan berkelanjutan.</p></div>
          <div class="card"><i class="fas fa-calculator card-icon"></i><h3>CPL 5</h3><p>Mengidentifikasi matematika, IPA, komputasi, rekayasa terapan terhadap prosedur & metodologi yang dikenal.</p></div>
          <div class="card"><i class="fas fa-bolt card-icon"></i><h3>CPL 6</h3><p>Menganalisis, memodelkan, memecahkan masalah teknis sistem tenaga listrik secara sistematis & terstandar.</p></div>
          <div class="card"><i class="fas fa-microchip card-icon"></i><h3>CPL 7</h3><p>Merancang, instalasi, proteksi, otomasi, operasi sistem tenaga listrik, optimasi, solusi inovatif & aman, standar global.</p></div>
          <div class="card"><i class="fas fa-tools card-icon"></i><h3>CPL 8</h3><p>Troubleshooting, pemeliharaan, optimalisasi sistem tenaga listrik di industri, solusi teknis tepat di lapangan.</p></div>
          <div class="card"><i class="fas fa-chart-line card-icon"></i><h3>CPL 9</h3><p>Mengadopsi, evaluasi, implementasi teknologi ketenagalistrikan terkini, integrasi inovasi ke solusi operasional berkelanjutan.</p></div>
          <div class="card"><i class="fas fa-users card-icon"></i><h3>CPL 10</h3><p>Menjalankan peran engineer profesional, integritas, tanggung jawab, kerja tim, kepemimpinan, inovasi teknis & peningkatan berkelanjutan.</p></div>
        </div>
      </div>
    </section>

    <!-- Hubungan POE, Profil Lulusan, CPL - visual matrix sederhana -->
    <section id="kurikulum" style="background: #ecfdf5;">
      <div class="container">
        <h2 class="section-title">🧩 Integrasi Kurikulum OBE</h2>
        <div class="section-sub">Keterkaitan antara Profil Lulusan ↔ POE ↔ CPL sebagai fondasi pembelajaran berbasis outcome</div>
        <div class="matrix-link">
          <i class="fas fa-project-diagram" style="font-size: 2rem; color: #2b6e4f;"></i>
          <p style="margin-top: 16px; font-weight: 500;">Profil Lulusan: <strong>Electrical Systems Designer</strong> & <strong>Automation/Maintenance Engineer</strong> dijabarkan melalui <strong>3 POE</strong> dan didukung oleh <strong>10 CPL</strong> yang mencakup aspek teknis, etika, karakter IDEAL, inovasi, serta daya saing global.</p>
          <div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 12px; margin-top: 24px;">
            <span class="badge" style="background:#1e3a5f; color:white;">🔗 POE 1 → CPL 4,5,6,7,9</span>
            <span class="badge" style="background:#1e3a5f; color:white;">🔗 POE 2 → CPL 1,2,3,10</span>
            <span class="badge" style="background:#1e3a5f; color:white;">🔗 POE 3 → CPL 7,8,9,10</span>
          </div>
          <a href="#" class="btn-outline" style="margin-top: 28px;"><i class="fas fa-download"></i> Unduh Peta Kurikulum (dummy)</a>
        </div>
        <div style="margin-top: 32px; background: white; border-radius: 28px; padding: 20px; border: 1px solid #cbd5e1;">
          <h3 style="font-weight: 700;">✨ Keunggulan Program D4 Teknik Listrik PNC</h3>
          <ul style="columns: 1; list-style: none; margin-top: 16px;">
            <li><i class="fas fa-check-circle" style="color:#2563eb;"></i> Kurikulum berbasis OBE (Outcome-Based Education) terintegrasi industri</li>
            <li><i class="fas fa-check-circle" style="color:#2563eb;"></i> Laboratorium canggih: proteksi, otomasi industri, simulasi tenaga listrik</li>
            <li><i class="fas fa-check-circle" style="color:#2563eb;"></i> Magang bersertifikasi di perusahaan nasional & multinasional</li>
            <li><i class="fas fa-check-circle" style="color:#2563eb;"></i> Soft skill kepemimpinan & nilai IDEAL berbasis budaya melayu</li>
            <li><i class="fas fa-check-circle" style="color:#2563eb;"></i> Lulusan siap kerja sebagai engineer perencana, operasional, maintenance, automation specialist</li>
          </ul>
        </div>
      </div>
    </section>

    <!-- Tabel POE & Profil Lulusan matrix sederhana -->
    <section style="padding: 40px 0;">
      <div class="container">
        <div style="background: white; border-radius: 32px; overflow-x: auto;">
          <table style="width:100%; border-collapse: collapse; text-align: left;">
            <thead style="background: #1e293b; color: white;">
              <tr><th style="padding: 16px;">Profil Lulusan</th><th style="padding: 16px;">POE Terkait</th><th style="padding: 16px;">CPL Inti</th></tr>
            </thead>
            <tbody>
              <tr style="border-bottom: 1px solid #e2e8f0;"><td style="padding: 14px;"><b>Electrical Systems Designer & Operational Engineer</b><br>Perancang & operator sistem tenaga</td><td style="padding: 14px;">POE 1, POE 2</td><td style="padding: 14px;">CPL 4, CPL 6, CPL 7, CPL 10</td></tr>
              <tr style="border-bottom: 1px solid #e2e8f0;"><td style="padding: 14px;"><b>Electrical Installation, Automation & Maintenance Engineer</b><br>Instalasi, otomasi, pemeliharaan</td><td style="padding: 14px;">POE 1, POE 3</td><td style="padding: 14px;">CPL 7, CPL 8, CPL 9, CPL 5</td></tr>
            </tbody>
          </table>
        </div>
        <p class="text-small" style="margin-top: 16px; text-align: center;">* Matriks capaian pembelajaran terintegrasi dengan prinsip keberlanjutan, K3, serta standar global</p>
      </div>
    </section>
  </main>

  <footer>
    <div class="container">
      <p><i class="fas fa-university"></i> Program Studi Sarjana Terapan Teknik Listrik | Politeknik Caltex Riau</p>
      <p style="margin-top: 8px; font-size: 0.8rem;">Kurikulum OBE berbasis KKNI & SN-Dikti, berorientasi Outcome-Based Education dengan keunggulan kompetensi Engineer Profesional Ketenagalistrikan.</p>
      <p style="margin-top: 16px;">📍 Kampus PNC - Riau | © 2026 | <i class="fas fa-solar-panel"></i> Inovasi untuk keberlanjutan energi</p>
    </div>
  </footer>
</body>
</html>
