<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Мой сайт-визитка</title>
    <style>
        /* Общие стили */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }
        
        body {
            line-height: 1.6;
            color: #333;
            background-color: #f9f9f9;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        section {
            padding: 60px 0;
        }
        
        h1, h2, h3 {
            margin-bottom: 20px;
            color: #2c3e50;
        }
        
        p {
            margin-bottom: 15px;
        }
        
        a {
            text-decoration: none;
            color: #3498db;
            transition: color 0.3s;
        }
        
        a:hover {
            color: #2980b9;
        }
        
        .btn {
            display: inline-block;
            padding: 12px 25px;
            background-color: #3498db;
            color: white;
            border-radius: 5px;
            text-transform: uppercase;
            font-weight: bold;
            transition: background-color 0.3s;
        }
        
        .btn:hover {
            background-color: #2980b9;
            color: white;
        }
        
        /* Навигация */
        header {
            background-color: #2c3e50;
            color: white;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }
        
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }
        
        .logo {
            font-size: 24px;
            font-weight: bold;
        }
        
        .nav-links {
            display: flex;
            list-style: none;
        }
        
        .nav-links li {
            margin-left: 30px;
        }
        
        .nav-links a {
            color: white;
            font-weight: 500;
        }
        
        .nav-links a:hover {
            color: #3498db;
        }
        
        /* Главный баннер */
        .hero {
            height: 100vh;
            display: flex;
            align-items: center;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            text-align: center;
            margin-top: 60px;
        }
        
        .hero-content h1 {
            font-size: 48px;
            margin-bottom: 20px;
            color: white;
        }
        
        .hero-content p {
            font-size: 20px;
            margin-bottom: 30px;
        }
        
        /* О себе */
        .about {
            background-color: white;
        }
        
        .about-content {
            display: flex;
            align-items: center;
            gap: 40px;
        }
        
        .about-text {
            flex: 1;
        }
        
        .about-image {
            flex: 1;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .about-image img {
            width: 100%;
            height: auto;
            display: block;
        }
        
        /* Услуги */
        .services {
            background-color: #f8f9fa;
            text-align: center;
        }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .service-card {
            background: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s;
        }
        
        .service-card:hover {
            transform: translateY(-10px);
        }
        
        .service-card h3 {
            color: #2c3e50;
        }
        
        .service-icon {
            font-size: 40px;
            margin-bottom: 20px;
            color: #3498db;
        }
        
        /* Контакты */
        .contact {
            background-color: white;
        }
        
        .contact-form {
            max-width: 600px;
            margin: 0 auto;
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }
        
        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 16px;
        }
        
        .form-group textarea {
            min-height: 150px;
            resize: vertical;
        }
        
        /* Футер */
        footer {
            background-color: #2c3e50;
            color: white;
            padding: 40px 0;
            text-align: center;
        }
        
        .footer-content {
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        
        .social-links {
            margin: 20px 0;
        }
        
        .social-links a {
            color: white;
            margin: 0 10px;
            font-size: 20px;
        }
        
        /* Адаптивность */
        @media (max-width: 768px) {
            .about-content {
                flex-direction: column;
            }
            
            .nav-links {
                display: none;
            }
            
            .hero-content h1 {
                font-size: 36px;
            }
            
            .hero-content p {
                font-size: 18px;
            }
        }
    </style>
</head>
<body>
    <!-- Шапка с навигацией -->
    <header>
        <div class="container">
            <nav>
                <div class="logo">МоеПортфолио</div>
                <ul class="nav-links">
                    <li><a href="#home">Главная</a></li>
                    <li><a href="#about">Обо мне</a></li>
                    <li><a href="#services">Услуги</a></li>
                    <li><a href="#contact">Контакты</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Главный баннер -->
    <section class="hero" id="home">
        <div class="container">
            <div class="hero-content">
                <h1>Привет, я Ева Ярославовна</h1>
                <p>Веб-разработчик и дизайнер с страстью к созданию красивых и функциональных сайтов</p>
                <a href="#contact" class="btn">Связаться со мной</a>
            </div>
        </div>
    </section>

    <!-- О себе -->
    <section class="about" id="about">
        <div class="container">
            <h2>Обо мне</h2>
            <div class="about-content">
                <div class="about-text">
                    <p>Привет! Меня зовут Ева, и я занимаюсь веб-разработкой уже 3 года. Я специализируюсь на создании современных, адаптивных и удобных веб-сайтов.</p>
                    <p>Мой подход сочетает в себе креативный дизайн и техническое совершенство. Я постоянно изучаю новые технологии и методы, чтобы предлагать клиентам только лучшие решения.</p>
                    <p>В свободное время я люблю читать профессиональную литературу, участвовать в IT-сообществах и заниматься фотографией.</p>
                </div>
                <div class="about-image">
                    <img src="https://placehold.co/600x400/3498db/ffffff" alt="Мое фото">
                </div>
            </div>
        </div>
    </section>

    <!-- Услуги -->
    <section class="services" id="services">
        <div class="container">
            <h2>Мои услуги</h2>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">💻</div>
                    <h3>Веб-разработка</h3>
                    <p>Создание современных и адаптивных веб-сайтов с использованием HTML5, CSS3, JavaScript и современных фреймворков.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">🎨</div>
                    <h3>Веб-дизайн</h3>
                    <p>Разработка уникального дизайна, который отражает характер вашего бизнеса и привлекает внимание посетителей.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">📱</div>
                    <h3>Мобильная адаптация</h3>
                    <p>Адаптация сайтов для корректного отображения на мобильных устройствах и планшетах.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Контакты -->
    <section class="contact" id="contact">
        <div class="container">
            <h2>Свяжитесь со мной</h2>
            <div class="contact-form">
                <form>
                    <div class="form-group">
                        <label for="name">Ваше имя</label>
                        <input type="text" id="name" placeholder="Введите ваше имя" required>
                    </div>
                    <div class="form-group">
                        <label for="email">Ваш email</label>
                        <input type="email" id="email" placeholder="Введите ваш email" required>
                    </div>
                    <div class="form-group">
                        <label for="message">Сообщение</label>
                        <textarea id="message" placeholder="Введите ваше сообщение" required></textarea>
                    </div>
                    <button type="submit" class="btn">Отправить сообщение</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Футер -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="social-links">
                    <a href="#">VK</a>
                    <a href="#">Telegram</a>
                    <a href="#">GitHub</a>
                </div>
                <p>&copy; 2023 МоеПортфолио. Все права защищены.</p>
            </div>
        </div>
    </footer>

    <script>
        // Плавная прокрутка к якорям
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });
        
        // Обработка формы
        const contactForm = document.querySelector('.contact-form form');
        if (contactForm) {
            contactForm.addEventListener('submit', function(e) {
                e.preventDefault();
                alert('Спасибо за ваше сообщение! Я свяжусь с вами в ближайшее время.');
                this.reset();
            });
        }
    </script>
</body>
</html>
