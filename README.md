
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RomaBraveLittleSparks - Viaggio a Roma</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Playfair+Display:wght@400;600;700&display=swap" rel="stylesheet">
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Inter', sans-serif;
            background: #fefefe;
            color: #333;
            line-height: 1.6;
        }
        
        .container {
            max-width: 900px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header */
        header {
            background: linear-gradient(135deg, #6a4c93 0%, #8b5fbf 100%);
            color: white;
            padding: 4rem 0;
            text-align: center;
        }
        
        .hero-title {
            font-family: 'Playfair Display', serif;
            font-size: 3.5rem;
            font-weight: 700;
            margin-bottom: 1rem;
            background: linear-gradient(45deg, #ffd700, #ffed4a);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .hero-subtitle {
            font-size: 1.3rem;
            font-weight: 300;
            opacity: 0.9;
            margin-bottom: 2rem;
        }
        
        /* Countdown */
        .countdown-section {
            background: #f8f9fa;
            padding: 3rem 0;
            border-bottom: 1px solid #e9ecef;
        }
        
        .countdown-container {
            text-align: center;
        }
        
        .countdown-title {
            font-family: 'Playfair Display', serif;
            font-size: 2.2rem;
            color: #6a4c93;
            margin-bottom: 2rem;
            font-weight: 600;
        }
        
        .countdown {
            display: flex;
            justify-content: center;
            gap: 2rem;
            flex-wrap: wrap;
        }
        
        .countdown-item {
            background: white;
            padding: 2rem 1.5rem;
            border-radius: 12px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.08);
            border: 1px solid #e9ecef;
            min-width: 120px;
            transition: transform 0.3s ease;
        }
        
        .countdown-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 30px rgba(106, 76, 147, 0.15);
        }
        
        .countdown-number {
            font-size: 3rem;
            font-weight: 700;
            color: #6a4c93;
            display: block;
            line-height: 1;
        }
        
        .countdown-label {
            font-size: 0.9rem;
            color: #6c757d;
            text-transform: uppercase;
            letter-spacing: 1px;
            font-weight: 500;
            margin-top: 0.5rem;
        }
        
        /* Main content */
        .main-content {
            padding: 4rem 0;
        }
        
        .section {
            margin-bottom: 5rem;
        }
        
        .section-header {
            text-align: center;
            margin-bottom: 3rem;
        }
        
        .section-title {
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            color: #6a4c93;
            margin-bottom: 1rem;
            font-weight: 600;
        }
        
        .section-subtitle {
            font-size: 1.1rem;
            color: #6c757d;
            font-weight: 300;
        }
        
        /* Accommodation */
        .accommodation-card {
            background: white;
            border-radius: 16px;
            box-shadow: 0 8px 30px rgba(0, 0, 0, 0.08);
            overflow: hidden;
            border: 1px solid #e9ecef;
        }
        
        .accommodation-header {
            background: linear-gradient(135deg, #6a4c93, #8b5fbf);
            color: white;
            padding: 2rem;
            text-align: center;
        }
        
        .accommodation-name {
            font-family: 'Playfair Display', serif;
            font-size: 1.8rem;
            font-weight: 600;
            margin-bottom: 0.5rem;
        }
        
        .accommodation-content {
            padding: 2rem;
        }
        
        .info-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
            margin-bottom: 2rem;
        }
        
        .info-item {
            display: flex;
            align-items: flex-start;
            gap: 1rem;
        }
        
        .info-icon {
            color: #6a4c93;
            font-size: 1.2rem;
            margin-top: 0.2rem;
        }
        
        .info-text {
            flex: 1;
        }
        
        .info-label {
            font-weight: 600;
            color: #333;
            margin-bottom: 0.2rem;
        }
        
        .info-value {
            color: #6c757d;
            font-size: 0.95rem;
        }
        
        .cta-button {
            display: inline-block;
            background: linear-gradient(135deg, #6a4c93, #8b5fbf);
            color: white;
            padding: 1rem 2rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            border: none;
            cursor: pointer;
        }
        
        .cta-button:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 25px rgba(106, 76, 147, 0.3);
        }
        
        .cta-button.secondary {
            background: linear-gradient(135deg, #ffd700, #ffed4a);
            color: #333;
            margin-left: 1rem;
        }
        
        /* Places */
        .places-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-bottom: 3rem;
        }
        
        .place-card {
            background: white;
            border-radius: 12px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.08);
            overflow: hidden;
            border: 1px solid #e9ecef;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .place-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 30px rgba(106, 76, 147, 0.15);
        }
        
        .place-content {
            padding: 2rem;
        }
        
        .place-name {
            font-family: 'Playfair Display', serif;
            font-size: 1.4rem;
            color: #6a4c93;
            margin-bottom: 1rem;
            font-weight: 600;
        }
        
        .place-description {
            color: #6c757d;
            line-height: 1.7;
        }
        
        /* Map */
        .map-container {
            margin: 3rem 0;
            border-radius: 16px;
            overflow: hidden;
            box-shadow: 0 8px 30px rgba(0, 0, 0, 0.08);
            border: 1px solid #e9ecef;
        }
        
        .map-container iframe {
            width: 100%;
            height: 450px;
            border: none;
        }
        
        .map-actions {
            text-align: center;
            margin-top: 2rem;
        }
        
        /* Gallery */
        .gallery-placeholder {
            background: white;
            border-radius: 16px;
            padding: 4rem 2rem;
            text-align: center;
            border: 2px dashed #e9ecef;
            transition: border-color 0.3s ease;
        }
        
        .gallery-placeholder:hover {
            border-color: #6a4c93;
        }
        
        .gallery-icon {
            font-size: 4rem;
            color: #6a4c93;
            margin-bottom: 1.5rem;
        }
        
        .gallery-title {
            font-family: 'Playfair Display', serif;
            font-size: 1.8rem;
            color: #6a4c93;
            margin-bottom: 1rem;
        }
        
        .gallery-text {
            color: #6c757d;
            font-size: 1.1rem;
        }
        
        /* Footer */
        footer {
            background: #f8f9fa;
            padding: 3rem 0;
            border-top: 1px solid #e9ecef;
            text-align: center;
        }
        
        .footer-quote {
            font-family: 'Playfair Display', serif;
            font-size: 1.5rem;
            color: #6a4c93;
            font-weight: 600;
            font-style: italic;
        }
        
        .sparkle {
            color: #ffd700;
            animation: sparkle 2s infinite;
        }
        
        @keyframes sparkle {
            0%, 100% { opacity: 1; transform: scale(1); }
            50% { opacity: 0.7; transform: scale(1.2); }
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .hero-title {
                font-size: 2.5rem;
            }
            
            .countdown {
                gap: 1rem;
            }
            
            .countdown-item {
                min-width: 100px;
                padding: 1.5rem 1rem;
            }
            
            .countdown-number {
                font-size: 2.5rem;
            }
            
            .cta-button.secondary {
                margin-left: 0;
                margin-top: 1rem;
            }
            
            .info-grid {
                grid-template-columns: 1fr;
            }
            
            .main-content {
                padding: 2rem 0;
            }
            
            .section {
                margin-bottom: 3rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1 class="hero-title">RomaBraveLittleSparks</h1>
            <p class="hero-subtitle">La grande avventura della nostra gilda di Final Fantasy XIV nella Città Eterna</p>
        </div>
    </header>

    <section class="countdown-section">
        <div class="container">
            <div class="countdown-container">
                <h2 class="countdown-title">Partenza per Roma in...</h2>
                <div class="countdown" id="countdown">
                    <div class="countdown-item">
                        <span class="countdown-number" id="days">0</span>
                        <span class="countdown-label">Giorni</span>
                    </div>
                    <div class="countdown-item">
                        <span class="countdown-number" id="hours">0</span>
                        <span class="countdown-label">Ore</span>
                    </div>
                    <div class="countdown-item">
                        <span class="countdown-number" id="minutes">0</span>
                        <span class="countdown-label">Minuti</span>
                    </div>
                    <div class="countdown-item">
                        <span class="countdown-number" id="seconds">0</span>
                        <span class="countdown-label">Secondi</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <main class="main-content">
        <div class="container">
            <!-- Accommodation Section -->
            <section class="section">
                <div class="section-header">
                    <h2 class="section-title">Il nostro alloggio</h2>
                    <p class="section-subtitle">Dove vivremo la nostra avventura romana</p>
                </div>
                
                <div class="accommodation-card">
                    <div class="accommodation-header">
                        <h3 class="accommodation-name">HostClean | Appartamento enorme vicino allo Stadio Olimpico</h3>
                    </div>
                    
                    <div class="accommodation-content">
                        <div class="info-grid">
                            <div class="info-item">
                                <i class="fas fa-users info-icon"></i>
                                <div class="info-text">
                                    <div class="info-label">Capacità</div>
                                    <div class="info-value">Appartamento spazioso<br>perfetto per la gilda</div>
                                </div>
                            </div>
                            <div class="info-item">
                                <i class="fas fa-star info-icon"></i>
                                <div class="info-text">
                                    <div class="info-label">Caratteristiche</div>
                                    <div class="info-value">Appartamento nuovo<br>ottimi collegamenti</div>
                                </div>
                            </div>
                            <div class="info-item">
                                <i class="fas fa-subway info-icon"></i>
                                <div class="info-text">
                                    <div class="info-label">Posizione</div>
                                    <div class="info-value">Vicino allo Stadio Olimpico<br>ben collegato al centro</div>
                                </div>
                            </div>
                        </div>
                        
                        <div style="text-align: center;">
                            <a href="https://www.airbnb.it/rooms/1379796091111192995?source_impression_id=p3_1752326554_P3D5BfqPKEvCwhQY" 
                               target="_blank" class="cta-button">
                                <i class="fab fa-airbnb"></i> Visualizza su Airbnb
                            </a>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Places Section -->
            <section class="section">
                <div class="section-header">
                    <h2 class="section-title">Luoghi da scoprire</h2>
                    <p class="section-subtitle">I tesori di Roma che ci aspettano</p>
                </div>
                
                <div class="map-container">
                    <iframe src="https://www.openstreetmap.org/export/embed.html?bbox=12.4489%2C41.9320%2C12.4580%2C41.9370&layer=mapnik&marker=41.9342%2C12.4537" 
                            allowfullscreen="" loading="lazy"></iframe>
                </div>
                
                <div class="map-actions">
                    <a href="https://maps.google.com/maps?q=Via+Unione+Sovietica,+14,+00196+Roma+RM,+Italia" 
                       target="_blank" class="cta-button">
                        <i class="fas fa-map-marked-alt"></i> Apri in Google Maps
                    </a>
                    <a href="https://maps.app.goo.gl/D768k3SEKvjRRDrx9" 
                       target="_blank" class="cta-button secondary">
                        <i class="fas fa-route"></i> Mappa completa luoghi
                    </a>
                </div>
                
                <div class="places-grid">
                    <div class="place-card">
                        <div class="place-content">
                            <h3 class="place-name">Colosseo</h3>
                            <p class="place-description">L'anfiteatro più famoso al mondo, simbolo dell'antica Roma. Un viaggio indietro nel tempo tra gladiatori e imperatori.</p>
                        </div>
                    </div>
                    
                    <div class="place-card">
                        <div class="place-content">
                            <h3 class="place-name">Fontana di Trevi</h3>
                            <p class="place-description">La fontana barocca più spettacolare di Roma. Lanciate una moneta e esprimete un desiderio per assicurarvi il ritorno!</p>
                        </div>
                    </div>
                    
                    <div class="place-card">
                        <div class="place-content">
                            <h3 class="place-name">Pantheon</h3>
                            <p class="place-description">Capolavoro dell'architettura romana antica, dedicato a tutti gli dei. La sua cupola perfetta è ancora oggi un mistero ingegneristico.</p>
                        </div>
                    </div>
                    
                    <div class="place-card">
                        <div class="place-content">
                            <h3 class="place-name">Piazza di Spagna</h3>
                            <p class="place-description">Una delle piazze più eleganti di Roma, con la celebre scalinata di Trinità dei Monti. Perfetta per una sosta romantica.</p>
                        </div>
                    </div>
                    
                    <div class="place-card">
                        <div class="place-content">
                            <h3 class="place-name">Città del Vaticano</h3>
                            <p class="place-description">Il più piccolo stato del mondo, custode di tesori artistici inestimabili. I Musei Vaticani e la Cappella Sistina vi lasceranno senza fiato.</p>
                        </div>
                    </div>
                    
                    <div class="place-card">
                        <div class="place-content">
                            <h3 class="place-name">Trastevere</h3>
                            <p class="place-description">Il quartiere più autentico di Roma, con le sue stradine acciottolate e i ristorantini tipici. La Roma vera, quella del cuore.</p>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Gallery Section -->
            <section class="section">
                <div class="section-header">
                    <h2 class="section-title">I nostri ricordi</h2>
                    <p class="section-subtitle">Qui raccoglieremo i momenti più belli del nostro viaggio</p>
                </div>
                
                <div class="gallery-placeholder">
                    <div class="gallery-icon">
                        <i class="fas fa-camera"></i>
                    </div>
                    <h3 class="gallery-title">Galleria delle avventure</h3>
                    <p class="gallery-text">Le foto dei nostri ricordi romani verranno aggiunte qui durante e dopo il viaggio</p>
                </div>
            </section>
        </div>
    </main>

    <!-- Music Section -->
    <section class="section">
        <div class="container">
            <div class="section-header">
                <h2 class="section-title">Colonna sonora del viaggio</h2>
                <p class="section-subtitle">La musica che accompagnerà le nostre avventure</p>
            </div>
            
            <div style="text-align: center; background: white; padding: 2rem; border-radius: 16px; box-shadow: 0 8px 30px rgba(0, 0, 0, 0.08);">
                <div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden;">
                    <iframe 
                        src="https://www.youtube.com/embed/SSYGILOL-tg?list=RDSSYGILOL-tg" 
                        style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; border-radius: 12px;"
                        allowfullscreen>
                    </iframe>
                </div>
                <p style="margin-top: 1rem; color: #6c757d; font-style: italic;">
                    🎵 Premi play per immergerti nell'atmosfera di Final Fantasy XIV
                </p>
            </div>
        </div>
    </section>

    <footer>
        <div class="container">
            <p class="footer-quote">
                "For the Sprouts, the Braves, and the Veteran Sparks" 
                <span class="sparkle">✨</span>
            </p>
        </div>
    </footer>

    <script>
        // Countdown Timer
        function updateCountdown() {
            const targetDate = new Date('2025-09-06T12:00:00').getTime();
            const now = new Date().getTime();
            const difference = targetDate - now;

            if (difference > 0) {
                const days = Math.floor(difference / (1000 * 60 * 60 * 24));
                const hours = Math.floor((difference % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
                const minutes = Math.floor((difference % (1000 * 60 * 60)) / (1000 * 60));
                const seconds = Math.floor((difference % (1000 * 60)) / 1000);

                document.getElementById('days').textContent = days;
                document.getElementById('hours').textContent = hours;
                document.getElementById('minutes').textContent = minutes;
                document.getElementById('seconds').textContent = seconds;
            } else {
                document.getElementById('days').textContent = '0';
                document.getElementById('hours').textContent = '0';
                document.getElementById('minutes').textContent = '0';
                document.getElementById('seconds').textContent = '0';
                
                document.querySelector('.countdown-title').textContent = 'Siamo a Roma! 🎉';
            }
        }

        // Update countdown every second
        setInterval(updateCountdown, 1000);
        updateCountdown(); // Initial call

        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
