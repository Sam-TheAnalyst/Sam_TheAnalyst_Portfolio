<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Samuel Precious - Data Analyst Portfolio</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
  <style>
    body {
      background: linear-gradient(to right, #1a1a1a, #2c3e50);
      color: #ecf0f1;
      font-family: 'Arial', sans-serif;
      margin: 0;
      padding: 0;
    }
    .container {
      max-width: 1000px;
      margin: 0 auto;
      padding: 40px 20px;
    }
    .hero {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 30px;
      padding: 50px 0;
      animation: fadeIn 1s ease-in;
    }
    .hero-left {
      flex: 1;
      min-width: 250px;
      text-align: center;
    }
    .hero-right {
      flex: 1;
      min-width: 250px;
    }
    .profile-img {
      width: 250px;
      height: 250px;
      border-radius: 50%;
      border: 5px solid #3498db;
      box-shadow: 0 8px 16px rgba(0, 0, 0, 0.5);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    .profile-img:hover {
      transform: scale(1.05);
      box-shadow: 0 12px 24px rgba(0, 0, 0, 0.7);
    }
    h1 {
      color: #3498db;
      font-size: 2.5em;
      margin-bottom: 10px;
    }
    .hero-right h2 {
      color: #ecf0f1;
      font-size: 1.8em;
      margin-bottom: 20px;
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
   0
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
        <img src="images/profile.jpg" alt="Samuel Precious" class="profile-img">
      </div>
      <div class="hero-right">
        <h1>Samuel Precious</h1>
        <h2>The Data Analyst</h2>
      </div>
    </div>
    <div class="section">
      <h3>About Me</h3>
      <p>I'm Samuel Precious, a passionate data analyst who transforms complex data into clear, actionable insights. I create dynamic dashboards and reports that empower businesses to make smarter decisions. From uncovering sales trends to optimizing operations, my work drives results and tells compelling data stories.</p>
    </div>
    <div class="section">
      <h3>Skills</h3>
      <div class="skills-grid">
        <div class="skill">
          <i class="fas fa-chart-bar"></i>
          <h4>Data Visualization</h4>
          <p>Crafting interactive dashboards that bring data to life.</p>
        </div>
        <div class="skill">
          <i class="fas fa-calculator"></i>
          <h4>Data Analysis</h4>
          <p>Uncovering trends and insights through statistical analysis and modeling.</p>
        </div>
        <div class="skill">
          <i class="fas fa-filter"></i>
          <h4>Data Cleaning</h4>
          <p>Preparing accurate datasets using Power Query for reliable results.</p>
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
