<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rocket Animation</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: black;
            font-family: Arial, sans-serif;
        }

        /* Navigation Bar */
        nav {
            background-color: #222;
            padding: 20px 40px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        nav h2 {
            color: white;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 25px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-size: 16px;
            transition: 0.3s;
        }

        nav ul li a:hover {
            color: blue;
        }

        /* Rocket Section */
        .container {
            height: 85vh;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .rocket {
            font-size: 80px;
            animation: fly 2s infinite ease-in-out;
        }

        @keyframes fly {
            0% {
                transform: translateY(0);
            }

            50% {
                transform: translateY(-100px);
            }

            100% {
                transform: translateY(0);
            }
        }

        /* Responsive Navigation */
        @media (max-width: 600px) {
            nav {
                padding: 20px;
                flex-direction: column;
                gap: 15px;
            }

            nav ul {
                gap: 15px;
                flex-wrap: wrap;
                justify-content: center;
            }
        }
    </style>
</head>

<body>

    <nav>
        <h2>🚀 Rocket</h2>

        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#services">Services</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <div class="container" id="home">
        <div class="rocket">🚀</div>
    </div>

</body>
</html>
