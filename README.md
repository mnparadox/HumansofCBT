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

        /* Body */
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
            background: linear-gradient(45deg, #1DB954, #191414);
            position: relative;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px;
        }

        .banner .info {
            position: absolute;
            top: 10px;
            right: 20px;
            display: flex;
            gap: 15px;
        }

        .banner .info a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            padding: 5px 10px;
            border-radius: 5px;
            transition: background-color 0.3s;
        }

        .banner .info a:hover {
            background-color: rgba(255, 255, 255, 0.2);
        }

        .highlight-image img {
            width: 300px;
            height: 300px;
            border-radius: 15px;
            cursor: grab;
        }

        /* Main Content */
        .section {
            padding: 20px;
            width: 1470px;
            margin: 0 auto;
        }

        .section h2 {
            font-size: 1.5rem;
            margin-bottom: 10px;
        }

        .gallery {
            display: flex;
            gap: 15px;
        }

        .gallery img {
            width: 300px;
            height: 300px;
            object-fit: cover;
            border-radius: 10px;
            transition: transform 0.3s ease;
        }

        .gallery img:hover {
            transform: scale(1.05);
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
        <div class="info">
            <a href="#about">Về HoC</a>
            <a href="#team">Đội ngũ</a>
            <a href="#gallery">Our Gallery</a>
        </div>
        <div class="highlight-image">
            <img src="https://via.placeholder.com/300" alt="Highlight">
        </div>
    </header>

    <!-- Main Content -->
    <main>
        <section id="about" class="section">
            <h2>Giới thiệu HoC</h2>
            <p>Humans of CBT là một cộng đồng dành cho việc kết nối và sáng tạo...</p>
        </section>
        <section id="projects" class="section">
            <h2>Sản phẩm nổi bật</h2>
            <div class="gallery">
                <img src="https://via.placeholder.com/300" alt="Product 1">
                <img src="https://via.placeholder.com/300" alt="Product 2">
                <img src="https://via.placeholder.com/300" alt="Product 3">
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="footer">
        <p>© 2024 HoC Club | Contact: hocclub@example.com</p>
    </footer>

    <!-- JavaScript -->
    <script>
        const highlightImage = document.querySelector('.highlight-image img');
        highlightImage.addEventListener('mousedown', (e) => {
            highlightImage.style.cursor = 'grabbing';
            highlightImage.style.position = 'absolute';

            const moveAt = (pageX, pageY) => {
                highlightImage.style.left = `${pageX - highlightImage.offsetWidth / 2}px`;
                highlightImage.style.top = `${pageY - highlightImage.offsetHeight / 2}px`;
            };

            moveAt(e.pageX, e.pageY);

            const onMouseMove = (event) => {
                moveAt(event.pageX, event.pageY);
            };

            document.addEventListener('mousemove', onMouseMove);

            document.onmouseup = () => {
                document.removeEventListener('mousemove', onMouseMove);
                highlightImage.style.cursor = 'grab';
                document.onmouseup = null;
            };
        });
    </script>
</body>
</html>
