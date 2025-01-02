<!DOCTYPE html>
<html lang="fa">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>موبایل مصطفی</title>
    <style>
        body {
            font-family: Tahoma, Arial, sans-serif;
            direction: rtl;
            text-align: center;
            background-color: #f9f9f9;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #0056b3;
            color: white;
            padding: 30px;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        header h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
        }
        header p {
            font-size: 1.2em;
        }
        .content {
            padding: 40px 20px;
        }
        .services {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
            margin: 0 auto;
            max-width: 900px;
        }
        .service-item {
            border: 1px solid #e1e1e1;
            border-radius: 8px;
            padding: 20px;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }
        .service-item:hover {
            transform: translateY(-10px);
        }
        .service-item p {
            font-size: 1.1em;
            margin: 10px 0;
        }
        .service-item:nth-child(1) {
            background-color: #f8d7da; /* رنگ قرمز کمرنگ */
        }
        .service-item:nth-child(2) {
            background-color: #d1ecf1; /* رنگ آبی کمرنگ */
        }
        .service-item:nth-child(3) {
            background-color: #d4edda; /* رنگ سبز کمرنگ */
        }
        .service-item:nth-child(4) {
            background-color: #fff3cd; /* رنگ زرد کمرنگ */
        }
        .service-item:nth-child(5) {
            background-color: #e2e3e5; /* رنگ خاکی کمرنگ */
        }
        .service-item:nth-child(6) {
            background-color: #cce5ff; /* رنگ آبی روشن */
        }
        .contact-info {
            background-color: #e9ecef;
            padding: 20px;
            border-radius: 8px;
            margin: 40px 0;
            font-size: 18px;
        }
        .contact-info h3 {
            margin-bottom: 10px;
        }
        .contact-btn {
            display: inline-block;
            padding: 10px 30px;
            background-color: #007bff;
            color: white;
            font-size: 1.2em;
            border-radius: 5px;
            text-decoration: none;
            margin-top: 20px;
            transition: background-color 0.3s ease;
        }
        .contact-btn:hover {
            background-color: #0056b3;
        }
        footer {
            background-color: #343a40;
            color: white;
            padding: 15px;
            text-align: center;
        }
    </style>
</head>
<body>
    <header>
        <h1>موبایل مصطفی</h1>
        <p>کلیه خدمات تلفن همراه با کیفیت بالا</p>
    </header>

    <div class="content">
        <h2>خدمات ما</h2>
        <div class="services">
            <div class="service-item">
                <h3>فروش انواع تلفن همراه</h3>
                <p>با بهترین قیمت و کیفیت</p>
            </div>
            <div class="service-item">
                <h3>تعمیرات تلفن همراه</h3>
                <p>تعمیرات سخت‌افزاری و نرم‌افزاری</p>
            </div>
            <div class="service-item">
                <h3>لوازم جانبی</h3>
                <p>فروش لوازم جانبی اصل و با کیفیت</p>
            </div>
            <div class="service-item">
                <h3>فروش اپل آیدی</h3>
                <p>ساخت و فروش اپل آیدی امن</p>
            </div>
            <div class="service-item">
                <h3>خرید و فروش خط 912</h3>
                <p>خرید و فروش شماره‌های خاص</p>
            </div>
            <div class="service-item">
                <h3>نمایندگی ایرانسل و رایتل</h3>
                <p>خدمات مربوط به سیم‌کارت‌ها</p>
            </div>
        </div>

        <div class="contact-info">
            <h3>تماس با ما</h3>
            <p>برای اطلاعات بیشتر یا درخواست خدمات، با ما تماس بگیرید:</p>
            <p>شماره تماس: 09354811944</p>
            <a href="tel:09354811944" class="contact-btn">تماس با ما</a>
        </div>
    </div>

    <footer>
        <p>&copy; 2025 موبایل مصطفی - تمامی حقوق محفوظ است</p>
    </footer>
</body>
</html>
