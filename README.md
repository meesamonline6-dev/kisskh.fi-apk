 <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>kisskh.fi - APK Download</title>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
    }

    body {
      background: #f5f5f5;
      color: #222;
    }

    header {
      background: #111;
      color: white;
      padding: 18px 25px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
    }

    .logo {
      font-size: 24px;
      font-weight: bold;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin-left: 20px;
      font-size: 15px;
    }

    .hero {
      background: #1d1d1d;
      color: white;
      text-align: center;
      padding: 70px 20px;
    }

    .hero h1 {
      font-size: 42px;
      margin-bottom: 15px;
    }

    .hero p {
      color: #ccc;
      margin-bottom: 25px;
    }

    .search {
      width: 90%;
      max-width: 500px;
      padding: 14px;
      border: none;
      border-radius: 8px;
      font-size: 16px;
    }

    .container {
      max-width: 1100px;
      margin: 40px auto;
      padding: 0 20px;
    }

    .title {
      text-align: center;
      margin-bottom: 25px;
      font-size: 28px;
    }

    .apps {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }

    .card {
      background: white;
      border-radius: 12px;
      padding: 20px;
      box-shadow: 0 3px 12px rgba(0,0,0,0.08);
    }

    .app-icon {
      width: 80px;
      height: 80px;
      background: #ddd;
      border-radius: 18px;
      display: flex;
      align-items: center;
      justify-content: center;
      margin-bottom: 15px;
      font-size: 30px;
    }

    .card h3 {
      margin-bottom: 8px;
    }

    .info {
      color: #777;
      font-size: 14px;
      margin-bottom: 15px;
    }

    .download {
      display: block;
      background: #111;
      color: white;
      text-align: center;
      text-decoration: none;
      padding: 12px;
      border-radius: 7px;
      font-weight: bold;
    }

    .download:hover {
      background: #333;
    }

    footer {
      margin-top: 50px;
      background: #111;
      color: #aaa;
      text-align: center;
      padding: 25px;
    }

    @media (max-width: 600px) {
      header {
        flex-direction: column;
        gap: 12px;
      }

      nav a {
        margin: 0 7px;
      }

      .hero h1 {
        font-size: 32px;
      }
    }
  </style>
</head>

<body>

  <header>
    <div class="logo">kisskh.fi</div>

    <nav>
      <a href="#">Home</a>
      <a href="#apps">Apps</a>
      <a href="#about">About</a>
    </nav>
  </header>

  <section class="hero">
    <h1>kisskh.fi</h1>
    <p>Download your favorite apps easily</p>

    <input
      class="search"
      type="text"
      placeholder="Search APK..."
      onkeyup="searchApps()"
      id="searchBox"
    >
  </section>

  <div class="container" id="apps">

    <h2 class="title">Latest APKs</h2>

    <div class="apps" id="appList">

      <div class="card">
        <div class="app-icon">📱</div>

        <h3>My APK App</h3>

        <p class="info">
          Version: 1.0.0<br>
          Size: 25 MB<br>
          Android: 5.0+
        </p>

        <!-- Yahan apni APK ka link lagana hai -->
        <a class="download" href="YOUR-APK-LINK-HERE" download>
          Download APK
        </a>
      </div>

      <div class="card">
        <div class="app-icon">🎮</div>

        <h3>My Game</h3>

        <p class="info">
          Version: 2.0.0<br>
          Size: 80 MB<br>
          Android: 6.0+
        </p>

        <!-- Yahan doosri APK ka link lagana hai -->
        <a class="download" href="YOUR-APK-LINK-HERE" download>
          Download APK
        </a>
      </div>

    </div>
  </div>

  <div class="container" id="about">
    <h2 class="title">About kisskh.fi</h2>

    <p style="text-align:center; color:#666;">
      Welcome to kisskh.fi. Find and download your apps easily.
    </p>
  </div>

  <footer>
    © 2026 kisskh.fi — All Rights Reserved
  </footer>

  <script>
    function searchApps() {
      let input = document.getElementById("searchBox")
        .value.toLowerCase();

      let cards = document.querySelectorAll(".card");

      cards.forEach(function(card) {
        let text = card.innerText.toLowerCase();

        if (text.includes(input)) {
          card.style.display = "block";
        } else {
          card.style.display = "none";
        }
      });
    }
  </script>

</body>
</html>
