---
layout: none
---

<link rel="stylesheet" href="styles/index.css">
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rubi de Barrio</title>
    <link rel="icon" href="assets/favicon_estrellita.png" type="image/png">
    

    <style>
        /* Add some basic styling */

    
        #video-container {
            display: none;
        }
    
        footer {
            margin-top: auto;
            background-color: #f1f1f1;
            padding: 20px;
            position: fixed;
            bottom: 0;
            right: 0;
        }
    </style>
</head>


<body>
    <header>
        <nav>
            <img src="assets/header.png" alt="Rubi de Barrio" style="max-height: 70px;">
            <!-- <h1>Rubi de Barrio</h1> -->
            <div>
                <a href="#personajes">Personajes</a>
            </div>
        </nav>
    </header>

    
    <div>
        <p>El bodegón más vistoso en bucle</p>
        <div id="password-container">
            <input type="password" id="password" placeholder="Enter password">
            <button onclick="checkPassword()">Submit</button>
        </div>
        <div id="video-container"> 
            <iframe
                width="560" height="315" frameborder="0" allowfullscreen
                iv_load_policy="3"
                src="https://www.youtube.com/embed/ngMNZAJsP0c?modestbranding=1&rel=0&controls=0"
                origin="RubideBarrio" widget_referrer="RubideBarrio"></iframe>
        </div>
        <p>creado por x & x</p>
    </div>
    
    
    
    <!-- Placeholder for footer -->
    <div id="footer-placeholder"></div>
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
    
    <!-- <footer class="footer">
        <div class="corner">
            <div class="layer layer1"></div>
            <div class="layer layer2"></div>
            <div class="layer layer3"></div>
        </div>
        <p>&copy; 2024</p>
    </footer> -->
    
    
</body>
</html>

{% include footer.html %}
