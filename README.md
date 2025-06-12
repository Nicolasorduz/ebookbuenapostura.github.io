!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Postura Perfecta - Alivia tu Dolor de Espalda desde Casa</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/js/all.min.js"></script>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            color: #333;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header */
        .header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 60px 0;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .header::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><circle cx="20" cy="20" r="2" fill="rgba(255,255,255,0.1)"/><circle cx="80" cy="80" r="2" fill="rgba(255,255,255,0.1)"/><circle cx="40" cy="60" r="1" fill="rgba(255,255,255,0.1)"/></svg>') repeat;
            animation: float 20s infinite linear;
        }

        @keyframes float {
            0% { transform: translateX(-50px) translateY(-50px); }
            100% { transform: translateX(-50px) translateY(-70px); }
        }

        .header h1 {
            font-size: 3.2em;
            font-weight: 700;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
            position: relative;
            z-index: 1;
        }

        .header .subtitle {
            font-size: 1.4em;
            margin-bottom: 30px;
            opacity: 0.95;
            position: relative;
            z-index: 1;
        }

        .cta-primary {
            background: linear-gradient(45deg, #ff6b6b, #feca57);
            color: white;
            padding: 18px 40px;
            border: none;
            border-radius: 50px;
            font-size: 1.2em;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 8px 15px rgba(0,0,0,0.1);
            position: relative;
            z-index: 1;
            text-decoration: none;
            display: inline-block;
        }

        .cta-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 12px 25px rgba(0,0,0,0.15);
        }

        /* Main Content */
        .main-content {
            background: white;
            margin: -30px auto 0;
            border-radius: 20px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            overflow: hidden;
            position: relative;
            z-index: 2;
        }

        .hero-section {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 60px;
            padding: 80px 60px;
            align-items: center;
        }

        .hero-content h2 {
            font-size: 2.5em;
            color: #2c3e50;
            margin-bottom: 25px;
            line-height: 1.2;
        }

        .hero-content p {
            font-size: 1.2em;
            color: #7f8c8d;
            margin-bottom: 30px;
        }

        .ebook-mockup {
            text-align: center;
            position: relative;
        }

        .ebook-cover {
            width: 300px;
            height: 400px;
            background: linear-gradient(135deg, #74b9ff, #0984e3);
            border-radius: 15px;
            margin: 0 auto;
            position: relative;
            box-shadow: 0 20px 40px rgba(0,0,0,0.15);
            transform: perspective(1000px) rotateY(-15deg);
            transition: transform 0.3s ease;
        }

        .ebook-cover:hover {
            transform: perspective(1000px) rotateY(-10deg) scale(1.05);
        }

        .ebook-cover::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 300 400"><text x="150" y="100" text-anchor="middle" fill="white" font-size="28" font-weight="bold">POSTURA</text><text x="150" y="140" text-anchor="middle" fill="white" font-size="28" font-weight="bold">PERFECTA</text><text x="150" y="200" text-anchor="middle" fill="rgba(255,255,255,0.8)" font-size="16">Guía Completa para</text><text x="150" y="220" text-anchor="middle" fill="rgba(255,255,255,0.8)" font-size="16">Aliviar el Dolor</text><text x="150" y="240" text-anchor="middle" fill="rgba(255,255,255,0.8)" font-size="16">de Espalda</text></svg>') no-repeat center;
            border-radius: 15px;
        }

        /* Stretching Images */
        .stretch-gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin: 40px 0;
        }

        .stretch-image {
            position: relative;
            height: 200px;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
            background-size: cover;
            background-position: center;
            transition: transform 0.3s ease;
        }

        .stretch-image:hover {
            transform: scale(1.05);
        }

        .stretch-image::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(to bottom, transparent 0%, rgba(0,0,0,0.3) 100%);
        }

        .stretch-caption {
            position: absolute;
            bottom: 15px;
            left: 15px;
            color: white;
            font-weight: bold;
            z-index: 1;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.7);
        }

        .stretch1 {
            background-image: url('https://images.unsplash.com/photo-1571019613454-1cb2f99b2d8b?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80');
        }

        .stretch2 {
            background-image: url('https://images.unsplash.com/photo-1506126613408-eca07ce68773?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80');
        }

        .stretch3 {
            background-image: url('https://images.unsplash.com/photo-1599901860904-17e6ed7083a0?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80');
        }

        .stretch4 {
            background-image: url('https://images.unsplash.com/photo-1544367567-0f2fcb009e0b?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80');
        }

        /* Exercise Section */
        .exercises-preview {
            background: linear-gradient(135deg, #e8f5e8 0%, #f0f8ff 100%);
            padding: 80px 0;
        }

        .exercises-preview h3 {
            text-align: center;
            font-size: 2.5em;
            color: #2c3e50;
            margin-bottom: 60px;
        }

        /* Benefits Section */
        .benefits {
            background: linear-gradient(135deg, #a8edea 0%, #fed6e3 100%);
            padding: 80px 0;
        }

        .benefits h3 {
            text-align: center;
            font-size: 2.5em;
            color: #2c3e50;
            margin-bottom: 60px;
        }

        .benefits-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 40px;
        }

        .benefit-card {
            background: white;
            padding: 40px 30px;
            border-radius: 20px;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
        }

        .benefit-card:hover {
            transform: translateY(-10px);
        }

        .benefit-icon {
            font-size: 3em;
            color: #667eea;
            margin-bottom: 20px;
        }

        .benefit-card h4 {
            font-size: 1.4em;
            color: #2c3e50;
            margin-bottom: 15px;
        }

        /* Testimonials */
        .testimonials {
            padding: 80px 0;
            background: white;
        }

        .testimonials h3 {
            text-align: center;
            font-size: 2.5em;
            color: #2c3e50;
            margin-bottom: 60px;
        }

        .testimonials-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 40px;
        }

        .testimonial {
            background: #f8f9fa;
            padding: 40px;
            border-radius: 20px;
            border-left: 5px solid #667eea;
            position: relative;
        }

        .testimonial::before {
            content: '"';
            font-size: 4em;
            color: #667eea;
            position: absolute;
            top: 10px;
            left: 20px;
            opacity: 0.3;
        }

        .testimonial-text {
            font-style: italic;
            margin-bottom: 20px;
            font-size: 1.1em;
            color: #555;
        }

        .testimonial-author {
            font-weight: bold;
            color: #2c3e50;
        }

        .testimonial-role {
            color: #7f8c8d;
            font-size: 0.9em;
        }

        /* Guarantee Section */
        .guarantee {
            background: linear-gradient(135deg, #ffeaa7 0%, #fab1a0 100%);
            padding: 60px 0;
            text-align: center;
        }

        .guarantee-content {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 30px;
            flex-wrap: wrap;
        }

        .guarantee-badge {
            background: white;
            width: 120px;
            height: 120px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }

        .guarantee-badge i {
            font-size: 3em;
            color: #00b894;
        }

        .guarantee-text h4 {
            font-size: 1.8em;
            color: #2c3e50;
            margin-bottom: 15px;
        }

        /* FAQ Section */
        .faq {
            padding: 80px 0;
            background: white;
        }

        .faq h3 {
            text-align: center;
            font-size: 2.5em;
            color: #2c3e50;
            margin-bottom: 60px;
        }

        .faq-item {
            background: #f8f9fa;
            margin-bottom: 20px;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.08);
        }

        .faq-question {
            padding: 25px;
            background: #667eea;
            color: white;
            cursor: pointer;
            font-weight: bold;
            font-size: 1.1em;
            display: flex;
            justify-content: space-between;
            align-items: center;
            transition: background 0.3s ease;
        }

        .faq-question:hover {
            background: #5a6fd8;
        }

        .faq-answer {
            padding: 0 25px;
            max-height: 0;
            overflow: hidden;
            transition: all 0.3s ease;
            background: white;
        }

        .faq-answer.active {
            padding: 25px;
            max-height: 200px;
        }

        /* Final CTA */
        .final-cta {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 80px 0;
            text-align: center;
        }

        .price-box {
            background: white;
            color: #2c3e50;
            padding: 40px;
            border-radius: 20px;
            display: inline-block;
            margin: 30px 0;
            box-shadow: 0 15px 35px rgba(0,0,0,0.1);
        }

        .old-price {
            text-decoration: line-through;
            color: #999;
            font-size: 1.2em;
        }

        .new-price {
            font-size: 3em;
            font-weight: bold;
            color: #e74c3c;
            margin: 10px 0;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .header h1 {
                font-size: 2.2em;
            }

            .header .subtitle {
                font-size: 1.1em;
            }

            .hero-section {
                grid-template-columns: 1fr;
                padding: 40px 30px;
                gap: 40px;
            }

            .hero-content {
                text-align: center;
            }

            .hero-content h2 {
                font-size: 2em;
            }

            .ebook-cover {
                width: 250px;
                height: 330px;
            }

            .benefits, .testimonials, .faq {
                padding: 60px 0;
            }

            .benefits h3, .testimonials h3, .faq h3 {
                font-size: 2em;
            }

            .guarantee-content {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="header">
        <div class="container">
            <h1>¡Alivia tu Dolor de Espalda!</h1>
            <p class="subtitle">Descubre la guía comprobada para corregir tu postura desde casa</p>
            <a href="#comprar" class="cta-primary">¡Quiero mejorar mi postura!</a>
        </div>
    </header>

    <!-- Main Content -->
    <main class="main-content">
        <div class="container">
            <!-- Hero Section -->
            <section class="hero-section">
                <div class="hero-content">
                    <h2>Postura Perfecta: Tu Solución Definitiva</h2>
                    <p>Elimina el dolor de espalda, mejora tu postura y recupera tu bienestar con ejercicios simples que puedes hacer desde casa. Sin tratamientos costosos, sin complicaciones.</p>
                    <a href="#comprar" class="cta-primary">Descargar ahora por USD $9.99</a>
                </div>
                <div class="ebook-mockup">
                    <div class="ebook-cover"></div>
                </div>
            </section>
        </div>
    </main>

    <!-- Exercise Preview Section -->
    <section class="exercises-preview">
        <div class="container">
            <h3>Ejercicios Que Aprenderás</h3>
            <p style="text-align: center; font-size: 1.2em; color: #666; margin-bottom: 40px;">
                Movimientos simples y efectivos que transformarán tu postura
            </p>
            <div class="stretch-gallery">
                <div class="stretch-image stretch1">
                    <div class="stretch-caption">Estiramiento Cervical</div>
                </div>
                <div class="stretch-image stretch2">
                    <div class="stretch-caption">Fortalecimiento Lumbar</div>
                </div>
                <div class="stretch-image stretch3">
                    <div class="stretch-caption">Apertura de Hombros</div>
                </div>
                <div class="stretch-image stretch4">
                    <div class="stretch-caption">Elongación Dorsal</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Benefits Section -->
    <section class="benefits">
        <div class="container">
            <h3>¿Qué Vas a Aprender?</h3>
            <div class="benefits-grid">
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-dumbbell"></i>
                    </div>
                    <h4>Ejercicios Fáciles desde Casa</h4>
                    <p>Rutinas simples de 10-15 minutos que puedes hacer sin equipos especiales. Perfectas para tu rutina diaria.</p>
                </div>
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-chart-line"></i>
                    </div>
                    <h4>Resultados Visibles en Semanas</h4>
                    <p>Métodos probados que te ayudarán a ver mejoras en tu postura y reducción del dolor en pocas semanas.</p>
                </div>
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-user-md"></i>
                    </div>
                    <h4>Aprobado por Especialistas</h4>
                    <p>Técnicas respaldadas por fisioterapeutas y especialistas en salud física para garantizar tu seguridad.</p>
                </div>
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-piggy-bank"></i>
                    </div>
                    <h4>Sin Tratamientos Costosos</h4>
                    <p>Ahorra miles en terapias físicas y tratamientos. Todo lo que necesitas está en esta guía completa.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials -->
    <section class="testimonials">
        <div class="container">
            <h3>Lo Que Dicen Nuestros Lectores</h3>
            <div class="testimonials-grid">
                <div class="testimonial">
                    <p class="testimonial-text">Después de años de dolor de espalda por el trabajo de oficina, esta guía me cambió la vida. En solo 3 semanas ya noto una diferencia increíble.</p>
                    <div class="testimonial-author">María González</div>
                    <div class="testimonial-role">Contadora, 34 años</div>
                </div>
                <div class="testimonial">
                    <p class="testimonial-text">Los ejercicios son súper fáciles de seguir y realmente funcionan. Mi postura ha mejorado notablemente y ya no tengo ese dolor constante.</p>
                    <div class="testimonial-author">Carlos Mendoza</div>
                    <div class="testimonial-role">Diseñador Gráfico, 28 años</div>
                </div>
                <div class="testimonial">
                    <p class="testimonial-text">Como madre ocupada, necesitaba algo práctico. Esta guía es perfecta: ejercicios rápidos que puedo hacer mientras los niños juegan.</p>
                    <div class="testimonial-author">Ana Rodríguez</div>
                    <div class="testimonial-role">Ama de Casa, 31 años</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Guarantee -->
    <section class="guarantee">
        <div class="container">
            <div class="guarantee-content">
                <div class="guarantee-badge">
                    <i class="fas fa-shield-alt"></i>
                </div>
                <div class="guarantee-text">
                    <h4>Garantía de Satisfacción 30 Días</h4>
                    <p>Si no ves mejoras en tu postura y dolor de espalda en 30 días, te devolvemos el 100% de tu dinero. Sin preguntas.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- FAQ -->
    <section class="faq">
        <div class="container">
            <h3>Preguntas Frecuentes</h3>
            <div class="faq-item">
                <div class="faq-question" onclick="toggleFAQ(this)">
                    ¿Cuánto tiempo necesito dedicar diariamente?
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    Solo necesitas 10-15 minutos al día. Los ejercicios están diseñados para adaptarse a tu rutina diaria sin complicaciones.
                </div>
            </div>
            <div class="faq-item">
                <div class="faq-question" onclick="toggleFAQ(this)">
                    ¿Necesito equipos especiales?
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    No necesitas ningún equipo especial. Todos los ejercicios se pueden realizar con elementos básicos que tienes en casa o simplemente con tu propio peso corporal.
                </div>
            </div>
            <div class="faq-item">
                <div class="faq-question" onclick="toggleFAQ(this)">
                    ¿Cómo recibo el ebook después de la compra?
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    Inmediatamente después del pago, recibirás un enlace de descarga en tu email. El ebook está en formato PDF y es compatible con todos los dispositivos.
                </div>
            </div>
            <div class="faq-item">
                <div class="faq-question" onclick="toggleFAQ(this)">
                    ¿Es seguro para personas con lesiones previas?
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    La guía incluye modificaciones para diferentes niveles y condiciones. Sin embargo, siempre recomendamos consultar con un profesional de la salud si tienes lesiones graves.
                </div>
            </div>
        </div>
    </section>

    <!-- Final CTA -->
    <section class="final-cta" id="comprar">
        <div class="container">
            <h3>¡No Dejes que el Dolor Controle tu Vida!</h3>
            <p>Únete a miles de personas que ya han transformado su postura y eliminado el dolor de espalda</p>
            
            <div class="price-box">
                <div class="new-price">USD $9.99</div>
                <p><strong>¡Precio especial de lanzamiento!</strong></p>
                <p style="font-size: 0.9em; color: #666;">Acceso inmediato después del pago</p>
            </div>
            
            <a href="#" class="cta-primary" onclick="redirectToHotmart()">¡Comprar Ahora - USD $9.99!</a>
            
            <p style="margin-top: 20px; opacity: 0.9;">
                <i class="fas fa-lock"></i> Pago 100% seguro vía Hotmart | 
                <i class="fas fa-download"></i> Descarga inmediata | 
                <i class="fas fa-shield-alt"></i> Garantía 30 días
            </p>
        </div>
    </section>

    <script>
        function toggleFAQ(element) {
            const answer = element.nextElementSibling;
            const icon = element.querySelector('i');
            
            if (answer.classList.contains('active')) {
                answer.classList.remove('active');
                icon.style.transform = 'rotate(0deg)';
            } else {
                // Close all other FAQs
                document.querySelectorAll('.faq-answer.active').forEach(faq => {
                    faq.classList.remove('active');
                });
                document.querySelectorAll('.faq-question i').forEach(i => {
                    i.style.transform = 'rotate(0deg)';
                });
                
                // Open clicked FAQ
                answer.classList.add('active');
                icon.style.transform = 'rotate(180deg)';
            }
        }

        function redirectToHotmart() {
            // Aquí colocas tu enlace de afiliado de Hotmart
            // Ejemplo: window.open('https://pay.hotmart.com/tu-producto?off=tu-codigo-afiliado', '_blank');
            alert('¡Redirigiendo a Hotmart para completar tu compra segura!\n\nEn la implementación real, aquí se abrirá tu enlace de Hotmart.');
            
            // Descomenta y modifica esta línea con tu enlace real de Hotmart:
            // window.open('TU_ENLACE_DE_HOTMART_AQUI', '_blank');
        }

        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Add scroll animations
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);

        // Observe benefit cards, testimonials and stretch images
        document.querySelectorAll('.benefit-card, .testimonial, .stretch-image').forEach(el => {
            el.style.opacity = '0';
            el.style.transform = 'translateY(20px)';
            el.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
            observer.observe(el);
        });
    </script>
</body>
</html>
