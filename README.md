<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HoC Gallery</title>
    <style>
        /* Reset cơ bản */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background-color: #121212;
            color: white;
            overflow-x: hidden;
        }

        /* Banner */
        .banner {
            width: 1470px;
            height: 340px;
            margin: 0 auto;
            position: relative;
            overflow: hidden;
            border-radius: 10px;
            background-color: black;
        }

        .slides-container {
            display: flex;
            width: 100%;
            height: 100%;
            position: relative;
            animation: slide 8s infinite;
        }

        .slide {
            min-width: 100%;
            height: 100%;
            transition: transform 1s ease-in-out;
        }

        .slide img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        /* Keyframes for animation */
        @keyframes slide {
            0%, 20% { transform: translateX(0); }
            25%, 45% { transform: translateX(-100%); }
            50%, 70% { transform: translateX(-200%); }
            75%, 100% { transform: translateX(0); }
        }

        .info {
            position: absolute;
            top: 10px;
            right: 20px;
            display: flex;
            gap: 15px;
            z-index: 10;
        }

        .info a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            padding: 5px 10px;
            background: rgba(0, 0, 0, 0.5);
            border-radius: 5px;
            transition: background-color 0.3s;
        }

        .info a:hover {
            background-color: rgba(255, 255, 255, 0.2);
        }

        /* Footer */
        .footer {
            width: 1470px;
            height: 340px;
            background-color: #191414;
            color: #ccc;
            text-align: center;
            line-height: 340px;
            margin: 0 auto;
        }
    </style>
</head>
<body>
    <!-- Banner -->
    <header class="banner">
        <div class="slides-container">
            <div class="slide"><img src="https://via.placeholder.com/1470x340" alt="Slide 1"></div>
            <div class="slide"><img src="https://via.placeholder.com/1470x340/ff7f7f" alt="Slide 2"></div>
            <div class="slide"><img src="https://via.placeholder.com/1470x340/7f7fff" alt="Slide 3"></div>
        </div>
        <div class="info">
            <a href="#about">Về HoC</a>
            <a href="#team">Đội ngũ</a>
            <a href="#gallery">Our Gallery</a>
        </div>
    </header>

    <!-- Main Content -->
    <main>
        <section id="about" class="section">
            <h2>Giới thiệu HoC</h2>
            <p>Humans of CBT là một cộng đồng dành cho việc kết nối và sáng tạo...</p>
        </section>
    </main>

    <!-- Footer -->
    <footer class="footer">
        <p>© 2024 HoC Club | Contact: hocclub@example.com</p>
    </footer>
</body>
</html>
