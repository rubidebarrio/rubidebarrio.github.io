---
layout: base
permalink: /
---


<body>
    <!-- ################################################################## -->
    <section
        id="test"
        style="margin: 0; background-color: black; height: 100vh; display: flex; justify-content: center; align-items: center;">
        <img src="assets/bodegones_bucle2.gif" alt="Bucle Bodegones" id="bucle-bodegones" style="width: 100vw; min-width: min(720px, 80vw);">
        <!-- <script>
            window.addEventListener('scroll', function() {
            const img = document.getElementById('bucle-bodegones');
            const scrollY = window.scrollY;
            const minWidth = 500; // Minimum width in pixels
            const maxWidth = window.innerWidth; // Maximum width is the full width
            const newWidth = Math.max(minWidth, maxWidth - scrollY);
            img.style.width = newWidth + 'px';
            });
        </script> -->
        
        <!-- <p class="descripcion" style="color: #e0e0e0">
            Rubí de Barrio es una serie de género comedia/misterio
            creada por Paula Mañeru y Paula Sanz.
        </p> -->

    </section>


    <div>
        <img src="assets/tablero_cluedo.png" alt="Bucle Bodegones" style="width: 80vw;">
    </div>


    <!-- ################################################################## -->
    <section>
        <h1>DESCRIPCIÓN</h1>
        <p>resumen del proyecto</p>
    </section>



    <!-- ################################################################## -->
    <section>

        <h1>SINOPSIS</h1>
        <p>Sepultadas bajo montañas de facturas por pagar, Verónica, Sofía y su séquito de mamarrachas del (ahora)
            decadente Cabaret Rubí arriesgan sus vidas al encontrarse un cliente muerto en el club. Con la policía
            en los talones y un cadáver en la nevera, Verónica hace todo lo posible por salvar su local de la ruina
            y de las torpes estrategias de sus compañeros. El espectáculo debe continuar, ¿no?</p>
        <div>
            <img src="assets/figuritas_personajes.png" alt="Personajes"
                style="width: 100%; filter: drop-shadow(0px 4px 8px #0006); max-width: 1200px;">
        </div>
    </section>



    <!-- ################################################################## -->
    <section>

        <h1>¿QUIENES SOMOS?</h1>
        <p>
            ¡Hola! Soy Paula (Mañeru). Nací en el 97, así que llevo 27 años aferrándome a todo estímulo creativo y
            enganchada a la purpurina. Empecé a hacer teatro desde pequeña (ahí me encontré a Paula) y, cuando crecí, volé a
            Madrid para formarme como actriz y compaginarlo con la carrera de Comunicación Audiovisual en la UC3M. Siempre
            he tenido inquietud por sacar adelante proyectos propios desde las obras del grupo de teatro a pequeños
            cortometrajes. Recientemente, he trabajado para el equipo de Dirección de Cuéntame Cómo Pasó (T22, T23) y Sueños
            de Libertad.
        </p>
            
        <p>Yo soy Paula (Sanz). Desde pequeña soñaba con habitar mundos de fantasía y eso me llevó a creer que quería ser
            actriz, así que hice teatro hasta que me di cuenta de que prefería crear esos mundos. Tras estudiar Relaciones
            Internacionales, decidí viajar a Inglaterra para estudiar Comunicación y Producción Audiovisual, un país en el
            que sigo residiendo y trabajando en el ámbito de la producción. Sueños por alcanzar ya solo me quedan rodar
            nuestra serie y conocer a una jirafa.
        </p>
    </section>
                


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
        }

        @media (max-width: 768px) {
            .polaroid {
                width: 35%;
            }
        }
    </style>

    <section class="polaroid-container">
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
    </section>

    <style>
        .slideshow-container {
            display: flex;
            overflow-x: auto;
            /* scroll-snap-type: x mandatory; */
            -webkit-overflow-scrolling: touch;
            width: 100vw;
        }

        .slide {
            flex: 0 0 auto;
            width: 100vw;
            scroll-snap-align: start;
        }

        .slide img {
            width: inherit;
            height: auto;
            display: block;
        }
    </style>

    <section class="slideshow-container">
        <div class="slide">
            <img src="assets/polaroid/slide1.png" alt="Slide 1">
        </div>
        <div class="slide">
            <img src="assets/polaroid/slide2.png" alt="Slide 2">
        </div>
        <div class="slide">
            <img src="assets/polaroid/slide3.png" alt="Slide 3">
        </div>
    </div>

    <script>
        const slideshowContainer = document.querySelector('.slideshow-container');

        slideshowContainer.addEventListener('scroll', () => {
            if (slideshowContainer.scrollLeft + slideshowContainer.clientWidth >= slideshowContainer.scrollWidth) {
                slideshowContainer.scrollLeft = 0;
            }
        });
    </script>


</body>