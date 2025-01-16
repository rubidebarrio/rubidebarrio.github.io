---
layout: base
permalink: /
---

<link rel="stylesheet" href="styles/index.css">
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta property="og:image" content="assets\tablero_cluedo.png"/>
    <meta property="twitter:image" content="assets\tablero_cluedo.png"/>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rubi de Barrio</title>
    <link rel="icon" type="image/png" href="assets/favicon_estrellita.png">
    <link rel="shortcut icon" id="favicon" type="image/png" href="assets/favicon_estrellita.png">
    

    <style>
        #video-container {
            display: none;
        }
        main {
            margin: 100px 0;
        }

        h1 {
            text-align: center;
            font-family: 'Courier New', Courier, monospace;
            font-size: 2em;
            color: #ff0000;
            padding: 1em 0;
        }
    </style>
</head>


<body>

    
    <h1>El bodegón más vistoso en bucle</h1>

    <div>
        <div id="password-container">
            <input type="password" id="password" placeholder="Enter password">
            <button onclick="checkPassword()">Submit</button>
        </div>
        <div id="video-container"> 
            <iframe
                max-width="560" height="315" frameborder="0" allowfullscreen
                iv_load_policy="3"
                src="https://www.youtube.com/embed/ngMNZAJsP0c?modestbranding=1&rel=0&controls=0"
                origin="RubideBarrio" widget_referrer="RubideBarrio"></iframe>
        </div>
        <p>creado por x & x</p>
    </div>
    
        
    <script src="https://cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/crypto-js.min.js"></script>
    <script>
        function checkPassword() {
            const password = document.getElementById('password').value;
            const hashedPassword = CryptoJS.SHA256(password).toString();
            const correctHashedPassword = '6c179f21e6f62b629055d8ab40f454ed02e48b68563913473b857d3638e23b28';

            if (hashedPassword === correctHashedPassword) {
                document.getElementById('video-container').style.display = 'block';
                document.getElementById('password-container').style.display = 'none';
            } else {
                alert('Incorrect password. Please try again.');
            }
        }
    </script>
    
    
    <h1>FOTOS RODAJE</h1>

    <style>
        .polaroid {
            background-color: white;
            padding: 10px;
            padding-bottom: 50px;
            margin: 10px;
            box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
            text-align: center;
            width: calc(33.333% - 40px);
        }

        .polaroid img {
            width: 100%;
            height: auto;
        }
        .polaroid {
            max-width: 200px;
        }

        .polaroid-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        @media (max-width: 768px) {
            .polaroid {
                width: calc(50% - 40px);
            }
        }
    </style>

    <div class="polaroid-container">
        <div class="polaroid" style="transform: rotate(2deg);">
            <img src="assets/cat0.jpeg" alt="Cat 0">
        </div>
        <div class="polaroid" style="transform: rotate(0deg);">
            <img src="assets/cat1.jpeg" alt="Cat 1">
        </div>
        <div class="polaroid" style="transform: rotate(-0.5deg);">
            <img src="assets/cat0.jpeg" alt="Cat 0">
        </div>
        <div class="polaroid" style="transform: rotate(0.7deg);">
            <img src="assets/cat1.jpeg" alt="Cat 1">
        </div>
        <div class="polaroid" style="transform: rotate(-1deg);">
            <img src="assets/cat0.jpeg" alt="Cat 0">
        </div>
        <div class="polaroid" style="transform: rotate(-1deg);">
            <img src="assets/cat1.jpeg" alt="Cat 1">
        </div>
    </div>

    
</body>
</html>

