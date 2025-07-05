<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Portfolio of Samuel Precious, Data Analyst specializing in Excel and Power BI">
  <meta name="keywords" content="data analyst, Power BI, Excel, data visualization">
  <meta name="author" content="Samuel Precious">
  <title>Samuel Precious - Data Analyst Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
  <style>
    * {
      box-sizing: border-box;
    }
    body {
      background: linear-gradient(135deg, #1e3c72, #2a5298);
      color: #ffffff;
      font-family: 'Roboto', sans-serif;
      margin: 0;
      padding: 0;
      line-height: 1.6;
    }
    .navbar {
      background: rgba(0, 0, 0, 0.8);
      padding: 15px 0;
      position: sticky;
      top: 0;
      z-index: 1000;
    }
    .navbar ul {
      list-style: none;
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: center;
      gap: 30px;
    }
    .navbar a {
      color: #ffffff;
      text-decoration: none;
      font-size: 1.1em;
      transition: color 0.3s ease;
    }
    .navbar a:hover {
      color: #00d4ff;
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
      gap: 40px;
      padding: 50px 0;
      background: url('https://images.unsplash.com/photo-1551288049-b1f3aaca3d75') no-repeat center/cover;
      border-radius: 12px;
      animation: fadeIn 1s ease-in;
    }
    .hero-text {
      flex: 1;
      min-width: 300px;
      text-align: left;
      padding: 20px;
      background: rgba(0, 0, 0, 0.6);
      border-radius: 8px;
    }
    .hero-image {
      flex: 1;
      min-width: 300px;
      text-align: center;
    }
    .profile-img {
      width: 300px;
      height: 300px;
      border-radius: 50%;
      border: 5px solid #00d4ff;
      box-shadow: 0 8px 16px rgba(0, 0, 0, 0.5);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      object-fit: cover;
    }
    .profile-img:hover {
      transform: scale(1.05);
      box-shadow: 0 12px 24px rgba(0, 0, 0, 0.7);
    }
    .hero h1 {
      font-size: 2.8em;
      margin: 0;
      font-weight: 700;
      color: #ffffff;
    }
    .hero h2 {
      color: #00d4ff;
      font-size: 1.6em;
      margin: 10px 0;
      font-weight: 400;
    }
    .hero p {
      font-size: 1.1em;
      color: #e0e0e0;
      line-height: 1.8;
    }
    .section {
      padding: 60px 0;
    }
    h3 {
      color: #00d4ff;
      font-size: 2em;
      border-bottom: 2px solid #00d4ff;
      padding-bottom: 10px;
      margin-bottom: 30px;
      display: inline-block;
    }
    .skills-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }
    .skill {
      text-align: center;
      padding: 20px;
      background: rgba(255, 255, 255, 0.1);
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    .skill:hover {
      transform: translateY(-5px);
      box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
    }
    .skill i {
      font-size: 50px;
      color: #00d4ff;
      margin-bottom: 15px;
    }
    .skill h4 {
      color: #ffffff;
      font-size: 1.3em;
      font-weight: 700;
      margin-bottom: 10px;
    }
    .skill p {
      color: #e0e0e0;
      font-size: 1em;
    }
    .projects-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 30px;
    }
    .project {
      background: rgba(255, 255, 255, 0.1);
      padding: 25px;
      border-radius: 12px;
      border: 2px solid #00d4ff;
      box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      position: relative;
      overflow: hidden;
    }
    .project:hover {
      transform: scale(1.05);
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.5);
    }
    .project img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 8px;
      margin-bottom: 15px;
    }
    .project h4 {
      color: #ffffff;
      font-size: 1.8em;
      font-weight: 700;
      margin-bottom: 10px;
      text-align: center;
    }
    .project p {
      color: #e0e0e0;
      font-size: 1em;
      line-height: 1.6;
      margin-bottom: 15px;
      text-align: center;
    }
    .project .tools {
      color: #00d4ff;
      font-size: 0.9em;
      margin-bottom: 15px;
      text-align: center;
    }
    .project a {
      color: #00d4ff;
      text-decoration: none;
      display: block;
      text-align: center;
      margin-bottom: 10px;
      font-weight: 500;
    }
    .project a:hover {
      text-decoration: underline;
    }
    .project .btn {
      background: #00d4ff;
      color: #1e3c72;
      padding: 10px 20px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      text-align: center;
      display: block;
      margin: 0 auto;
      transition: background 0.3s ease;
    }
    .project .btn:hover {
      background: #00b7d4;
    }
    .contact-form {
      max-width: 600px;
      margin: 0 auto;
      background: rgba(255, 255, 255, 0.1);
      padding: 20px;
      border-radius: 8px;
    }
    .contact-form input, .contact-form textarea {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border: none;
      border-radius: 5px;
      background: rgba(255, 255, 255, 0.2);
      color: #ffffff;
      font-size: 1em;
    }
    .contact-form button {
      background: #00d4ff;
      color: #1e3c72;
      padding: 10px 20px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      transition: background 0.3s ease;
    }
    .contact-form button:hover {
      background: #00b7d4;
    }
    .blog-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 30px;
    }
    .blog-post {
      background: rgba(255, 255, 255, 0.1);
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      transition: transform 0.3s ease;
    }
    .blog-post:hover {
      transform: translateY(-5px);
    }
    .blog-post h4 {
      color: #ffffff;
      font-size: 1.5em;
      margin-bottom: 10px;
    }
    .blog-post p {
      color: #e0e0e0;
      font-size: 1em;
    }
    .blog-post a {
      color: #00d4ff;
      text-decoration: none;
      font-weight: 500;
    }
    .blog-post a:hover {
      text-decoration: underline;
    }
    @media (max-width: 768px) {
      .hero {
        flex-direction: column;
        text-align: center;
      }
      .hero-text, .hero-image {
        flex: 100%;
      }
      .profile-img {
        width: 250px;
        height: 250px;
      }
      .hero h1 {
        font-size: 2.2em;
      }
      .hero h2 {
        font-size: 1.4em;
      }
      .navbar ul {
        flex-direction: column;
        gap: 15px;
      }
      .skills-grid, .projects-grid, .blog-grid {
        grid-template-columns: 1fr;
      }
    }
    @media (max-width: 480px) {
      .profile-img {
        width: 200px;
        height: 200px;
      }
      .hero h1 {
        font-size: 1.8em;
      }
      .hero h2 {
        font-size: 1.2em;
      }
    }
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }
  </style>
