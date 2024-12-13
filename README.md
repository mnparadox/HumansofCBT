<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Web Dài Cuộn Xuống</title>
    <style>
        /* CSS: Định dạng toàn bộ trang */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background-color: black;
            color: white;
            scroll-behavior: smooth;
        }

        /* Định dạng section */
        .section {
            width: 100%;
            height: 100vh; /* Chiều cao bằng màn hình */
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 20px;
        }

        /* Nền màu khác nhau cho từng section */
        #about { background-color: #1a1a1a; }
        #gallery { background-color: #333333; }
        #team { background-color: #4d4d4d; }
        #footer { background-color: #666666; }

        /* Button cuộn mượt */
        .scroll-button {
            margin-top: 20px;
            padding: 10px 20px;
            background-color: #4CAF50;
            color: white;
            border: none;
            cursor: pointer;
        }

        .scroll-button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <!-- Phần 1: Giới thiệu -->
    <section id="about" class="section">
        <h1>Welcome to HoC</h1>
        <p>Giới thiệu về Humans of CBT</p>
        <button class="scroll-button" onclick="scrollToSection('gallery')">Xem Gallery</button>
    </section>

    <!-- Phần 2: Gallery -->
    <section id="gallery" class="section">
        <h1>HoC's Gallery</h1>
        <p>Khám phá những khoảnh khắc đẹp!</p>
        <button class="scroll-button" onclick="scrollToSection('team')">Xem Đội Ngũ</button>
    </section>

    <!-- Phần 3: Our Team -->
    <section id="team" class="section">
        <h1>Our Team</h1>
        <p>Gặp gỡ các thành viên của chúng tôi.</p>
        <button class="scroll-button" onclick="scrollToSection('footer')">Liên hệ</button>
    </section>

    <!-- Phần 4: Footer -->
    <section id="footer" class="section">
        <h1>Contact Us</h1>
        <p>Email: hocclub@example.com | Phone: +84 123 456 789</p>
    </section>

    <!-- JavaScript -->
    <script>
        function scrollToSection(sectionId) {
            const section = document.getElementById(sectionId);
            section.scrollIntoView({ behavior: 'smooth' });
        }
    </script>
</body>
</html>
