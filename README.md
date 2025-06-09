<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Profil Rabiatul Samaiya</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
    }

    header {
      background-color: #0077cc;
      color: white;
      padding: 20px;
      text-align: center;
    }

    .navbar {
      display: flex;
      justify-content: center;
      background-color: #005fa3;
    }

    .navbar a {
      color: white;
      padding: 14px 20px;
      text-decoration: none;
      text-align: center;
    }

    .navbar a:hover {
      background-color: #003f6b;
    }

    .content {
      display: flex;
      flex-direction: row; /* supaya konten disusun ke samping */
      padding: 20px;
    }

    .box {
      flex: 1;
      margin: 10px;
      padding: 20px;
      background-color: #eaeaea;
      border-radius: 10px;
    }
  </style>
</head>
<body>

  <header>
    <h1>Rabiatul Samaiya</h1>
    <p>Selamat Datang di Profil Saya</p>
  </header>

  <div class="navbar">
    <a href="#">Home</a>
    <a href="#">About Me</a>
    <a href="#">Social Media</a>
    <a href="#">Contact</a>
  </div>

  <div class="content">
    <div class="box">
      <h2>Home</h2>
      <p>Selamat datang di halaman utama.</p>
    </div>
    <div class="box">
      <h2>About Me</h2>
      <p>Ini adalah bagian tentang saya.</p>
    </div>
    <div class="box">
      <h2>Social Media</h2>
      <p>Temukan saya di media sosial.</p>
    </div>
    <div class="box">
      <h2>Contact</h2>
      <p>Hubungi saya di sini.</p>
    </div>
  </div>

</body>
</html>
