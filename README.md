<!DOCTYPE html><html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aymiré - Luxury Fashion</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background-color: black;
            color: white;
            font-family: Arial, sans-serif;
            text-align: center;
        }
        header {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(0, 0, 0, 0.8);
            padding: 20px;
            font-size: 24px;
            transition: all 0.3s;
        }
        header.shrink {
            padding: 10px;
            background: rgba(20, 20, 20, 0.9);
            font-size: 18px;
        }
        .hero {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 50px;
            font-weight: bold;
        }
        video {
            width: 100%;
            height: auto;
        }
    </style>
</head>
<body>
    <header id="header">Aymiré</header>
    <div class="hero">Exclusive Fashion Awaits</div>
    <video autoplay muted loop>
        <source src="luxury-video.mp4" type="video/mp4">
        Your browser does not support the video tag.
    </video>
    <script>
        window.addEventListener("scroll", function() {
            let header = document.getElementById("header");
            if (window.scrollY > 50) {
                header.classList.add("shrink");
            } else {
                header.classList.remove("shrink");
            }
        });
    </script>
</body>
</html>