</head>
<body>
  <nav class="navbar">
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#blog">Blog</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
  <div class="container">
    <div class="hero" id="home">
      <div class="hero-text">
        <h1>Hello, I'm Samuel Precious</h1>
        <h2>Transforming Data into Insights</h2>
        <p>As a passionate data analyst, I specialize in turning complex data into actionable insights using Excel and Power BI. My work focuses on solving real-world challenges like identifying sales trends, optimizing workflows, and uncovering customer insights. Let’s make your data tell a powerful story!</p>
      </div>
      <div class="hero-image">
        <img src="images/profile.jpg" alt="Samuel Precious" class="profile-img">
      </div>
    </div>
    <div class="section" id="skills">
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
          <i class="fas fa-lightbulb"></i>
          <h4>Business Intelligence</h4>
          <p>Building KPIs to track and boost business performance with actionable insights.</p>
        </div>
      </div>
    </div>
    <div class="section" id="projects">
      <h3>Projects</h3>
      <div class="projects-grid">
        <div class="project">
          <img src="images/sales-dashboard.jpg" alt="Sales Trends Dashboard">
          <h4>Sales Trends Dashboard</h4>
          <p>Analyzed sales data from 2009-2012 to identify trends and forecast performance, helping optimize inventory.</p>
          <p class="tools"><strong>Tools</strong>: Power BI, Excel</p>
          <a href="https://www.behance.net/gallery/210978159/Sales-Trends-Dashboard">View Dashboard</a>
          <a href="https://github.com/your-username/portfolio/raw/main/files/sales-trends.xlsx">Download Excel</a>
          <button class="btn" onclick="alert('Details: Built an interactive Power BI dashboard to visualize sales trends.')">View Details</button>
        </div>
        <div class="project">
          <img src="images/customer-behavior.jpg" alt="Customer Behavior Analysis">
          <h4>Customer Behavior Analysis</h4>
          <p>Segmented customers by purchase history to guide targeted marketing strategies, boosting engagement.</p>
          <p class="tools"><strong>Tools</strong>: Excel, Power BI</p>
          <a href="https://github.com/your-username/portfolio">View Report</a>
          <button class="btn" onclick="alert('Details: Used Power BI to segment customers and improve marketing ROI.')">View Details</button>
        </div>
        <div class="project">
          <img src="images/efficiency-report.jpg" alt="Operational Efficiency Report">
          <h4>Operational Efficiency Report</h4>
          <p>Identified workflow bottlenecks to improve efficiency by 10% using detailed data analysis.</p>
          <p class="tools"><strong>Tools</strong>: Excel</p>
          <a href="https://github.com/your-username/portfolio/raw/main/files/efficiency-report.xlsx">Download Report</a>
          <button class="btn" onclick="alert('Details: Conducted in-depth Excel analysis to streamline operations.')">View Details</button>
        </div>
      </div>
    </div>
    <div class="section" id="blog">
      <h3>Blog</h3>
      <div class="blog-grid">
        <div class="blog-post">
          <h4>Creating Impactful Dashboards in Power BI</h4>
          <p>Learn how to design interactive dashboards that communicate insights effectively.</p>
          <a href="https://medium.com/@your-username/power-bi-dashboards">Read More</a>
        </div>
        <div class="blog-post">
          <h4>Excel Tips for Data Cleaning</h4>
          <p>Discover essential Excel techniques for preparing clean and reliable datasets.</p>
          <a href="https://medium.com/@your-username/excel-data-cleaning">Read More</a>
        </div>
      </div>
    </div>
    <div class="section" id="contact">
      <h3>Contact</h3>
      <p>Ready to make your data work harder? Let’s connect!</p>
      <div class="contact-form">
        <input type="text" placeholder="Your Name" required>
        <input type="email" placeholder="Your Email" required>
        <textarea placeholder="Your Message" rows="5" required></textarea>
        <button type="button" onclick="alert('Thank you for your message! I’ll get back to you soon.')">Send Message</button>
      </div>
      <p><strong>Email</strong>: samuel.precious@example.com</p>
      <p><strong>LinkedIn</strong>: <a href="https://www.linkedin.com/in/your-profile">My Profile</a></p>
    </div>
  </div>
</body>
</html>
