<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Samuel Precious - Data Analyst Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
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
      display: inline-block;
    }
    .skills-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
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
      font-size: 48px;
      color: #00C4B4;
      margin-bottom: 15px;
    }
    .skill h4 {
      color: #00C4B4;
      font-size: 1.2em;
      font-weight: 700;
      margin-bottom: 15px;
    }
    .skill p {
      color: #bdc3c7;
      font-size: 1em;
      line-height: 1.5;
    }
    /* Portfolio Section Styles */
    .portfolio-section {
      background: #1A1A1A;
      padding: 40px 0;
    }
    .grid-container {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 30px;
      max-width: 900px;
      margin: 0 auto;
    }
    .project-item {
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    .project-card {
      background: rgba(255, 255, 255, 0.1);
      border-radius: 12px;
      border: 2px solid #00C4B4;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      width: 100%;
      max-width: 404px;
      overflow: hidden;
    }
    .iframe-wrapper {
      position: relative;
      padding-bottom: 78.2%; /* 316 / 404 */
      height: 0;
    }
    .iframe-wrapper iframe {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      border: none;
      overflow: hidden;
      scrolling: no;
    }
    .project-title {
      font-family: 'Montserrat', sans-serif;
      font-weight: 700;
      color: #FFFFFF;
      text-align: center;
      margin-top: 15px;
      font-size: 1.2em;
    }
    @media (max-width: 768px) {
      .grid-container {
        grid-template-columns: 1fr;
      }
    }
    /* Contact Section Styles */
    .contact-section {
      padding: 40px 0;
    }
    .contact-content {
      display: flex;
      gap: 40px;
      justify-content: space-between;
    }
    .contact-form {
      flex: 1;
      background: white;
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
      position: relative;
      transition: transform 0.3s ease;
    }
    .contact-form:hover {
      transform: translateY(-5px);
    }
    .contact-info {
      flex: 1;
      background: linear-gradient(135deg, #333 0%, #1A1A1A 100%);
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
      position: relative;
      transition: transform 0.3s ease;
    }
    .contact-info:hover {
      transform: translateY(-5px);
    }
    .contact-info::before {
      content: '';
      position: absolute;
      top: -15px;
      left: 50%;
      transform: translateX(-50%);
      width: 30px;
      height: 30px;
      background: #00C4B4;
      border-radius: 50%;
    }
    .form-group {
      margin-bottom: 25px;
    }
    .form-group label {
      display: block;
      margin-bottom: 8px;
      font-size: 0.9em;
      text-transform: uppercase;
      color: #333;
      font-weight: 700;
    }
    .form-group input, .form-group textarea {
      width: 100%;
      padding: 12px 0;
      border: none;
      border-bottom: 2px solid #333;
      background: transparent;
      color: #333;
      font-size: 1.1em;
      transition: border-color 0.3s ease;
    }
    .form-group input:focus, .form-group textarea:focus {
      border-bottom-color: #00C4B4;
      outline: none;
    }
    .form-group textarea {
      height: 120px;
      resize: vertical;
    }
    .form-group input::placeholder, .form-group textarea::placeholder {
      font-size: 1.1em;
      color: #888;
      font-family: 'Montserrat', sans-serif;
      font-weight: 400;
    }
    .btn-submit {
      background: #00C4B4;
      color: white;
      padding: 12px 30px;
      border: none;
      border-radius: 25px;
      cursor: pointer;
      font-size: 1.1em;
      font-weight: 700;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      transition: background 0.3s ease, transform 0.3s ease;
    }
    .btn-submit:hover {
      background: #00a899;
      transform: translateY(-2px);
    }
    .contact-list {
      list-style: none;
      padding: 0;
    }
    .contact-list li {
      margin-bottom: 20px;
      display: flex;
      align-items: center;
      font-size: 1.1em;
    }
    .contact-list i {
      margin-right: 15px;
      color: #00C4B4;
      font-size: 1.2em;
    }
    .social-icons {
      display: flex;
      gap: 15px;
      margin-top: 20px;
    }
    .social-icons a {
      color: #00C4B4;
      font-size: 1.5em;
      transition: color 0.3s ease;
      text-decoration: none;
    }
    .social-icons a:hover {
      color: #00a899;
    }
    @media (max-width: 768px) {
      .contact-content {
        flex-direction: column;
        gap: 30px;
      }
      .contact-info::before {
        top: -15px;
        left: 50%;
        transform: translateX(-50%);
      }
      .contact-form, .contact-info {
        flex: none;
        width: 100%;
      }
    }
    /* End of Contact Section Styles */
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
    .anchorjs-link {
      display: none !important;
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
          <i class="fas fa-lightbulb"></i>
          <h4>Business Intelligence</h4>
          <p>Building KPIs to track and boost business performance with actionable insights.</p>
        </div>
      </div>
    </div>
    <div class="section portfolio-section">
      <h3>Projects</h3>
      <div class="grid-container">
        <div class="project-item">
          <div class="project-card">
            <div class="iframe-wrapper">
              <iframe src="https://www.behance.net/embed/project/210978159?ilo0=1" allowfullscreen lazyload frameborder="0" allow="clipboard-write" refererPolicy="strict-origin-when-cross-origin" scrolling="no"></iframe>
            </div>
          </div>
          <h4 class="project-title">Sales Trends Dashboard</h4>
        </div>
        <div class="project-item">
          <div class="project-card">
            <div class="iframe-wrapper">
              <iframe src="https://www.behance.net/embed/project/200511787?ilo0=1" allowfullscreen lazyload frameborder="0" allow="clipboard-write" refererPolicy="strict-origin-when-cross-origin" scrolling="no"></iframe>
            </div>
          </div>
          <h4 class="project-title">Customer Behavior Analysis</h4>
        </div>
        <div class="project-item">
          <div class="project-card">
            <div class="iframe-wrapper">
              <iframe src="https://www.behance.net/embed/project/172419277?ilo0=1" allowfullscreen lazyload frameborder="0" allow="clipboard-write" refererPolicy="strict-origin-when-cross-origin" scrolling="no"></iframe>
            </div>
          </div>
          <h4 class="project-title">Project 3</h4>
        </div>
        <div class="project-item">
          <div class="project-card">
            <div class="iframe-wrapper">
              <iframe src="https://www.behance.net/embed/project/200509947?ilo0=1" allowfullscreen lazyload frameborder="0" allow="clipboard-write" refererPolicy="strict-origin-when-cross-origin" scrolling="no"></iframe>
            </div>
          </div>
          <h4 class="project-title">Project 4</h4>
        </div>
        <div class="project-item">
          <div class="project-card">
            <div class="iframe-wrapper">
              <iframe src="https://www.behance.net/embed/project/191472599?ilo0=1" allowfullscreen lazyload frameborder="0" allow="clipboard-write" refererPolicy="strict-origin-when-cross-origin" scrolling="no"></iframe>
            </div>
          </div>
          <h4 class="project-title">Project 5</h4>
        </div>
      </div>
    </div>
    <div class="section contact-section">
      <h3>Contact</h3>
      <div class="contact-content">
        <div class="contact-form">
          <p style="color: #555; font-size: 1em; text-transform: uppercase; margin-bottom: 25px;">Feel free to contact us any time. We will get back to you as soon as we can!</p>
          <form action="https://formspree.io/f/mgvybkjn" method="POST">
            <div class="form-group">
              <label for="name">Name</label>
              <input type="text" id="name" name="name" placeholder="Your Name" required>
            </div>
            <div class="form-group">
              <label for="email">Email</label>
              <input type="email" id="email" name="email" placeholder="Your Email" required>
            </div>
            <div class="form-group">
              <label for="message">Message</label>
              <textarea id="message" name="message" placeholder="Your Message" required></textarea>
            </div>
            <button type="submit" class="btn-submit">Send</button>
          </form>
        </div>
        <div class="contact-info">
          <h3 style="color: white; margin-bottom: 25px; font-size: 1.5em;">Get in Touch</h3>
          <ul class="contact-list">
            <li><i class="fas fa-envelope"></i> samuel.precious@example.com</li>
            <li><i class="fas fa-phone"></i> +123 456 7890</li>
            <li><i class="fas fa-map-marker-alt"></i> 123 Data Lane, Insight City</li>
            <li><i class="fas fa-clock"></i> Mon-Fri, 9:00 AM - 5:00 PM</li>
          </ul>
          <div class="social-icons">
            <a href="https://www.linkedin.com" target="_blank"><i class="fab fa-linkedin"></i></a>
            <a href="https://www.x.com" target="_blank"><i class="fab fa-x-twitter"></i></a>
            <a href="https://www.instagram.com" target="_blank"><i class="fab fa-instagram"></i></a>
            <a href="https://www.facebook.com" target="_blank"><i class="fab fa-facebook"></i></a>
          </div>
        </div>
      </div>
    </div>
  </div>
</body>
</html><!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Samuel Precious - Data Analyst Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
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
      display: inline-block;
    }
    .skills-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
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
      font-size: 48px;
      color: #00C4B4;
      margin-bottom: 15px;
    }
    .skill h4 {
      color: #00C4B4;
      font-size: 1.2em;
      font-weight: 700;
      margin-bottom: 15px;
    }
    .skill p {
      color: #bdc3c7;
      font-size: 1em;
      line-height: 1.5;
    }
    /* Portfolio Section Styles */
    .portfolio-section {
      background: #1A1A1A;
      padding: 40px 0;
    }
    .grid-container {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 30px;
      max-width: 900px;
      margin: 0 auto;
    }
    .project-item {
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    .project-card {
      background: rgba(255, 255, 255, 0.1);
      border-radius: 12px;
      border: 2px solid #00C4B4;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      width: 100%;
      max-width: 404px;
      overflow: hidden;
    }
    .iframe-wrapper {
      position: relative;
      padding-bottom: 78.2%; /* 316 / 404 */
      height: 0;
    }
    .iframe-wrapper iframe {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      border: none;
      overflow: hidden;
      scrolling: no;
    }
    .project-title {
      font-family: 'Montserrat', sans-serif;
      font-weight: 700;
      color: #FFFFFF;
      text-align: center;
      margin-top: 15px;
      font-size: 1.2em;
    }
    @media (max-width: 768px) {
      .grid-container {
        grid-template-columns: 1fr;
      }
    }
    /* Contact Section Styles */
    .contact-section {
      padding: 40px 0;
    }
    .contact-content {
      display: flex;
      gap: 40px;
      justify-content: space-between;
    }
    .contact-form {
      flex: 1;
      background: white;
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
      position: relative;
      transition: transform 0.3s ease;
    }
    .contact-form:hover {
      transform: translateY(-5px);
    }
    .contact-form::before {
      content: '';
      position: absolute;
      left: -15px;
      top: 50%;
      transform: translateY(-50%);
      width: 8px;
      height: 60px;
      background: #00C4B4;
      border-radius: 4px;
    }
    .contact-info {
      flex: 1;
      background: linear-gradient(135deg, #333 0%, #1A1A1A 100%);
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
      position: relative;
      transition: transform 0.3s ease;
    }
    .contact-info:hover {
      transform: translateY(-5px);
    }
    .contact-info::before {
      content: '';
      position: absolute;
      top: -15px;
      left: 50%;
      transform: translateX(-50%);
      width: 30px;
      height: 30px;
      background: #00C4B4;
      border-radius: 50%;
    }
    .form-group {
      margin-bottom: 25px;
    }
    .form-group label {
      display: block;
      margin-bottom: 8px;
      font-size: 0.9em;
      text-transform: uppercase;
      color: #333;
      font-weight: 700;
    }
    .form-group input, .form-group textarea {
      width: 100%;
      padding: 12px 0;
      border: none;
      border-bottom: 2px solid #333;
      background: transparent;
      color: #333;
      font-size: 1.1em;
      transition: border-color 0.3s ease;
    }
    .form-group input:focus, .form-group textarea:focus {
      border-bottom-color: #00C4B4;
      outline: none;
    }
    .form-group textarea {
      height: 120px;
      resize: vertical;
    }
    .btn-submit {
      background: #00C4B4;
      color: white;
      padding: 12px 30px;
      border: none;
      border-radius: 25px;
      cursor: pointer;
      font-size: 1.1em;
      font-weight: 700;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      transition: background 0.3s ease, transform 0.3s ease;
    }
    .btn-submit:hover {
      background: #00a899;
      transform: translateY(-2px);
    }
    .contact-list {
      list-style: none;
      padding: 0;
      display: flex;
      gap: 15px;
      flex-wrap: wrap;
    }
    .contact-list li {
      margin-bottom: 20px;
    }
    .contact-list i {
      margin-right: 0;
      color: #00C4B4;
      font-size: 1.5em;
      transition: color 0.3s ease;
    }
    .contact-list a {
      color: #00C4B4;
      text-decoration: none;
    }
    .contact-list a:hover i {
      color: #00a899;
    }
    @media (max-width: 768px) {
      .contact-content {
        flex-direction: column;
        gap: 30px;
      }
      .contact-form::before {
        left: 50%;
        top: -15px;
        transform: translateX(-50%);
        width: 60px;
        height: 8px;
        border-radius: 4px;
      }
      .contact-info::before {
        top: -15px;
        left: 50%;
        transform: translateX(-50%);
      }
      .contact-form, .contact-info {
        flex: none;
        width: 100%;
      }
      .contact-list {
        justify-content: center;
      }
    }
    /* End of Contact Section Styles */
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
    .anchorjs-link {
      display: none !important;
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
          <i class="fas fa-lightbulb"></i>
          <h4>Business Intelligence</h4>
          <p>Building KPIs to track and boost business performance with actionable insights.</p>
        </div>
      </div>
    </div>
    <div class="section portfolio-section">
      <h3>Projects</h3>
      <div class="grid-container">
        <div class="project-item">
          <div class="project-card">
            <div class="iframe-wrapper">
              <iframe src="https://www.behance.net/embed/project/210978159?ilo0=1" allowfullscreen lazyload frameborder="0" allow="clipboard-write" refererPolicy="strict-origin-when-cross-origin" scrolling="no"></iframe>
            </div>
          </div>
          <h4 class="project-title">Sales Trends Dashboard</h4>
        </div>
        <div class="project-item">
          <div class="project-card">
            <div class="iframe-wrapper">
              <iframe src="https://www.behance.net/embed/project/200511787?ilo0=1" allowfullscreen lazyload frameborder="0" allow="clipboard-write" refererPolicy="strict-origin-when-cross-origin" scrolling="no"></iframe>
            </div>
          </div>
          <h4 class="project-title">Customer Behavior Analysis</h4>
        </div>
        <div class="project-item">
          <div class="project-card">
            <div class="iframe-wrapper">
              <iframe src="https://www.behance.net/embed/project/172419277?ilo0=1" allowfullscreen lazyload frameborder="0" allow="clipboard-write" refererPolicy="strict-origin-when-cross-origin" scrolling="no"></iframe>
            </div>
          </div>
          <h4 class="project-title">Project 3</h4>
        </div>
        <div class="project-item">
          <div class="project-card">
            <div class="iframe-wrapper">
              <iframe src="https://www.behance.net/embed/project/200509947?ilo0=1" allowfullscreen lazyload frameborder="0" allow="clipboard-write" refererPolicy="strict-origin-when-cross-origin" scrolling="no"></iframe>
            </div>
          </div>
          <h4 class="project-title">Project 4</h4>
        </div>
        <div class="project-item">
          <div class="project-card">
            <div class="iframe-wrapper">
              <iframe src="https://www.behance.net/embed/project/191472599?ilo0=1" allowfullscreen lazyload frameborder="0" allow="clipboard-write" refererPolicy="strict-origin-when-cross-origin" scrolling="no"></iframe>
            </div>
          </div>
          <h4 class="project-title">Project 5</h4>
        </div>
      </div>
    </div>
    <div class="section contact-section">
      <h3>Contact</h3>
      <div class="contact-content">
        <div class="contact-form">
          <form action="https://formspree.io/f/mgvybkjn" method="POST">
            <div class="form-group">
              <label for="name">Name</label>
              <input type="text" id="name" name="name" placeholder="Your Name" required>
            </div>
            <div class="form-group">
              <label for="email">Email</label>
              <input type="email" id="email" name="email" placeholder="Your Email" required>
            </div>
            <div class="form-group">
              <label for="message">Message</label>
              <textarea id="message" name="message" placeholder="Your Message" required></textarea>
            </div>
            <button type="submit" class="btn-submit">Send</button>
          </form>
        </div>
        <div class="contact-info">
          <h3 style="color: white; margin-bottom: 25px; font-size: 1.5em;">Get in Touch</h3>
          <ul class="contact-list">
            <li><i class="fab fa-linkedin"><a href="[your-linkedin-profile]" style="display: block; width: 100%; height: 100%;"></a></i></li>
            <li><i class="fab fa-x"><a href="[your-x-profile]" style="display: block; width: 100%; height: 100%;"></a></i></li>
            <li><i class="fab fa-instagram"><a href="[your-instagram-profile]" style="display: block; width: 100%; height: 100%;"></a></i></li>
            <li><i class="fab fa-facebook"><a href="[your-facebook-profile]" style="display: block; width: 100%; height: 100%;"></a></i></li>
          </ul>
          <ul class="contact-list">
            <li><i class="fas fa-envelope"></i> samuel.precious@example.com</li>
            <li><i class="fas fa-phone"></i> +123 456 7890</li>
            <li><i class="fas fa-map-marker-alt"></i> 123 Data Lane, Insight City</li>
            <li><i class="fas fa-clock"></i> Mon-Fri, 9:00 AM - 5:00 PM</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</body>
</html>
