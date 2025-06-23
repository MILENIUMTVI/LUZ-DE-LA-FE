# LUZ-DE-LA-FE
PROYECTO LUZ DE LA FE
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="La Luz de la Fe, liderada por FUNCECOR, fomenta los valores católicos con reflexiones profundas, cuentos inspiradores y actividades para fortalecer la vida familiar y la comunidad.">
    <meta name="keywords" content="valores católicos, fe, esperanza, caridad, familia, comunidad, FUNCECOR, catolicismo, cuentos de fe, educación espiritual">
    <meta name="author" content="FUNCECOR">
    <meta name="robots" content="index, follow">
    <title>La Luz de la Fe - FUNCECOR</title>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&family=Lora:wght@400;700&family=Montserrat:wght@500;600&family=Cormorant+Garamond:wght@400;700&display=swap" rel="stylesheet">
    <!-- Font Awesome para íconos -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Roboto', sans-serif;
            background: linear-gradient(135deg, #f9f9f9, #e0e8f0);
            color: #333;
            line-height: 1.8;
            overflow-x: hidden;
        }
        /* Encabezado */
        header {
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('banner.jpg');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 7rem 2rem;
            position: relative;
            animation: fadeInDown 2s ease-out;
        }
        header .header-content {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 2rem;
            max-width: 1300px;
            margin: 0 auto;
        }
        header h1 {
            font-family: 'Cormorant Garamond', serif;
            font-size: 4rem;
            margin: 0;
            text-shadow: 3px 3px 6px rgba(0,0,0,0.6);
            letter-spacing: 2px;
        }
        header img.logo {
            max-width: 280px;
            height: auto;
            transition: transform 0.4s ease, box-shadow 0.4s ease;
        }
        header img.logo:hover {
            transform: scale(1.1) rotate(5deg);
            box-shadow: 0 0 15px rgba(255,215,0,0.5);
        }
        header p {
            font-size: 1.4rem;
            max-width: 800px;
            margin: 2rem auto 0;
            font-family: 'Montserrat', sans-serif;
            opacity: 0.95;
            text-shadow: 1px 1px 3px rgba(0,0,0,0.3);
        }
        /* Animaciones */
        @keyframes fadeInDown {
            from { opacity: 0; transform: translateY(-50px); }
            to { opacity: 1; transform: translateY(0); }
        }
        /* Navegación */
        nav {
            background: linear-gradient(90deg, #1a5f7a, #0f3c4c);
            padding: 1.5rem;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 4px 20px rgba(0,0,0,0.3);
        }
        nav ul {
            display: flex;
            justify-content: center;
            list-style: none;
            gap: 2.5rem;
        }
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 600;
            font-family: 'Montserrat', sans-serif;
            font-size: 1.1rem;
            transition: color 0.4s, text-shadow 0.4s;
        }
        nav ul li a:hover {
            color: #ffd700;
            text-shadow: 0 0 10px rgba(255,215,0,0.7);
        }
        /* Contenedor Principal */
        .container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 3rem;
        }
        /* Sección Hero */
        .hero {
            text-align: center;
            padding: 5rem 2rem;
            background: linear-gradient(135deg, #ffffff, #f0f4f8, #e0e8f0);
            border-radius: 20px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.15);
            margin-bottom: 4rem;
            animation: slideUpFade 1.5s ease-out;
        }
        .hero h2 {
            font-family: 'Cormorant Garamond', serif;
            color: #1a5f7a;
            font-size: 3.5rem;
            margin-bottom: 2rem;
            text-transform: uppercase;
            letter-spacing: 1px;
        }
        .hero p {
            font-size: 1.3rem;
            max-width: 900px;
            margin: 0 auto 2.5rem;
            color: #444;
            font-family: 'Montserrat', sans-serif;
        }
        .multimedia {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
            gap: 2.5rem;
            margin-top: 2.5rem;
        }
        .multimedia iframe, .multimedia audio {
            width: 100%;
            border-radius: 12px;
            box-shadow: 0 6px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
        }
        .multimedia iframe:hover, .multimedia audio:hover {
            transform: scale(1.02);
        }
        /* Animación */
        @keyframes slideUpFade {
            from { transform: translateY(30px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }
        /* Carrusel de Valores */
        .values-carousel {
            display: flex;
            overflow-x: auto;
            gap: 2.5rem;
            padding: 2rem;
            background: linear-gradient(135deg, #e8f1f2, #d6e6f2, #c0d6e4);
            border-radius: 20px;
            margin-bottom: 4rem;
            scrollbar-width: thin;
            scrollbar-color: #1a5f7a #e8f1f2;
        }
        .value-card {
            flex: 0 0 240px;
            background: linear-gradient(135deg, #ffffff, #f8fafc);
            padding: 1.8rem;
            border-radius: 12px;
            text-align: center;
            box-shadow: 0 6px 18px rgba(0,0,0,0.15);
            transition: all 0.5s ease;
        }
        .value-card:hover {
            transform: translateY(-12px) scale(1.08);
            box-shadow: 0 12px 30px rgba(0,0,0,0.3);
        }
        .value-card h3 {
            color: #1a5f7a;
            font-family: 'Cormorant Garamond', serif;
            margin-bottom: 1rem;
            font-size: 1.5rem;
        }
        .value-card p {
            font-size: 1rem;
            color: #555;
            line-height: 1.5;
        }
        /* Secciones */
        .section {
            background: linear-gradient(135deg, #ffffff, #f8fafc, #f0f4f8);
            padding: 3rem;
            margin-bottom: 4rem;
            border-radius: 20px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.1);
            transition: transform 0.4s ease, box-shadow 0.4s ease;
        }
        .section:hover {
            transform: translateY(-8px);
            box-shadow: 0 12px 35px rgba(0,0,0,0.2);
        }
        .section h2 {
            font-family: 'Cormorant Garamond', serif;
            color: #1a5f7a;
            font-size: 3rem;
            margin-bottom: 2rem;
            text-align: center;
            text-shadow: 1px 1px 3px rgba(0,0,0,0.1);
        }
        /* Testimonios */
        .testimonials {
            background: linear-gradient(135deg, #e8f1f2, #d6e6f2, #c0d6e4);
            padding: 3rem;
            border-radius: 20px;
            margin-bottom: 4rem;
        }
        .testimonial {
            margin-bottom: 2.5rem;
            font-style: italic;
            font-size: 1.2rem;
            color: #333;
            padding: 2rem;
            background: linear-gradient(135deg, #ffffff, #f8fafc);
            border-radius: 12px;
            box-shadow: 0 6px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
        }
        .testimonial:hover {
            transform: translateY(-5px);
        }
        /* Formulario */
        .contact-form {
            display: flex;
            flex-direction: column;
            gap: 1.5rem;
            max-width: 800px;
            margin: 0 auto;
            padding: 2.5rem;
            background: linear-gradient(135deg, #ffffff, #f0f4f8);
            border-radius: 20px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.1);
        }
        .contact-form input, .contact-form textarea {
            padding: 1.2rem;
            border: 2px solid #ccc;
            border-radius: 10px;
            font-size: 1.2rem;
            transition: border-color 0.4s, box-shadow 0.4s;
        }
        .contact-form input:focus, .contact-form textarea:focus {
            border-color: #1a5f7a;
            box-shadow: 0 0 10px rgba(26,95,122,0.3);
            outline: none;
        }
        .contact-form button {
            background: linear-gradient(135deg, #1a5f7a, #0f3c4c);
            color: white;
            padding: 1.2rem;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            font-size: 1.3rem;
            font-weight: 600;
            text-transform: uppercase;
            transition: background 0.4s, transform 0.4s, box-shadow 0.4s;
        }
        .contact-form button:hover {
            background: linear-gradient(135deg, #0f3c4c, #1a5f7a);
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(0,0,0,0.3);
        }
        /* Pie de Página */
        footer {
            background: linear-gradient(135deg, #1a5f7a, #0f3c4c, #0a2a36);
            color: white;
            text-align: center;
            padding: 3rem;
            margin-top: 4rem;
        }
        footer a {
            color: #ffd700;
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s, text-shadow 0.3s;
        }
        footer a:hover {
            color: #ffeb3b;
            text-shadow: 0 0 10px rgba(255,235,59,0.7);
        }
        /* Nueva Sección: Cuentos de Fe */
        .faith-stories {
            background: linear-gradient(135deg, #f8fafc, #e8f1f2, #d6e6f2);
            padding: 3rem;
            margin-bottom: 4rem;
            border-radius: 20px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.1);
        }
        .faith-stories h2 {
            font-family: 'Cormorant Garamond', serif;
            color: #1a5f7a;
            font-size: 3rem;
            margin-bottom: 2rem;
            text-align: center;
            text-shadow: 1px 1px 3px rgba(0,0,0,0.1);
        }
        .faith-stories .story-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
            gap: 2.5rem;
        }
        .faith-stories .story-card {
            background: linear-gradient(135deg, #ffffff, #f8fafc);
            padding: 2rem;
            border-radius: 15px;
            box-shadow: 0 6px 18px rgba(0,0,0,0.1);
            transition: transform 0.4s ease, box-shadow 0.4s ease;
        }
        .faith-stories .story-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 12px 30px rgba(0,0,0,0.2);
        }
        .faith-stories .story-card img {
            max-width: 100%;
            border-radius: 10px;
            margin-bottom: 1.5rem;
            transition: transform 0.3s ease;
        }
        .faith-stories .story-card img:hover {
            transform: scale(1.05);
        }
        .faith-stories .story-card .story-content h3 {
            color: #1a5f7a;
            font-family: 'Cormorant Garamond', serif;
            font-size: 1.8rem;
            margin-bottom: 1rem;
        }
        .faith-stories .story-card .story-content p {
            font-size: 1.1rem;
            color: #555;
            margin-bottom: 1.5rem;
        }
        .faith-stories .story-card .multimedia {
            grid-template-columns: 1fr;
            gap: 1.5rem;
        }
        /* Responsividad */
        @media (max-width: 768px) {
            header .header-content {
                flex-direction: column;
                gap: 1.5rem;
            }
            header h1 {
                font-size: 2.8rem;
            }
            header img.logo {
                max-width: 200px;
            }
            nav ul {
                flex-direction: column;
                gap: 1.5rem;
                text-align: center;
            }
            .hero h2 {
                font-size: 2.2rem;
            }
            .multimedia, .faith-stories .story-grid {
                grid-template-columns: 1fr;
            }
            .faith-stories .story-card {
                padding: 1.5rem;
            }
        }
    </style>
</head>
<body>
    <!-- Encabezado -->
    <header role="banner">
        <div class="header-content">
            <img src="logo.png" alt="Logo FUNCECOR - Fundación Educativa para el Desarrollo" class="logo">
            <h1>FUNCECOR</h1>
        </div>
        <p>La Luz de la Fe: Un sendero que guía a las familias católicas hacia la unión, la esperanza y el amor de Dios, inspirando a padres, niños y jóvenes a vivir los valores cristianos de fe, esperanza, caridad, respeto, responsabilidad, perdón y solidaridad.</p>
    </header>

    <!-- Navegación -->
    <nav role="navigation">
        <ul>
            <li><a href="#inicio">Inicio</a></li>
            <li><a href="#valores">Valores</a></li>
            <li><a href="#padres">Para Padres</a></li>
            <li><a href="#jovenes">Para Niños y Jóvenes</a></li>
            <li><a href="#cuentos">Cuentos de Fe</a></li>
            <li><a href="#eventos">Eventos</a></li>
            <li><a href="#contacto">Contacto</a></li>
        </ul>
    </nav>

    <!-- Contenedor Principal -->
    <main class="container" role="main">
        <!-- Sección Hero -->
        <section id="inicio" class="hero" aria-labelledby="hero-title">
            <h2 id="hero-title">Bienvenidos a La Luz de la Fe</h2>
            <p>En <strong>FUNCECOR</strong>, abrimos las puertas de un espacio donde los valores católicos florecen. Acompañamos a las familias en un viaje espiritual, ofreciendo reflexiones profundas, actividades inspiradoras y recursos que fortalecen la fe y el amor en el hogar, impactando positivamente a nuestras comunidades.</p>
            <div class="multimedia">
                <iframe width="560" height="315" src="https://www.youtube.com/embed/zoKoxeSRIag" title="Bienvenida a La Luz de la Fe" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            </div>
        </section>

        <!-- Carrusel de Valores -->
        <section id="valores" aria-labelledby="values-title">
            <h2 id="values-title">Nuestros Pilares de Fe</h2>
            <div class="values-carousel">
                <div class="value-card">
                    <h3>Fe</h3>
                    <p>Principio de la vida cristiana, que orienta al ser humano hacia la comunión con Dios y la vida eterna.</p>
                </div>
                <div class="value-card">
                    <h3>Esperanza</h3>
                    <p>Dirige el corazón del hombre hacia la verdadera felicidad, que se encuentra en la unión con Dios.</p>
                </div>
                <div class="value-card">
                    <h3>Caridad</h3>
                    <p>Ee manifiesta en actos concretos de amor, misericordia y servicio hacia los demás, especialmente hacia los más necesitados.</p>
                </div>
                <div class="value-card">
                    <h3>Respeto</h3>
                    <p>Honrar la dignidad de cada ser como reflejo de la creación divina.</p>
                </div>
                <div class="value-card">
                    <h3>Responsabilidad</h3>
                    <p>Compromiso fiel con nuestros deberes hacia Dios, familia y comunidad.</p>
                </div>
                <div class="value-card">
                    <h3>Perdón</h3>
                    <p>Es un acto de amor cristiano que refleja la misericordia de Dios.</p>
                </div>
                <div class="value-card">
                    <h3>Solidaridad</h3>
                    <p>Unirnos en amor y apoyo para construir un mundo más justo y fraternal.</p>
                </div>
            </div>
        </section>

        <!-- Sección para Padres -->
        <section id="padres" class="section" aria-labelledby="parents-title">
            <h2 id="parents-title">Guía Espiritual para Padres (25-50 años)</h2>
            <p>Queridos padres, este espacio les ofrece meditaciones profundas, oraciones guiadas y consejos prácticos para sembrar en sus hijos los valores católicos. Descubran cómo cultivar un hogar lleno de <strong>fe</strong>, <strong>responsabilidad</strong> y <strong>perdón</strong> bajo la luz la fe.</p>
            <div class="multimedia">
                <iframe width="560" height="315" src="https://www.youtube.com/embed/-2mRj-IBMbo" title="Meditación para padres en la fe" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <audio controls>
                    <source src="assets/oracion_familiar.mp3" type="audio/mp3">
                    Tu navegador no soporta el elemento de audio.
                </audio>
            </div>
        </section>

        <!-- Sección para Niños y Jóvenes -->
        <section id="jovenes" class="section" aria-labelledby="youth-title">
            <h2 id="youth-title">Aventura Espiritual para Niños y Jóvenes (5-18 años)</h2>
            <p>¡Jóvenes y pequeños exploradores de la fe! Sumérjanse en un mundo de historias, canciones y videos que les acercan a la <strong>caridad</strong>, la <strong>esperanza</strong> y la <strong>solidaridad</strong>, mientras crecen en amor y devoción.</p>
            <div class="multimedia">
                <iframe width="560" height="315" src="https://www.youtube.com/embed/1Tk4BB8y4hw" title="Aventura de la caridad" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <audio controls>
                    <source src="assets/cancion_infantil.mp3" type="audio/mp3">
                    Tu navegador no soporta el elemento de audio.
                </audio>
            </div>
        </section>

        <!-- Nueva Sección: Cuentos de Fe -->
        <section id="cuentos" class="faith-stories" aria-labelledby="stories-title">
            <h2 id="stories-title">Cuentos de Fe: Tesoros Espirituales</h2>
            <p>Embárquense en un viaje narrativo lleno de fe y enseñanza. Estos cuentos, diseñados para niños y jóvenes, transmiten los valores católicos a través de historias que tocan el corazón y elevan el espíritu.</p>
            <div class="story-grid">
                <div class="story-card">
                    <img src="assets/cuento1.jpg" alt="Ilustración del cuento 'La Luz del Perdón'">
                    <div class="story-content">
                        <h3>La Luz del Perdón</h3>
                        <p>Un niño aprende a perdonar a su amigo tras una discusión, guiado por la voz suave de Jesús que le muestra el poder del amor redentor.</p>
                        <div class="multimedia">
                            <iframe width="560" height="315" src="https://www.youtube.com/embed/j15P0ppFwa0" title="Cuento: La Luz del Perdón" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                            <audio controls>
                                <source src="assets/cuento_perdon.mp3" type="audio/mp3">
                                Tu navegador no soporta el elemento de audio.
                            </audio>
                        </div>
                    </div>
                </div>
                <div class="story-card">
                    <img src="assets/cuento2.jpg" alt="Ilustración del cuento 'El Árbol de la Caridad'">
                    <div class="story-content">
                        <h3>El Árbol de la Caridad</h3>
                        <p>Una familia descubre la alegría de compartir sus bienes con los necesitados, viendo cómo un pequeño acto de amor florece como un árbol eterno.</p>
                        <div class="multimedia">
                            <iframe width="560" height="315" src="https://www.youtube.com/embed/WPMN_fOY_Is" title="Cuento: El Árbol de la Caridad" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                            <audio controls>
                                <source src="assets/cuento_caridad.mp3" type="audio/mp3">
                                Tu navegador no soporta el elemento de audio.
                            </audio>
                        </div>
                    </div>
                </div>
                <div class="story-card">
                    <img src="assets/cuento3.jpg" alt="Ilustración del cuento 'La Estrella de la Esperanza'">
                    <div class="story-content">
                        <h3>La Estrella de la Esperanza</h3>
                        <p>Un joven encuentra fuerza en la fe al seguir una estrella que lo guía hacia la esperanza en tiempos de oscuridad.</p>
                        <div class="multimedia">
                            <iframe width="560" height="315" src="https://www.youtube.com/embed/D2kcF_LIaRM" title="Cuento: La Estrella de la Esperanza" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                            <audio controls>
                                <source src="assets/cuento_esperanza.mp3" type="audio/mp3">
                                Tu navegador no soporta el elemento de audio.
                            </audio>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Sección de Testimonios -->
        <section id="testimonios" class="testimonials" aria-labelledby="testimonials-title">
            <h2 id="testimonials-title">Voces de Nuestra Comunidad de Fe</h2>
            <div class="testimonial">
                <p>"La Luz de la Fe ha renovado nuestro hogar con oraciones diarias y un amor más profundo por los valores católicos." - <strong>María, madre de tres</strong></p>
            </div>
            <div class="testimonial">
                <p>"Los cuentos de fe han capturado el corazón de mis hijos; ahora piden rezar juntos cada noche." - <strong>Juan, padre dedicado</strong></p>
            </div>
            <div class="testimonial">
                <p>"El taller de oración nos ha unido como familia como nunca antes; gracias, FUNCECOR." - <strong>Ana, madre de dos</strong></p>
            </div>
        </section>

        <!-- Sección de Eventos -->
        <section id="eventos" class="section" aria-labelledby="events-title">
            <h2 id="events-title">Eventos para Enriquecer tu Fe</h2>
            <p>Participe en nuestras actividades diseñadas para fortalecer la fe familiar y comunitaria:</p>
            <ul>
                <li><strong>Taller de Oración Familiar</strong> - 15 de julio de 2025, 6:00 PM (Virtual)</li>
                <li><strong>Retiro Espiritual para Jóvenes</strong> - 22 de agosto de 2025, 9:00 AM (Presencial)</li>
                <li><strong>Festival de Cuentos de Fe</strong> - 10 de septiembre de 2025, 3:00 PM (Online)</li>
                <li><strong>Día de la Caridad Comunitaria</strong> - 5 de octubre de 2025, 10:00 AM (Local)</li>
            </ul>
        </section>

        <!-- Sección de Contacto -->
        <section id="contacto" class="section" aria-labelledby="contact-title">
            <h2 id="contact-title">Únete a Nuestra Misión</h2>
            <p>¿Desea formar parte de esta comunidad de fe o recibir nuestro boletín mensual con reflexiones y eventos? Compártanos su mensaje y camine con nosotros.</p>
            <form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
                <input type="text" name="name" placeholder="Tu Nombre Completo" required aria-label="Nombre">
                <input type="email" name="email" placeholder="Tu Correo Electrónico" required aria-label="Correo Electrónico">
                <textarea name="message" placeholder="Comparte tus ideas, sugerencias o peticiones de oración" rows="7" required aria-label="Mensaje"></textarea>
                <button type="submit">Enviar Mensaje con Fe</button>
            </form>
        </section>
    </main>

    <!-- Pie de Página -->
    <footer role="contentinfo">
        <p>© 2025 FUNCECOR - La Luz de la Fe. Todos los derechos reservados.</p>
        <p>Síguenos en <a href="https://facebook.com/funcecor" target="_blank"><i class="fab fa-facebook"></i> Facebook</a> | <a href="https://instagram.com/funcecor" target="_blank"><i class="fab fa-instagram"></i> Instagram</a> | <a href="mailto:contacto@funcecor.org">contacto@funcecor.org</a></p>
        <p>Diseñado con amor y fe para la gloria de Dios.</p>
    </footer>
</body>
</html>
