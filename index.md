---
layout: base_no_header
permalink: /
---


<body>
    <header>
        <style>
            header {
                position: absolute;
                top: 0;
                left: 0;
                width: 100%;
                background-color: transparent;
                z-index: 10; /* Ensure the header is on top */
            }
        </style>
        <nav>
            <a href="/">
                <img class="header-logo" src="assets/header.png" alt="Rubi de Barrio">
            </a>
            
            <div>
                <a href="/teaser">Teaser</a>
            </div>
        </nav>
    </header>


    <!-- ################################################################## -->
    <section class="hero">
        <div class="parallax-container">
            <img class="hero-video" src="assets/bodegones_bucle1.gif" alt="Bucle Bodegones">
        </div>
        <div class="hero-overlay"></div>
        <!-- <div class="hero-content">
            <h1>Rubí de Barrio</h1>
            <p>Una serie de género comedia/misterio creada por Paula Mañeru y Paula Sanz.</p>
        </div> -->
    </section>


    <section>
        <img src="assets/tablero_cluedo.png" alt="Bucle Bodegones" style="width: 100%;">
    </section>


    <!-- ################################################################## -->
    <section>
        <h1>Descripción</h1>
        <p>
            Rubí de Barrio es una serie de género comedia/misterio creada por Paula Mañeru y Paula Sanz. Inspirada en
            una obra teatral producida en nuestra adolescencia, el proyecto comenzó tanto como un desafío para nosotras
            mismas, como una carta de amor a nuestros amigos que también participaron en aquella obra de teatro. La
            pregunta “¿Qué querríamos contar ahora?” nos llevó a desarrollar el mundo en el que el Cabaret existía y el
            tipo de aventuras que disfrutaríamos viendo a los personajes vivir.

            A pesar de ser una serie de entretenimiento, Rubí de Barrio refleja realidades y conversaciones presentes
            entre la gente de nuestra generación que a menudo no se ven representadas en los medios.

        </p>
    </section>



    <!-- ################################################################## -->
    <section>

        <h1>Sinopsis</h1>
        <p>Sepultadas bajo montañas de facturas por pagar, Verónica, Sofía y su séquito de mamarrachas del (ahora)
            decadente Cabaret Rubí arriesgan sus vidas al encontrarse un cliente muerto en el club. Con la policía
            en los talones y un cadáver en la nevera, Verónica hace todo lo posible por salvar su local de la ruina
            y de las torpes estrategias de sus compañeros. El espectáculo debe continuar, ¿no?</p>
        <div>
            <img src="assets/figuritas_personajes.png" alt="Personajes"
                style="width: 100%;">
        </div>
    </section>


    <!-- ################################################################## -->
    <section>
        <h1>Personajes</h1>

        <div>
            <div>
                <h4>Veronica</h4>
                <p>
                    La dueña del cabaret. Trata de mantener el recuerdo de su madre, el icono
                    del cabaret Renata Rubí, vivo a través del local, lo cual le llevará a tomar decisiones cada vez más
                    controvertidas para salvarlo.
                </p>
            </div>
            <div>
                <h4>Sofía</h4>
                <p>
                    La otra cara de la moneda de Verónica. Alcohólica funcional siempre trata de
                    evadirse y entretenerse. Más pesimista frente a la realidad, sólo está dispuesta a luchar por Verónica y
                    se verá obligada a hacerlo.
                </p>
            </div>
            <div>
                <h4>El elenco</h4>
                <p>
                    Compuesto por un grupo de jóvenes eclécticos, el resto de los artistas del
                    cabaret está dividido entre personajes realistas y otros más fantasiosos que dan lugar a divertidos
                    intentos de ayudar.
                </p>
            </div>
        </div>
    </section>



    <!-- ################################################################## -->
    <section>

        <h1>¿Quienes somos?</h1>
        <p>
            ¡Hola! Soy Paula (Mañeru). Nací en el 97, así que llevo 27 años aferrándome a todo estímulo creativo y
            enganchada a la purpurina. Empecé a hacer teatro desde pequeña (ahí me encontré a Paula) y, cuando crecí,
            volé a Madrid para formarme como actriz y compaginarlo con la carrera de Comunicación Audiovisual en la
            UC3M.
            Siempre he tenido inquietud por sacar adelante proyectos propios desde las obras del grupo de teatro a
            pequeños
            cortometrajes. Recientemente, he trabajado para el equipo de Dirección de Cuéntame Cómo Pasó (T22, T23) y
            Sueños de Libertad.
        </p>

        <p>
            Yo soy Paula (Sanz). Desde pequeña soñaba con habitar mundos de fantasía y eso me llevó a creer que quería
            ser actriz, así que hice teatro hasta que me di cuenta de que prefería crear esos mundos. Tras estudiar
            Relaciones Internacionales, decidí viajar a Inglaterra para estudiar Comunicación y Producción Audiovisual,
            un país en el que sigo residiendo y trabajando en el ámbito de la producción. Sueños por alcanzar ya solo me
            quedan rodar nuestra serie y conocer a una jirafa.
        </p>
    </section>



    <!-- ################################################################## -->
    <h1>Fotos rodaje</h1>

    <style>
        .slideshow-container {
            display: flex;
            overflow-x: auto; /* Allow user-driven scrolling */
            scrollbar-width: none;
            width: 100%;
            -webkit-overflow-scrolling: touch;
            position: relative;
        }

        .slideshow-track {
            display: flex;
            /* Removed animation for user-driven scrolling */
        }

        .slide {
            flex: 0 0 auto;
            height: max(30vh, 20vw);
        }

        .slide img {
            height: 100%;
            width: auto;
            display: block;
        }
    </style>

    <section class="slideshow-container">
        <div class="slideshow-track">
            <img class="slide" src="assets/polaroid/slide1.png" alt="Polaroid slide 1">
            <img class="slide" src="assets/polaroid/slide2.png" alt="Polaroid slide 2">
            <img class="slide" src="assets/polaroid/slide3.png" alt="Polaroid slide 3">
            <!-- <img class="slide" src="assets/polaroid/slide4.png" alt="Polaroid slide 4">
            <img class="slide" src="assets/polaroid/slide5.png" alt="Polaroid slide 5">
            <img class="slide" src="assets/polaroid/slide6.png" alt="Polaroid slide 6"> -->
        </div>
    </section>

    <script>
        const container = document.querySelector('.slideshow-container');
        const track = document.querySelector('.slideshow-track');

        container.addEventListener('scroll', () => {
            const scrollLeft = container.scrollLeft;
            const scrollWidth = container.scrollWidth;
            const clientWidth = container.clientWidth;

            // Check if scrolled to the end
            if (scrollLeft + clientWidth >= scrollWidth - 10) {
                // Duplicate the track
                const newTrack = track.cloneNode(true);
                container.appendChild(newTrack);

                // Remove the leftmost track if there are more than 2 tracks
                const tracks = container.querySelectorAll('.slideshow-track');
                if (tracks.length > 3) {
                    container.removeChild(tracks[0]);
                }
            }
        });
    </script>



</body>