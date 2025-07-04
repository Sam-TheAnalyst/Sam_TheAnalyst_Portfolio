<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Samuel Precious - Data Analyst Portfolio</title>
  <link rel="stylesheet" href="[invalid url, do not cite]
  <style>
    body {
      background-color: #1A1A1A;
      color: #FFFFFF;
      font-family: 'Montserrat', sans-serif;
      margin: 0;
      padding: 0;
    }
    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 40px 20px;
    }
    .hero {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: center;
      gap: 40px;
      padding: 60px 0;
      animation: fadeIn 1s ease-in;
    }
    .hero-left {
      flex: 1;
      min-width: 300px;
      text-align: left;
    }
    .hero-right {
      flex: 1;
      min-width: 300px;
      position: relative;
      display: flex;
      justify-content: center;
      align-items: center;
    }
    .profile-img {
      width: 300px;
      height: 300px;
      border-radius: 50%;
      object-fit: cover;
      z-index: 2;
    }
    .circle {
      width: 400px;
      height: 400px;
      border-radius: 50%;
      background: radial-gradient(circle, #00D7A7, #00FFBF);
      position: absolute;
      z-index: 1;
    }
    h1 {
      font-size: 48px;
      font-weight: bold;
      margin: 0;
      line-height: 1.2;
    }
    h1 .small {
      font-size: 24px;
      font-weight: normal;
      display: block;
    }
    h2 {
      font-size: 36px;
      color: #00D7A7;
      margin: 10px 0;
      font-weight: normal;
    }
    .contact-btn {
      background-color: #FFC107;
      color: #000;
      padding: 12px 24px;
      border: none;
      border-radius: 5px;
      font-size: 16px;
      cursor: pointer;
      margin-top: 20px;
      transition: background-color 0.3s ease;
    }
    .contact-btn:hover {
      background-color: #FFB300;
    }
    .section {
      padding: 40px 0;
    }
    h3 {
      color: #3498db;
      font-size: 1.8em;
      border-bottom: 2px solid #3498db;
      padding-bottom: 10px;
      margin-bottom: 20px;
    }
    .skills-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 20px;
    }
    .skill {
      text-align: center;
      padding: 20px;
      background: rgba(255, 255, 255, 0.1);
      border-radius: 8px;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    .skill:hover {
      transform: translateY(-5px);
      box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
    }
    .skill i {
      font-size: 48px;
      color: #3498db;
      margin-bottom: 10px;
    }
    .skill h4 {
      color: #3498db;
      font-size: 1.2em;
      margin-bottom: 10px;
    }
    .skill p {
      color: #bdc3c7;
      font-size: 1em;
    }
    .project {
      background: rgba(255, 255, 255, 0.1);
      padding: 20px;
      border-radius: 8px;
      margin-bottom: 20px;
    }
    .project h4 {
      color: #3498db;
      font-size: 1.5em;
      margin-bottom: 15px;
    }
    a {
      color: #3498db;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }
    iframe {
      width: 100%;
      height: 400px;
      border-radius: 8px;
    }
    p, li {
      line-height: 1.6;
      font-size: 1.1em;
      color: #bdc3c7;
    }
    @media (max-width: 768px) {
      .hero {
        flex-direction: column;
        text-align: center;
      }
      .hero-left, .hero-right {
        flex: 100%;
      }
      .profile-img {
        width: 200px;
        height: 200px;
      }
      .circle {
        width: 300px;
        height: 300px;
      }
      h1 {
        font-size: 36px;
      }
      h1 .small {
        font-size: 18px;
      }
      h2 {
        font-size: 24px;
      }
    }
    @media (max-width: 480px) {
      .profile-img {
        width: 150px;
        height: 150px;
      }
      .circle {
        width: 250px;
        height: 250px;
      }
      h1 {
        font-size: 28px;
      }
      h1 .small {
        font-size: 14px;
      }
      h2 {
        font-size: 20px;
      }
    }
    @media (max-width: 1080px) {
      .skills-grid {
        grid-template-columns: repeat(3, 1fr);
      }
    }
    @media (max-width: 640px) {
      .skills-grid {
        grid-template-columns: repeat(2, 1fr);
      }
    }
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="hero">
      <div class="hero-left">
        <h1 class="small">Hello</h1>
        <h1>I'm Samuel Precious</h1>
        <h2>Your Data Analyst</h2>
        <button class="contact-btn">Contact Me</button>
      </div>
      <div class="hero-right">
        <div class="circle"></div>
        <img src="images/profile.jpg" alt="Samuel Precious" class="profile-img" <!-- CLUE: Replace this image path with your uploaded file path -->>
      </div>
    </div>
    <div class="section">
      <h3>About Me</h3>
      <p>I'm Samuel Precious, a passionate data analyst who transforms complex data into clear, actionable insights. Specializing in Excel and Power BI, I create dynamic dashboards and reports that empower businesses to make smarter decisions. From uncovering sales trends to optimizing operations, my work drives results and tells compelling data stories.</p>
    </div>
    <div class="section">
      <h3>Skills</h3>
      <div class="skills-grid">
        <div class="skill">
          <i class="fas fa-chart-bar"></i>
          <h4>Data Visualization</h4>
          <p>Crafting interactive dashboards in Power BI and Excel to bring data to life.</p>
        </div>
        <div class="skill">
          <i class="fas fa-calculator"></i>
          <h4>Data Analysis</h4>
          <p>Uncovering trends and insights through statistical analysis and modeling.</p>
        </div>
        <div class="skill">
          <i class="fas fa-filter"></i>
          <h4>Data Cleaning</h4>
          <p>Preparing accurate datasets using Excel and Power BI for reliable results.</p>
        </div>
        <div class="skill">
          <i class="fas fa-analytics"></i>
          <h4>Business Intelligence</h4>
          <p>Building KPIs to track and boost business performance with actionable insights.</p>
        </div>
      </div>
    </div>
    <div class="section">
      <h3>Projects</h3>
      <div class="project">
        <h4>Sales Trends Dashboard</h4>
        <p>Analyzed sales data from 2009-2012 to identify trends and forecast performance, helping optimize inventory.</p>
        <p><strong>Tools</strong>: Power BI, Excel</p>
        <p><a href="[your-power-bi-link-or-repo-folder]">View Dashboard</a> | <a href="[your-excel-file-link]">Download Excel</a></p>
        <!-- Replace with Power BI iframe if available -->
        <!-- <iframe src="[your-power-bi-iframe-url]" allowFullScreen="true"></iframe> -->
      </div>
      <div class="project">
        <h4>Customer Behavior Analysis</h4>
        <p>Segmented customers by purchase history to guide targeted marketing strategies, boosting engagement.</p>
        <p><strong>Tools</strong>: Excel, Power BI</p>
        <p><a href="[your-report-link-or-repo-folder]">View Report</a></p>
      </div>
      <div class="project">
        <h4>Operational Efficiency Report</h4>
        <p>Identified workflow bottlenecks to improve efficiency by 10% using detailed data analysis.</p>
        <p><strong>Tools</strong>: Excel</p>
        <p><a href="[your-excel-file-link]">Download Report</a></p>
      </div>
    </div>
    <div class="section">
      <h3>Contact</h3>
      <p>Ready to make your data work harder? Let’s connect!</p>
      <p><strong>Email</strong>: [your-email@example.com]</p>
      <p><strong>LinkedIn</strong>: <a href="[your-linkedin-profile]">My Profile</a></p>
    </div>
  </div>
</body>
</html>
