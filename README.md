<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Profil Interaktif</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: Arial, sans-serif;
      display: flex;
      min-height: 100vh;
      background-color:#2b37a6;;
    }

    .sidebar {
      width: 250px;
      background-color: lch(58.15% 31.65 261.05 / 0.352);
      color: rgb(236, 229, 229);
      padding: 30px 20px;
      text-align: center;
    }

    .sidebar img {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      object-fit: cover;
      margin-bottom: 15px;
      border: 3px solid #lch;
    }

    .sidebar h1 {
      font-size: 20px;
      margin-bottom: 10px;
    }

    .sidebar a {
      display: block;
      color: white;
      text-decoration: none;
      margin: 10px 0;
      font-size: 14px;
      cursor: pointer;
      padding: 8px;
      border-radius: 5px;
      transition: background 0.3s;
    }

    .sidebar a:hover {
      background-color: #2ecc71;
    }

    .content {
      flex: 1;
      padding: 40px;
      overflow-y: auto;
    }

    .card {
      background-color: rgb(109, 168, 247);
      padding: 25px;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      margin-bottom: 20px;
    }

    .card h2 {
      margin-bottom: 10px;
      color: #2c3e50;
    }

    .biodata-item {
      margin-bottom: 10px;
    }

    .skill-tag {
      display: inline-block;
      background: #2ecc71;
      color: white;
      padding: 5px 10px;
      border-radius: 20px;
      margin: 5px 5px 0 0;
      font-size: 13px;
    }

    .section {
      display: none;
    }

    .section.active {
      display: block;
    }

    /* === HOME SECTION STYLE === */
    #home {
      position: relative;
      height: 100%;
      min-height: 80vh;
      padding: 0;
    }

    .home-background {
      background-image: url('https://images.unsplash.com/photo-1498050108023-c5249f4df085');
      background-size: cover;
      background-position: center;
      height: 100%;
      border-radius: 10px;
      position: relative;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      color: white;
    }

    .home-overlay {
      background-color: rgba(0, 0, 0, 0.6);
      padding: 50px;
      border-radius: 10px;
    }

    .home-overlay h1 {
      font-size: 40px;
      margin-bottom: 20px;
    }

    .home-overlay p {
      font-size: 18px;
      line-height: 1.6;
      max-width: 600px;
      margin: 0 auto;
    }
    
  </style>
  
</head>
<body>

  <div class="sidebar">
    <img src="c:\Users\HP\Downloads\WhatsApp Image 2025-06-04 at 11.28.30_8a7ffed4.jpg" alt="Foto Profil">
    <h1>Rabiatul Samaiya</h1>
    <a onclick="showSection('home')">Home</a>
    <a onclick="showSection('about')">About Me</a>
    <a onclick="showSection('social')">Social Media</a>
    <a onclick="showSection('contact')">Contact</a>
  </div>

  <div class="content">
    <!-- HOME SECTION -->
    <div id="home" class="section active">
      <div class="home-background">
        <div class="home-overlay">
          <h1>Selamat Datang di Profil Saya</h1>
          <p>Halo! Saya Rabiatul Samaiya,Pengembang kreatif dengan semangat di dunia desain dan teknologi. Selamat datang!</p>
        </div>
      </div>
    </div>

    <!-- ABOUT SECTION -->
    <div id="about" class="section">
      <div class="card">
        <h2>Tempat, Tanggal Lahir</h2>
        <div class="biodata-item">Lubuk Pakam,1 April 2005</div>
      </div>
      <div class="card">
    <h2>Skill</h2>
    <div id="skill-container">
      <button class="skill-tag" onclick="showSkillImage('js')">Blender</button>
       <a href="https://drive.google.com/file/d/1qJOrpRUwnQnVKpp1S7q6xpvNqi-ygke7/view?usp=drive_link">Blender></a>
      <button class="skill-tag" onclick="showSkillImage('uiux')">lightroom</button>
       <a href="https://drive.google.com/file/d/1Ce_Ksy926ySYVpqzD3g7lF8Ok6bzBTAR/view?usp=drive_linkd">lightroom></a>
      <button class="skill-tag" onclick="showSkillImage('canva')">Canva</button>
       <a href="https://drive.google.com/file/d/1UcENKv-dIUC_WU5_RdHTOmRPEA97hweF/view?usp=drive_linkd hover:bg-purple-700 text-sm">Canva</a>

    </div>
    <div id="skill-image" style="margin-top: 20px; text-align:center;"></div>
  </div>

      <div class="card">
        <h2>Hobi</h2>
        <ul>
          <li>Menonton film/Drakor</li>
          <li>Membaca Novel,Webtoon,Manga,dan Manhwa</li>
        </ul>
      </div>
      <div class="card">
        <h2>Tentang Saya</h2>
        <p>Saya adalah seorang mahasiswa yang sedang belajar menjadi seorang devolever yang ingin membuat website modern dan menarik.</p>
      </div>
    </div>

    <!-- SOCIAL MEDIA -->
    <div id="social" class="section">
      <div class="card">
        <h2>Media Sosial</h2>
        <div class="biodata-item">Instagram: https://www.instagram.com/sasao__o?igsh=MXI3eWNzYmtvamhpaQ==</div>
        <div class="biodata-item">Facebook: https://www.facebook.com/rabiatul.samaiya</div>
        <div class="biodata-item">GitHub: https://github.com/rabiatulsasa</div>
      </div>
    </div>

    <!-- CONTACT SECTION -->
    <div id="contact" class="section">
      <div class="card">
        <h2>Kontak</h2>
        <div class="biodata-item">email:wawaoppo54@gmail.com</div>
        <div class="biodata-item">No HP: 0812-3456-7890</div>
      </div>
    </div>
  </div>

  <script>
    function showSection(id) {
      const sections = document.querySelectorAll('.section');
      sections.forEach(sec => sec.classList.remove('active'));
      document.getElementById(id).classList.add('active');
    }
  </script>

</body>
</html>
