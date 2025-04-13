<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vanguard Digitals</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: #fff;
            color: #111;
        }

        header {
            background: #000;
            color: #fff;
            padding: 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: fixed;
            top: 0;
            width: 100%;
            z-index: 999;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.3);
        }

        header h1 {
            color: red;
        }

        nav a {
            color: #fff;
            margin-left: 20px;
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s;
        }

        nav a:hover {
            color: red;
        }

        section {
            padding: 100px 40px;
            min-height: 100vh;
        }

        .home {
            background: linear-gradient(135deg, #000, #004aad);
            color: #fff;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
        }

        .home h2 {
            font-size: 3em;
            margin-bottom: 20px;
            background: linear-gradient(90deg, red, blue);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .about {
            background: #f7f7f7;
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            justify-content: space-around;
        }

        .about-text {
            max-width: 600px;
            font-size: 1.1em;
            line-height: 1.6;
        }

        .about-images {
            position: relative;
        }

        .about-images img {
            width: 300px;
            height: auto;
            border-radius: 20px;
            box-shadow: 0 0 20px rgba(0, 0, 255, 0.5);
            animation: changeImg 8s infinite;
        }

        @keyframes changeImg {
            0%, 50% {
                content: url('uday.jpg');
            }
            51%, 100% {
                content: url('uday2.webp');
            }
        }

        .section-title {
            text-align: center;
            font-size: 2.5em;
            margin-bottom: 30px;
            color: #004aad;
        }

        .cards {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 30px;
        }

        .card {
            background: #fff;
            border-radius: 15px;
            padding: 30px;
            width: 280px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            position: relative;
        }

        .card:hover {
            transform: scale(1.05);
            box-shadow: 0 6px 20px rgba(0, 0, 0, 0.2);
        }

        .pricing .card:nth-child(1) { background: #ffe5e5; }
        .pricing .card:nth-child(2) { background: #e0f7ff; }
        .pricing .card:nth-child(3) { background: #e6ffe0; }

        .services .card:nth-child(odd) { background: #f0f8ff; }
        .services .card:nth-child(even) { background: #fff5f5; }

        .card h3 {
            margin-bottom: 10px;
            color: #004aad;
        }

        .card p {
            font-size: 1em;
            line-height: 1.4;
        }

        .cartoon {
            width: 80px;
            height: 80px;
            margin-top: 10px;
            animation: float 2s ease-in-out infinite;
        }

        @keyframes float {
            0% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0); }
        }

        .contact {
            background: #000;
            color: #fff;
            text-align: center;
        }

        .contact p {
            font-size: 1.1em;
            margin-bottom: 10px;
        }

        footer {
            background: #111;
            color: #ccc;
            text-align: center;
            padding: 20px;
        }
    </style>
</head>

<body>
    <header>
        <h1>Vanguard Digitals</h1>
        <nav>
            <a href="#home">Home</a>
            <a href="#about">About</a>
            <a href="#services">Services</a>
            <a href="#pricing">Pricing</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <section class="home" id="home">
        <h2>Welcome to Vanguard Digitals</h2>
        <p>Your Trusted SMMA Partner</p>
    </section>
    

    <section class="about" id="about">
        <div class="about-text">
            <h2 class="section-title">About Me</h2>
            <p>Hey! I’m the creator and strategist behind Vanguard Digitals. I specialize in helping businesses grow online with effective social media and marketing strategies. My mission is to craft content that connects and strategies that deliver results. As the owner and operator, I’m dedicated to making your brand shine digitally!</p>
        </div>
        <div class="about-images">
            <img src="images/uday1.jpg" alt="uday" style="border: 2px solid red; width: 300px;">
        </div>
    </section>
    
    <section class="services" id="services">
        <h2 class="section-title">Our Services</h2>
        <style>
            .service-icon {
              width: 100px; /* size ni ikkada adjust cheyyi */
              height: 100px;
              display: block;
              margin: 20px auto;
            }
          </style>
        <div class="cards">
            <div class="card">
                <h3>Social Media Management</h3>
                <p>We manage your social media pages, keep them active, and grow your audience.</p>
                <img src="images/ser2.svg" alt="Content Creation" class="service-icon">
            </div>
            <div class="card">
                <h3>Content Creation</h3>
                <p>We create high-quality posts, reels, and stories tailored for your brand.</p>
                <img src="images/ser1.svg" alt="Social Media Management" class="service-icon">
            </div>
            <div class="card">
                <h3>Strategy & Planning</h3>
                <p>Custom marketing strategies designed to boost engagement and sales.</p>
                <img src="images/ser3.svg" alt="Strategy & Planning" class="service-icon">
            </div>
            <div class="card">
                <h3>Facebook/Instagram Ads</h3>
                <p>We set up and optimize ads for maximum reach and conversions.</p>
                <img src="images/ser4.svg" alt="Ads Service" class="service-icon">
            </div>
            <div class="card">
                <h3>Analytics & Reporting</h3>
                <p>Track your performance with detailed reports and insights.</p>
                <img src="images/ser5.svg" alt="Analytics" class="service-icon">
            </div>
        </div>
    </section>
    <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vanguard Digitals</title>
    <style>
        /* General Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: #fff;
            color: #111;
        }
        
        /* Our Works Section Styles */
        .our-works {
            background: #f4f4f4;
            padding: 80px 20px;
            text-align: center;
            overflow: hidden;
        }
        
        .scroll-container {
            width: 100%;
            overflow: hidden;
            position: relative;
        }

        .scroll-track {
            display: flex;
            gap: 30px;
            animation: scrollLeft 30s linear infinite;
        }

        .project-card {
            min-width: 250px;
            height: 200px;
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 0 20px #999;
            transition: transform 0.3s;
        }

        .project-card img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .project-card:hover {
            transform: scale(1.05);
        }

        /* Glow Effect for Different Cards */
        .glow-red {
            box-shadow: 0 0 20px red;
        }

        .glow-blue {
            box-shadow: 0 0 20px blue;
        }

        .glow-green {
            box-shadow: 0 0 20px green;
        }

        .glow-yellow {
            box-shadow: 0 0 20px yellow;
        }

        .glow-pink {
            box-shadow: 0 0 20px pink;
        }

        /* Animation for Infinite Scroll */
        @keyframes scrollLeft {
            0% {
                transform: translateX(0);
            }
            100% {
                transform: translateX(-50%);
            }
        }

        /* Section Title */
        .section-title {
            font-size: 2.5em;
            margin-bottom: 30px;
            color: #004aad;
        }
    </style>
</head>
<body>

    <body>

        <!-- Our Works Section -->
        <section class="our-works" id="our-works">
            <h2 class="section-title">Our Works</h2>
            <div class="scroll-container">
                <div class="scroll-track">
                    <!-- Cards with your images -->
                    <div class="project-card glow-red">
                        <img src="images/apoorva.png" alt="Restaurant Post">
                    </div>
                    <div class="project-card glow-blue">
                        <img src="images/swad.png" alt="Restaurant Post">
                    </div>
                    <div class="project-card glow-green">
                        <img src="images/gym.png" alt="Gym Post">
                    </div>
                    <div class="project-card glow-yellow">
                        <img src="images/rameshwaram.png" alt="Restaurant Post">
                    </div>
                    <div class="project-card glow-pink">
                        <img src="images/saloon.png" alt="Beauty Parlour Post">
                    </div>
    
                    <!-- Duplicate Cards for Infinite Loop -->
                    <div class="project-card glow-red">
                        <img src="images/apoorva.png" alt="Restaurant Post">
                    </div>
                    <div class="project-card glow-blue">
                        <img src="images/swad.png" alt="Restaurant Post">
                    </div>
                    <div class="project-card glow-green">
                        <img src="images/gym.png" alt="Gym Post">
                    </div>
                    <div class="project-card glow-yellow">
                        <img src="images/rameshwaram.png" alt="Restaurant Post">
                    </div>
                    <div class="project-card glow-pink">
                        <img src="images/saloon.png" alt="Beauty Parlour Post">
                    </div>
                </div>
            </div>
        </section>
    
    </body>
    
</html>


    <section class="pricing" id="pricing">
        <h2 class="section-title">Pricing</h2>
        <div class="cards">
            <div class="card">
                <h3>Basic Plan</h3>
                <p>₹3,000/month<br>8–10 posts/month<br>Captions + Hashtags<br>Weekly engagement</p>
            </div>
            <div class="card">
                <h3>Growth Plan</h3>
                <p>₹4,500/month<br>12–15 posts/month<br>Reels + Highlights<br>Strategy Call<br>Page Optimization</p>
            </div>
            <div class="card">
                <h3>Add-Ons</h3>
                <p>Logo Design: ₹500–₹1000<br>Landing Page: ₹2500–₹3000</p>
            </div>
        </div>
    </section>
<section class="contact" id="contact">
  <style>
    .contact {
      background: #0f0f0f;
      padding: 60px 20px;
      text-align: center;
      color: #fff;
      position: relative;
      overflow: hidden;
    }

    .contact h2 {
      font-size: 2.5rem;
      margin-bottom: 20px;
      color: #00ffff;
      text-shadow: 0 0 10px #00ffff;
    }

    .glow-text a {
      font-size: 1.2rem;
      color: #ffffff;
      text-decoration: none;
      display: inline-block;
      margin: 10px 0;
      padding: 5px 10px;
      border-radius: 6px;
      background: rgba(255, 255, 255, 0.1);
      box-shadow: 0 0 10px #00f7ff, 0 0 20px #00f7ff, 0 0 30px #00f7ff;
      transition: transform 0.3s ease;
    }

    .glow-text a:hover {
      transform: scale(1.05);
      box-shadow: 0 0 15px #ff0055, 0 0 25px #ff0055, 0 0 35px #ff0055;
    }

    .rocket {
      position: absolute;
      width: 60px;
      top: 30%;
      left: -100px;
      animation: flyRocket 10s linear infinite;
      z-index: 2;
    }

    .smoke {
      position: absolute;
      width: 20px;
      height: 20px;
      background: rgba(255, 255, 255, 0.2);
      border-radius: 50%;
      top: 35%;
      left: -120px;
      z-index: 1;
      animation: smokeTrail 10s linear infinite;
      filter: blur(6px);
    }

    @keyframes flyRocket {
      0% {
        transform: rotate(45deg);
        top: 30%;
        left: -100px;
      }
      50% {
        transform: rotate(45deg);
        top: 20%;
        left: 50%;
      }
      100% {
        transform: rotate(45deg);
        top: 10%;
        left: 120%;
      }
    }

    @keyframes smokeTrail {
      0% {
        top: 35%;
        left: -120px;
        opacity: 0.5;
      }
      50% {
        top: 25%;
        left: 45%;
        opacity: 0.2;
      }
      100% {
        top: 15%;
        left: 118%;
        opacity: 0;
      }
    }
  </style>

  <h2>Contact Us</h2>
  <p class="glow-text">
    <a href="mailto:udaysankar2005@gmail.com">📧 udaysankar2005@gmail.com</a>
  </p>
  <p class="glow-text">
    <a href="tel:8179893267">📞 8179893267</a>
  </p>
</section>

    

    <footer>
        <p>© 2025 Vanguard Digitals. All rights reserved.</p>
    </footer>
</body>

</html>
