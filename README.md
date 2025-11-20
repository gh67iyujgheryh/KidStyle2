<html lang="kk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>KidStyle — Балалар Киім Дүкені</title>

    <!-- Қазақша шрифт -->
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans:wght@300;400;500;600;700;800&display=swap&subset=cyrillic" rel="stylesheet">

    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: "Noto Sans", sans-serif; }

        body {
            background: linear-gradient(135deg, #ffd8e8, #d4f1ff, #ffe8c7);
            background-size: 300% 300%;
            animation: bgMove 12s infinite alternate;
        }

        @keyframes bgMove {
            0% { background-position: 0% 50%; }
            100% { background-position: 100% 50%; }
        }

        /* HEADER */
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 50px;
            backdrop-filter: blur(20px);
            background: rgba(255,255,255,0.35);
            border-bottom: 1px solid rgba(255,255,255,0.4);
            position: sticky;
            top: 0;
            z-index: 10;
        }

        .logo { font-size: 30px; font-weight: bold; color: #ff5fa2; }

        nav a {
            margin-left: 25px;
            text-decoration: none;
            font-weight: 600;
            color: #444;
        }
        nav a:hover { color: #ff5fa2; }

        /* HERO */
        .hero {
            padding: 130px 20px;
            text-align: center;
        }

        .hero-box {
            display: inline-block;
            background: rgba(255,255,255,0.3);
            padding: 60px;
            border-radius: 25px;
            backdrop-filter: blur(20px);
            border: 2px solid rgba(255,255,255,0.45);
        }

        .hero h1 { font-size: 60px; color: #ff3f8f; margin-bottom: 20px; }
        .hero p { font-size: 22px; margin-bottom: 30px; }

        .hero button {
            padding: 15px 34px;
            background: #ff5fa2;
            color: white;
            font-size: 20px;
            border-radius: 15px;
            border: none;
            cursor: pointer;
        }
        .hero button:hover { background: #ff3f8f; }

        /* PRODUCTS */
        .products { padding: 70px 20px; text-align: center; }
        .products h2 { font-size: 42px; margin-bottom: 40px; color: #ff5fa2; }

        .grid {
            display: flex;
            justify-content: center;
            gap: 30px;
            flex-wrap: wrap;
        }

        .item {
            width: 280px;
            padding: 25px;
            border-radius: 20px;
            background: rgba(255,255,255,0.45);
            backdrop-filter: blur(15px);
            border: 2px solid rgba(255,255,255,0.5);
            box-shadow: 0 10px 30px rgba(0,0,0,0.12);
        }

        .item img {
            width: 100%;
            height: 280px;
            object-fit: cover;
            border-radius: 15px;
            margin-bottom: 15px;
        }

        .item h3 { font-size: 22px; color: #ff3f8f; margin-bottom: 10px; }
        .price { font-size: 20px; font-weight: bold; margin-bottom: 10px; }

        /* ORDER FORM */
        .order {
            padding: 60px 20px;
            text-align: center;
        }
        .order h2 { font-size: 40px; color: #ff3f8f; margin-bottom: 30px; }

        .order-box {
            max-width: 550px;
            margin: auto;
            background: rgba(255,255,255,0.45);
            padding: 30px;
            border-radius: 20px;
            backdrop-filter: blur(15px);
        }

        input, select, textarea {
            width: 100%;
            padding: 14px;
            margin-bottom: 15px;
            border-radius: 10px;
            border: 1px solid #ddd;
            font-size: 16px;
        }

        button.order-btn {
            background: #ff3f8f;
            color: white;
            padding: 15px 25px;
            width: 100%;
            border: none;
            border-radius: 12px;
            font-size: 18px;
            cursor: pointer;
        }

        button.order-btn:hover {
            background: #ff236f;
        }

        /* CONTACTS */
        .contact {
            padding: 70px 20px;
            text-align: center;
        }

        .contact h2 {
            font-size: 40px;
            color: #ff3f8f;
            margin-bottom: 20px;
        }

        .contact p {
            font-size: 20px;
            margin-bottom: 10px;
        }

        .contact a {
            color: #ff3f8f;
            font-size: 22px;
            text-decoration: none;
        }

        footer {
            padding: 20px;
            background: rgba(255,255,255,0.35);
            text-align: center;
            margin-top: 40px;
            font-weight: bold;
        }
    </style>
</head>
<body>

<header>
    <div class="logo">KidStyle</div>
    <nav>
        <a href="#products">Тауарлар</a>
        <a href="#order">Заказ беру</a>
        <a href="#contact">Байланыс</a>
    </nav>
</header>

<!-- HERO -->
<section class="hero">
    <div class="hero-box">
        <h1>Балалар стилі жаңа деңгейде ✨</h1>
        <p>Сапалы, әдемі және жайлы киімдер.</p>
        <button onclick="location.href='#products'">Өнімдерді көру</button>
    </div>
</section>

<!-- PRODUCTS -->
<section class="products" id="products">
    <h2>Жаңа коллекциялар</h2>

    <div class="grid">
        <div class="item">
            <img src="https://img.freepik.com/premium-photo/pink-jacket-yellow-jumper-hanger-set-baby-clothes-accessories-spring-autumn-white-background-fashion-kids-outfit-flat-lay-top-view_479776-7507.jpg">
            <h3>Балалар футболкасы</h3>
            <p class="price">3 500 ₸</p>
        </div>

        <div class="item">
            <img src="https://xcdn.next.co.uk/common/items/default/default/itemimages/3_4Ratio/product/lge/N77198s.jpg?im=Resize,width=750">
            <h3>Қыздарға көйлек</h3>
            <p class="price">6 900 ₸</p>
        </div>

        <div class="item">
            <img src="https://ir.ozone.ru/s3/multimedia-7/c400/6719830819.jpg">
            <h3>Сәбилер костюмі</h3>
            <p class="price">5 200 ₸</p>
        </div>

        <div class="item">
            <img src="https://img.news-textile.ru/img/2020/01/detskaya-moda-na-zimu-v-2019-2020.jpg">
            <h3>Балалар курткасы</h3>
            <p class="price">12 500 ₸</p>
        </div>
    </div>
</section>

<!-- ORDER FORM -->
<section class="order" id="order">
    <h2>Заказ беру</h2>

    <div class="order-box">
        <input type="text" placeholder="Атыңыз" required>
        <input type="tel" placeholder="Телефон нөмірі" required>

        <select>
            <option>Өнімді таңдаңыз</option>
            <option>Балалар футболкасы</option>
            <option>Қыздарға көйлек</option>
            <option>Сәбилер костюмі</option>
            <option>Балалар курткасы</option>
        </select>

        <textarea rows="4" placeholder="Қосымша ақпарат"></textarea>

        <button class="order-btn" onclick="alert('Тапсырысыңыз қабылданды! Менеджер хабарласады 😊')">
            Заказ беру
        </button>
    </div>
</section>

<!-- CONTACTS -->
<section class="contact" id="contact">
    <h2>Байланыс</h2>

    <p>📞 Телефон: <a href="tel:+77000000000">+7 700 000 00 00</a></p>
    <p>📱 WhatsApp: <a href="https://wa.me/77000000000" target="_blank">Хабарласу</a></p>
    <p>📸 Instagram: <a href="#" target="_blank">@kidstyle_shop</a></p>
    <p>📍 Адрес: Алматы қ., Назарбаев даңғылы 120</p>
</section>

<footer>
    © 2025 KidStyle — Балалар киім дүкені  
</footer>

</body>
</html>
