<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Humans of CBT</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600&display=swap" rel="stylesheet">
    <style>
        /* Import font Montserrat từ Google Fonts */
        @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600&display=swap');

        /* Reset CSS cơ bản */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Áp dụng font toàn bộ trang */
        body {
            font-family: 'Montserrat', sans-serif;
            background-color: #fff;
            color: #333;
        }

        /* Điều chỉnh cho Navigation Bar */
        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background-color: #111;
            padding: 10px 20px;
        }

        .nav-logo {
            font-size: 24px;
            color: #fff;
            font-weight: 600;
        }

        .nav-links {
            list-style: none;
            display: flex;
        }

        .nav-links li {
            margin-left: 20px;
        }

        .nav-links a {
            text-decoration: none;
            color: #fff;
            font-size: 16px;
            font-weight: 500;
            transition: color 0.3s ease;
        }

        .nav-links a:hover {
            color: #ff9f00;
        }

        /* Section Poster */
        .poster {
            background: url('poster-background.jpg') no-repeat center center/cover;
            color: #fff;
            text-align: center;
            padding: 100px 20px;
        }

        .poster h1 {
            font-size: 48px;
            margin-bottom: 20px;
        }

        .poster p {
            font-size: 20px;
            font-weight: 400;
        }

        /* About HoC Section */
        .about {
            padding: 60px 20px;
            background-color: #f4f4f4;
            text-align: center;
        }

        .about h2 {
            font-size: 36px;
            margin-bottom: 20px;
        }

        .about p {
            font-size: 18px;
            color: #666;
            max-width: 800px;
            margin: 0 auto;
        }

        /* HoC Gallery Section */
        .gallery {
            padding: 60px 20px;
            background-color: #fff;
            text-align: center;
        }

        .gallery h2 {
            font-size: 36px;
            margin-bottom: 30px;
        }

        .gallery-content {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 20px;
        }

        .gallery .vertical-image {
            width: 300px;
            height: 500px;
            object-fit: cover;
            border-radius: 10px;
        }

        .gallery .horizontal-images {
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        .gallery .horizontal-images img {
            width: 300px;
            height: 200px;
            object-fit: cover;
            border-radius: 10px;
        }

        /* HoC Projects Section */
        .projects {
            padding: 60px 20px;
            background-color: #f4f4f4;
            text-align: center;
        }

        .projects h2 {
            font-size: 36px;
            margin-bottom: 30px;
        }

        .project-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
            gap: 30px;
        }

        .project-info {
            max-width: 500px;
            text-align: left;
        }

        .project-info h3 {
            font-size: 28px;
            margin-bottom: 10px;
        }

        .project-info p {
            font-size: 18px;
            color: #666;
        }

        .project-video {
            position: relative;
            max-width: 600px;
        }

        .project-video video {
            width: 100%;
            border-radius: 10px;
        }

        .project-video .overlay {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            color: #fff;
            font-size: 24px;
            font-weight: 600;
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .project-video:hover .overlay {
            opacity: 1;
        }

        /* Our Team Section */
        .team {
            padding: 60px 20px;
            background-color: #fff;
            text-align: center;
        }

        .team h2 {
            font-size: 36px;
            margin-bottom: 30px;
        }

        .team-members {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 30px;
        }

        .member {
            text-align: center;
        }

        .member img {
            width: 150px;
            height: 150px;
            object-fit: cover;
            border-radius: 50%;
            margin-bottom: 10px;
        }

        .member p {
            font-size: 16px;
            font-weight: 500;
        }

        /* Footer Section */
        .footer {
            background-color: #111;
            color: #fff;
            padding: 40px 20px;
            text-align: center;
        }

        .footer-logo {
            font-size: 24px;
            margin-bottom: 20px;
            font-weight: 600;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
        }

        .social-links a {
            text-decoration: none;
            color: #fff;
            font-size: 18px;
            transition: color 0.3s ease;
        }

        .social-links a:hover {
            color: #ff9f00;
        }
    </style>
</head>
<body>
    <!-- Navigation Bar -->
    <nav class="navbar">
        <div class="nav-logo">HoC Logo</div>
        <ul class="nav-links">
            <li><a href="#about">About HoC</a></li>
            <li><a href="#gallery">HoC Gallery</a></li>
            <li><a href="#projects">HoC Project</a></li>
            <li><a href="#team">Our Team</a></li>
            <li><a href="#footer">Footer</a></li>
        </ul>
    </nav>

    <!-- Poster Section -->
    <header class="poster">
        <h1>Welcome to HoC Club</h1>
        <p>Inspiring Creativity and Innovation</p>
    </header>

    <!-- About HoC Section -->
    <section id="about" class="about">
        <h2>About HoC</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Discover the story of our club and our mission to empower creativity and innovation.</p>
    </section>

    <!-- HoC Gallery Section -->
    <section id="gallery" class="gallery">
        <h2>Humans of CBT Gallery</h2>
        <div class="gallery-content">
            <img src="vertical.jpg" alt="Vertical Image" class="vertical-image">
            <div class="horizontal-images">
                <img src="horizontal1.jpg" alt="Horizontal Image 1">
                <img src="horizontal2.jpg" alt="Horizontal Image 2">
                <img src="horizontal3.jpg" alt="Horizontal Image 3">
            </div>
        </div>
    </section>

    <!-- HoC Projects Section -->
    <section id="projects" class="projects">
        <h2>HoC Project</h2>
        <div class="project-content">
            <div class="project-info">
                <h3>Project Name</h3>
                <p>Purpose: To showcase our commitment to innovation and teamwork.</p>
                <p>Production Date: <span>January 2025</span></p>
                <p>Team: <span>Team HoC</span></p>
            </div>
            <div class="project-video">
                <video src="project-video.mp4" muted autoplay loop></video>
                <div class="overlay">Hover to see more!</div>
            </div>
        </div>
    </section>

    <!-- Our Team Section -->
    <section id="team" class="team">
        <h2>Our Team</h2>
        <div class="team-members">
            <div class="member">
                <img src="member1.jpg" alt="Team Member">
                <p>Member Name</p>
            </div>
            <div class="member">
                <img src="member2.jpg" alt="Team Member">
                <p>Member Name</p>
            </div>
            <!-- Add more members as needed -->
        </div>
    </section>

    <!-- Footer Section -->
    <footer id="footer" class="footer">
        <div class="footer-content">
            <div class="footer-logo">HoC Logo</div>
            <div class="social-links">
                <a href="#">Email</a>
                <a href="#">TikTok</a>
                <a href="#">Facebook</a>
                <a href="#">Instagram</a>
            </div>
        </div>
    </footer>
</body>
</html>
