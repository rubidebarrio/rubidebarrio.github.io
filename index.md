---
layout: base
permalink: /
---


<body>
    <style>
        #video-container {
            display: none;
        }

        h1 {
            text-align: center;
            font-family: 'Courier New', Courier, monospace;
            font-size: 2em;
            color: #ff0000;
            padding: 1.5em 0 0.5em;
        }
    </style>

    
    <!-- ################################################################## -->
    <h1>El bodegón más vistoso en bucle</h1>
    <div>
        <img src="assets/bucle_bodegones-7.gif" alt="Bucle Bodegones"
            style="max-width: 600px; width: 80%;">
        <p>creado por Paula Mañero & Paula Sanz</p>
    </div>


    <div>
        <img 
            src="assets/tablero_cluedo.png" alt="Bucle Bodegones"
            style="width: 80vw;"
        >
    </div>


    <div>
        <div id="password-container">
            <input class="rubi_input" type="password" id="password" placeholder="Enter password">
            <button class="rubi_btn" onclick="checkPassword()">Submit</button>
        </div>
        <div id="video-container"> 
            <iframe
                max-width="560" height="315" frameborder="0" allowfullscreen
                iv_load_policy="3"
                src="https://www.youtube.com/embed/ngMNZAJsP0c?modestbranding=1&rel=0&controls=0"
                origin="RubideBarrio" widget_referrer="RubideBarrio"></iframe>
        </div>
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


    <!-- ################################################################## -->
    <h1>DESCRIPCIÓN</h1>
    <p>resumen del proyecto</p>



    <!-- ################################################################## -->
    <h1>SINOPSIS</h1>
    <p>bla</p>
    <div>
        <img 
            src="assets/figuritas_personajes.png" alt="Personajes"
            style="width: 100%; filter: drop-shadow(0px 4px 8px #0006);"
        >
    </div>

    

    <!-- ################################################################## -->
    <h1>¿QUIENES SOMOS?</h1>
    <p>Texto de presentación</p>
    
    

    <!-- ################################################################## -->
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
            max-width: 900px;
            margin: 0 auto;
        }

        @media (max-width: 768px) {
            .polaroid {
                width: 35%;
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

