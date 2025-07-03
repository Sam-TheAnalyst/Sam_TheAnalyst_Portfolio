<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Data Analytics Consulting - Home</title>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&family=Open+Sans:wght@300;400;600&display=swap" rel="stylesheet">
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.15.4/css/all.css" integrity="sha384-dyB7Q2I0yOxpoDlKa9vE6o6ftqau9FAQ8m1R9JyI57Hkf3RUIu30lRQ1X2wR7B3M" crossorigin="anonymous">
    <link rel="stylesheet" href="assets/css/style.css">
</head>
<body>
    <header>
        <div class="container header-content">
            <div class="logo">Data<span class="logo-highlight">Analytics</span> Inc.</div>
            <nav>
                <ul class="nav-list">
                    <li><a href="index.html" class="active">Home</a></li>
                    <li><a href="projects.html">Projects</a></li>
                    <li><a href="services.html">Services</a></li>
                    <li><a href="blog.html">Blog</a></li>
                    <li><a href="contact.html">Contact</a></li>
                </ul>
                <div class="menu-toggle" id="mobile-menu"><i class="fas fa-bars"></i></div>
            </nav>
        </div>
    </header>
    <section class="hero">
        <div class="container">
            <h1>Unlock the Power of Your Data</h1>
            <p>Expert data analytics consulting to help your business make data-driven decisions.</p>
            <a href="contact.html" class="btn">Get Started</a>
        </div>
    </section>
    <section class="intro container">
        <h2>Who We Are</h2>
        <p>We are a team of data analysts and consultants dedicated to turning raw data into meaningful insights. With experience in multiple industries, we help you visualize, model, and interpret your data to drive strategic decision-making.</p>
    </section>
    <section class="services-preview container">
        <h2>Our Services</h2>
        <div class="services-grid">
            <div class="service-card">
                <i class="fas fa-chart-line fa-3x"></i>
                <h3>Data Analysis</h3>
                <p>Analyze and interpret your data to uncover trends, patterns, and insights that drive business growth.</p>
            </div>
            <div class="service-card">
                <i class="fas fa-chart-pie fa-3x"></i>
                <h3>Data Visualization</h3>
                <p>Create compelling charts and visualizations that make your data easy to understand and share.</p>
            </div>
            <div class="service-card">
                <i class="fas fa-brain fa-3x"></i>
                <h3>Predictive Modeling</h3>
                <p>Build predictive models and machine learning solutions to forecast outcomes and optimize performance.</p>
            </div>
            <div class="service-card">
                <i class="fas fa-tablet-alt fa-3x"></i>
                <h3>Dashboard Development</h3>
                <p>Design interactive dashboards and reports to monitor key metrics and make informed decisions in real-time.</p>
            </div>
        </div>
        <a href="services.html" class="btn">View All Services</a>
    </section>
    <section class="projects-preview container">
        <h2>Featured Projects</h2>
        <div class="projects-grid">
            <div class="project-card">
                <img src="https://via.placeholder.com/600x400?text=Sales+Dashboard" alt="Sales Dashboard Project">
                <h3>Sales Performance Dashboard</h3>
                <p>An interactive dashboard to track and visualize sales KPIs for a retail business.</p>
            </div>
            <div class="project-card">
                <img src="https://via.placeholder.com/600x400?text=Customer+Analysis" alt="Customer Analysis Project">
                <h3>Customer Segmentation Analysis</h3>
                <p>Clustering analysis to segment customers based on purchasing behavior and demographics.</p>
            </div>
            <div class="project-card">
                <img src="https://via.placeholder.com/600x400?text=Market+Trend" alt="Market Trend Forecast Project">
                <h3>Market Trend Forecast</h3>
                <p>Predictive modeling project to forecast market trends using historical data and machine learning.</p>
            </div>
        </div>
        <a href="projects.html" class="btn">View All Projects</a>
    </section>
    <footer>
        <div class="container footer-content">
            <p>&copy; 2025 Data Analytics Consulting. All rights reserved.</p>
        </div>
    </footer>
    <script>
        // Mobile menu toggle script
        const menuToggle = document.getElementById('mobile-menu');
        const navList = document.querySelector('.nav-list');
        menuToggle.addEventListener('click', () => {
            navList.classList.toggle('active');
        });
    </script>
</body>
</html>
