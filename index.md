
<html lang="fa">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>موبایل مصطفی</title>
    <style>
        body {
            font-family: 'Vazir', 'Tahoma', sans-serif;
            direction: rtl;
            text-align: center;
            background: linear-gradient(135deg, #e0eafc, #cfdef3);
            color: #212529;
            margin: 0;
            padding: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            overflow: hidden;
        }
        
        .content-box {
            background: rgba(255, 255, 255, 0.9);
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.19), 0 6px 6px rgba(0, 0, 0, 0.23);
            animation: fadeIn 1s ease-in-out;
            width: 80%;
            max-width: 600px;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        h1 {
            font-size: 3em;
            color: #0056b3;
            margin-bottom: 30px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
        }
        
        ul {
            list-style-type: none;
            padding: 0;
        }

        li {
            font-size: 1.4em;
            margin: 15px 0;
            line-height: 1.6;
            position: relative;
            padding-right: 30px; /* فضا برای آیکون */
        }

        li::before {
            content: '✔';
            position: absolute;
            right: 0;
            color: #28a745; /* رنگ سبز برای تیک */
            font-weight: bold;
        }
        
        a {
            color: #d9534f;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s ease;
        }
        
        a:hover {
            color: #c9302c;
            text-decoration: underline;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.1);
        }

        .contact-info {
            margin-top: 30px;
            font-size: 1.2em;
        }
    </style>
</head>
<body>
    <div class="content-box">
        <h1>موبایل مصطفی</h1>
        <ul>
            <li>کلیه خدمات تلفن همراه</li>
            <li>تعمیرات تخصصی نرم‌افزار و سخت‌افزار</li>
            <li>نمایندگی ایرانسل و رایتل</li>
            <li>فروش اپل آیدی</li>
            <li>لوازم جانبی</li>
        </ul>
        <div class="contact-info">
            <p>تماس با ما: <a href="tel:09354811944">09354811944</a></p>
        </div>
    </div>
</body>
</html>
