<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HoC Website</title>
    <style>
        /* Reset mặc định */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Body toàn trang */
        body {
            font-family: Arial, sans-serif;
        }
        /* header cho trang */
        .header {
            width: 100%;
            position: relative;
        }

        /* Banner */
        .banner {
            background-color: #4CAF50;
            color: white;
            text-align: center;
            padding: 30px 0;
        }

        .banner h1 {
            font-size: 2rem;
        }

        /* Navbar */
        .navbar {
            background-color: #333;
            overflow: hidden;
        }
        .navbar ul {
            list-style: none;
            display: flex;
            justify-content: center;
        }

        .navbar li {
            margin: 0 15px;
        }

        .navbar a {
            color: white;
            text-decoration: none;
            font-size: 1rem;
            padding: 10px 15px;
            display: inline-block;
            transition: background-color 0.3s ease;
        }

        .navbar a:hover {
            background-color: #575757;
            border-radius: 5px;
        }

        /* Container chính */
        .content-container {
            display: flex;
            justify-content: space-between;
            padding: 20px;
        }

        /* Slideshow chính bên trái */
        .slideshow-container {
            flex: 1.5;
            height: 60vh;
            margin-right: 20px;
            position: relative;
            overflow: hidden;
            border: 2px solid #ccc;
            border-radius: 10px;
        }

        .slides {
            width: 100%;
            height: 100%;
            display: none;
        }

        .slideshow-container img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .active {
            display: block;
        }

        /* Khung nhỏ bên phải */
        .side-container {
            flex: 1;
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        .small-box {
            flex: 1;
            height: 28vh;
            border: 2px solid #ccc;
            border-radius: 10px;
            overflow: hidden;
        }

        .small-box img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="header">
        <div class="banner">
            <h1 style="text-align: center; background-color: #4CAF50; color: white; padding: 20px;">Welcome to HoC</h1>
        </div>
         <nav class="navbar">
            <ul>
                <li><a href="#home">Trang chủ</a></li>
                <li><a href="#about">Về HoC</a></li>
                <li><a href="#projects">Dự án</a></li>
                <li><a href="#activities">Hoạt động</a></li>
                <li><a href="#team">Đội ngũ HoC</a></li>
            </ul>
        </nav>
    </header>

    <!-- Main Content -->
    <div class="content-container">
        <!-- Slideshow bên trái -->
        <div class="slideshow-container">
            <img src="https://via.placeholder.com/600x400" class="slides active" alt="Dự án 1">
            <img src="https://via.placeholder.com/600x400" class="slides" alt="Dự án 2">
            <img src="https://via.placeholder.com/600x400" class="slides" alt="Dự án 3">
        </div>

        <!-- Khung bên phải -->
        <div class="side-container">
            <div class="small-box">
                <img src="https://via.placeholder.com/300x200" alt="TikTok nổi bật">
            </div>
            <div class="small-box">
                <img src="https://via.placeholder.com/300x200" alt="Instagram nổi bật">
            </div>
        </div>
    </div>

    <!-- JavaScript for Slideshow -->
    <script>
        let slideIndex = 0;

        function showSlides() {
            let slides = document.querySelectorAll('.slides');
            slides.forEach(slide => slide.classList.remove('active'));
            slideIndex = (slideIndex + 1) % slides.length;
            slides[slideIndex].classList.add('active');
        }

        setInterval(showSlides, 3000); // Chuyển slide mỗi 3 giây
    </script>
</body>
</html>
