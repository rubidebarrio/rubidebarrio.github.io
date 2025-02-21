---
layout: base
permalink: /teaser
---


<body>
    <style>
        #video-container-yt {
            position: relative;
            margin: auto;
            height: 0;
            /* padding-bottom: calc(56.25% * 0.90); */
            width: 720px;
            height: 400px;
        }
        #video-container-vm {
            position: relative;
        }
        .video {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }

        /* ************************************* */
        .rubi_btn {
            background-color: var(--accent_red_2);
            border-radius: 7px;
            color: white;
            padding: 7px 12px;
            border: none;
            cursor: pointer;
            font-size: 1em;
            margin-top: 10px;
        }
        .rubi_btn:hover {
            filter: brightness(115%);
        }
        .rubi_input {
            padding: 7px 12px;
            border-radius: 7px;
            border: 1px solid var(--accent_red_2);
            margin-top: 10px;
            color: #303030;
        }
    </style>


    <!-- ################################################################## -->
    <section>
        <h1>Teaser</h1>
        <div>
            <div id="password-container" style="margin: 20px auto;">
                <input class="rubi_input" type="password" id="password" placeholder="Enter password">
                <button class="rubi_btn" onclick="checkPassword()">Submit</button>
            </div>
            <div id="video-container-yt" style="display: block;">
                <iframe
                width="720" height="400" 
                frameborder="0" allowfullscreen
                class="video"
                iv_load_policy="3"
                src="https://www.youtube.com/embed/ngMNZAJsP0c?modestbranding=1&rel=0&controls=0"
                origin="RubideBarrio" widget_referrer="RubideBarrio"></iframe>
            </div>
        </div>
    </section>


    <section>
        <div id="video-container-vm">
            <iframe 
                src="https://player.vimeo.com/video/347119375"
                byline="false" portrait="false" title="false"
                vimeo_logo="false" color="var(--accent_red_1)"
                width="720" height="400" 
                frameborder="0" allow="autoplay; fullscreen" 
                allowfullscreen>
            </iframe>
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

