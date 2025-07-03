<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Data Analytics Consulting</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@600;800&family=Open+Sans:wght@300;500&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="assets/css/style.css">
</head>
<body>
  <header>
    <div class="container header-wrapper">
      <div class="logo">Data<span>Analytics</span></div>
      <nav>
        <ul class="nav">
          <li><a href="#" class="active">Home</a></li>
          <li><a href="#">Projects</a></li>
          <li><a href="#">Services</a></li>
          <li><a href="#">Blog</a></li>
          <li><a href="#">Contact</a></li>
        </ul>
        <div class="menu-toggle">&#9776;</div>
      </nav>
    </div>
  </header>

  <section class="hero">
    <div class="hero-overlay"></div>
    <div class="container hero-content">
      <h1>Unlock the Power of Your Data</h1>
      <p>Transform raw numbers into actionable insights that drive your business forward.</p>
      <a href="#" class="btn">Get Started</a>
    </div>
  </section>

  <section class="services container">
    <h2>Our Services</h2>
    <div class="services-grid">
      <div class="card"><i class="fas fa-chart-line"></i><h3>Data Analysis</h3></div>
      <div class="card"><i class="fas fa-chart-pie"></i><h3>Data Visualization</h3></div>
      <div class="card"><i class="fas fa-brain"></i><h3>Predictive Modeling</h3></div>
      <div class="card"><i class="fas fa-tablet-alt"></i><h3>Dashboard Creation</h3></div>
    </div>
  </section>

  <footer>
    <div class="container footer">
      <p>&copy; 2025 Data Analytics Consulting</p>
    </div>
  </footer>

  <script>
    document.querySelector('.menu-toggle').onclick = () =>
      document.querySelector('.nav').classList.toggle('active');
  </script>
  <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
</body>
</html>
