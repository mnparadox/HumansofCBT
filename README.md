<!DOCTYPE html>
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
            line-height: 1.6;
        }

        /* Header */
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
    </style>
</head>
<body>
    <!-- Header -->
    <header class="header">
        <div class="banner">
            <h1>Welcome to HoC</h1>
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
</body>
</html>
