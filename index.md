<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Samuel Precious - Data Analyst Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body {
      background: #1A1A1A;
      color: #ecf0f1;
      font-family: 'Montserrat', sans-serif;
      margin: 0;
      padding: 0;
    }
    .container {
      max-width: 1000px;
      margin: 0 auto;
      padding: 30px 20px;
    }
    .hero {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 40px;
      padding: 30px 0;
      animation: fadeIn 1s ease-in;
    }
    .hero-text {
      flex: 1;
      min-width: 200px;
      text-align: left;
    }
    .hero-image {
      flex: 1;
      min-width: 200px;
      text-align: center;
    }
    .profile-img {
      width: 350px;
      height: 350px;
      border-radius: 50%;
      border: 5px solid #00C4B4;
      box-shadow: 0 8px 16px rgba(0, 0, 0, 0.5);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      object-fit: cover;
      display: block;
      margin: 0 auto;
    }
    .profile-img:hover {
      transform: scale(1.05);
      box-shadow: 0 12px 24px rgba(0, 0, 0, 0.7);
    }
    .hero h1 {
      color: #FFFFFF;
      font-size: 3em;
      margin: 0;
      font-weight: 700;
      border-bottom: none;
    }
    .hero h2 {
      color: #00C4B4;
      font-size: 1.8em;
      margin: 10px 0;
      font-weight: 400;
      border-bottom: none;
    }
    .hero p {
      color: #bdc3c7;
      font-size: 1.1em;
      line-height: 1.6;
      margin: 10px 0;
    }
    .section {
      padding: 40px 0;
    }
    h3 {
      color: #00C4B4;
      font-size: 1.8em;
      border-bottom: 2px solid #00C4B4;
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
      color: #00C4B4;
      margin-bottom: 10px;
    }
    .skill h4 {
      color: #00C4B4;
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
      color: #00C4B4;
      font-size: 1.5em;
      margin-bottom: 15px;
    }
    a {
      color: #00C4B4;
      text-decoration: none;
    }
    a:hover {
      text-decoration: none;
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
      }
      .hero-text, .hero-image {
        flex: 100%;
        text-align: left;
      }
      .profile-img {
        width: 300px;
        height: 300px;
      }
      .hero h1 {
        font-size: 2.5em;
      }
      .hero h2 {
        font-size: 1.5em;
      }
      .skills-grid {
        grid-template-columns: repeat(2, 1fr);
      }
    }
    @media (max-width: 480px) {
      .profile-img {
        width: 250px;
        height: 250px;
      }
      .hero h1 {
        font-size: 2em;
      }
      .hero h2 {
        font-size: 1.2em;
      }
      .skills-grid {
        grid-template-columns: 1fr;
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
      <div class="hero-text">
        <h1>Hello I'm Samuel Precious</h1>
        <h2>Your Data Analyst</h2>
        <p>As a data analyst, I specialize in transforming complex data into clear, actionable insights using Excel and Power BI. My work solves challenges like identifying sales trends, optimizing workflows, and uncovering customer insights. By understanding data’s purpose, I deliver solutions that empower businesses to make informed decisions and drive growth.</p>
      </div>
      <div class="hero-image">
        <img src="images/profile.jpg" alt="Samuel Precious" class="profile-img">
        <!-- If your image has a different name, update the src attribute, e.g., src="images/samuel-profile.png" -->
      </div>
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
