<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bloom CoLive PG</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Arial Rounded MT', sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            background-color: #f9f9fb;
            color: #333;
            scroll-behavior: smooth;
        }
        body::-webkit-scrollbar {
            width: 12px;
        }
        body::-webkit-scrollbar-track {
            background: #f0f0f0;
            border-radius: 6px;
        }
        body::-webkit-scrollbar-thumb {
            background: linear-gradient(to bottom, #ffd700, #ff7f00);
            border-radius: 6px;
            border: 3px solid #f0f0f0;
        }
        header {
            background: #212121;
            color: #fff;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }
        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: #ffd700;
        }
        .nav-links {
            list-style: none;
            display: flex;
            gap: 1.5rem;
        }
        .nav-links a { color: #dfaf46;
            font-weight: 600;
            font-size: 0.9rem;
            transition: color 0.3s ease;
        }
        .nav-links a:hover {
            color: #ffd700;
        }
        #hero { background: linear-gradient(to bottom right, #ffd700, #fff8e1);
            min-height: 100vh;
            color: #1a1a1a;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 0 1rem;
            clip-path: polygon(0 0, 100% 0, 100% 85%, 0 100%);
        }
        #hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            animation: fadeIn 1.5s ease;
        }
        #hero p {
            font-size: 1.5rem;
            margin-bottom: 2rem;
            animation: fadeIn 2s ease;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        section {
            padding: 4rem 2rem;
            text-align: center;
        }
        section h2 {
            font-size: 2rem;
            margin-bottom: 1.5rem;
            color: #333;
            position: relative;
            display: inline-block;
        }
        section h2::after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background: #ffd700;
            margin: 0.5rem auto;
            border-radius: 2px;
        }
        section p, ul {
            font-size: 1rem;
            line-height: 1.6;
            color: #555;
            max-width: 800px;
            margin: 0 auto;
        }
        ul {
            list-style: none;
            padding: 0;
        }
        ul li {
            padding: 0.8rem;
            background: #fff;
            margin: 0.5rem 0;
            border-radius: 12px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        ul li:hover {
            transform: translateY(-5px);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
        }
        .room-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }
        .room {
            text-align: left;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            border-radius: 12px;
            overflow: hidden;
            background: #fffff;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .room:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
        }
        .room img {
            width: 100%;
            border-bottom: 4px solid #ffd700;
        }
        .room h3 {
            padding: 1.5rem;
            font-size: 1.5rem;
            color: #333;
        }
        .room p {
            padding: 0 1.5rem 1.5rem;
            font-size: 0.9rem;
            color: #555;
        }
        footer {
            background: #212121;
            color: #fff;
            padding: 2rem;
            text-align: center;
            box-shadow: 0 -4px 10px rgba(0, 0, 0, 0.1);
        }
        footer p {
            font-size: 1rem;
            margin: 0;
        }
        .contact-details {
            font-size: 1.1rem;
            line-height: 1.6;
            color: #555;
            margin-top: 2rem;
        }
        .contact-details strong {
            color: #333;
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">Bloom CoLive PG</div>
        <ul class="nav-links">
            <li><a href="#about">About</a></li>
            <li><a href="#amenities">Amenities</a></li>
            <li><a href="#rooms">Rooms</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </header>

    <section id="hero">
        <h1>Welcome to Bloom CoLive PG</h1>
        <p>Your next cozy and affordable stay awaits!</p>
    </section>

    <section id="about">
        <h2>About Us</h2>
        <p>Bloom CoLive PG offers comfortable and ventilated rooms. Our CoLive PG is all about convenience, affordability, and comfort.</p>
    </section>

    <section id="amenities">
        <h2>Amenities</h2>
        <ul>
            <li>High-Speed WiFi</li>
            <li>Security</li>
            <li>3 Times Food a Day</li>
            <li>Washing Machine</li>
            <li>Fridge</li>
            <li>Power Backup</li>
            <li>Elevator</li>
            <li>Hot Water</li>
        </ul>
    </section>

    <section id="rooms">
        <h2>Our Rooms</h2>
        <br>
        <div class="room-container">
            <div class="room">
                <img src=""C:\Users\Vidva\Downloads\2024-12-03 (1).jpg"" alt="Single Occupancy Room">
                <h3>Single Occupancy</h3>
                <p>Experience privacy and comfort with our single occupancy rooms.</p>
            </div>
            <div class="room">
                <img src="https://lh3.googleusercontent.com/p/AF1QipN_KEc-_B9uNyLlBqETHJRBO7d-93eLIjcHbS0f=s680-w680-h510" alt="Double Occupancy Room">
                <h3>Double Occupancy</h3>
                <p>Share your space with friends and family with our double occupancy rooms.</p>
            </div>
        </div>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <div class="contact-details">
            <p><strong>Phone:</strong> +91 9902444658</p>
            <p><strong>Email:</strong> BloomCoLivePG@gmail.com</p>
            <p><strong>Address:</strong> 04, 20th Cross, near sports Arena, Pragathi Layout, Doddanekundi, Bengaluru, Karnataka 560037</p>
        </div>
    </section>

    <footer>
        <p>Bloom CoLive PG</p>
    </footer>

</body>
</html>
