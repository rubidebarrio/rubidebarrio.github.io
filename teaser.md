---
layout: base
permalink: /teaser
---


<body>
    <style>
        #video-container {
            position: relative;
            margin: auto;
            height: 0;
            padding-bottom: calc(56.25% * 0.75); /* 16:9 */
            width: 75%;
        }
        .video {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }
    </style>


    <section>

        <!-- ################################################################## -->
        <h1>TEASER</h1>
        <div style="max-width: 720px; margin: auto;">
            <div id="password-container">
                <input class="rubi_input" type="password" id="password" placeholder="Enter password">
                <button class="rubi_btn" onclick="checkPassword()">Submit</button>
            </div>
            <div id="video-container" style="display: none;">
                <iframe
                max-width="1080" frameborder="0" allowfullscreen
                class="video"
                iv_load_policy="3"
                src="https://www.youtube.com/embed/ngMNZAJsP0c?modestbranding=1&rel=0&controls=0"
                origin="RubideBarrio" widget_referrer="RubideBarrio"></iframe>
            </div>
        </div>
    </section>
    
        
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

    
</body>

