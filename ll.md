[
<html lang="fa">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>تبدیل لینک گوگل درایو به لینک مستقیم و QR کد</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f9;
            color: #333;
            text-align: center;
            padding: 20px;
        }

        h2 {
            color: #4CAF50;
        }

        label {
            display: block;
            margin-top: 20px;
            font-size: 1.1em;
        }

        input[type="text"] {
            width: 70%;
            padding: 10px;
            margin: 10px 0;
            font-size: 1em;
            border: 1px solid #ccc;
            border-radius: 5px;
            box-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);
        }

        button {
            background-color: #4CAF50;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 1em;
            cursor: pointer;
            border-radius: 5px;
            margin-top: 10px;
            transition: background-color 0.3s ease;
        }

        button:hover {
            background-color: #45a049;
        }

        button:active {
            background-color: #3e8e41;
        }

        .container {
            max-width: 600px;
            margin: 0 auto;
            background-color: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .output {
            margin-top: 20px;
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 10px;
        }

        .output input {
            width: 70%;
            padding: 10px;
        }

        #qrcode {
            margin-top: 20px;
        }

        .input-group {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 10px;
        }

    </style>
    <!-- کتابخانه QRCode.js -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js"></script>
    <script>
        function convertLink() {
            var inputLink = document.getElementById("driveLink").value;
            var fileId = inputLink.match(/[-\w]{25,}/);
            if (fileId) {
                var directLink = "https://drive.google.com/uc?export=download&id=" + fileId[0];
                document.getElementById("directLink").value = directLink;

                // ساخت QR کد
                var qrcodeContainer = document.getElementById("qrcode");
                qrcodeContainer.innerHTML = ""; // پاک کردن QR کد قبلی
                new QRCode(qrcodeContainer, {
                    text: directLink,
                    width: 128,
                    height: 128,
                    colorDark: "#333",
                    colorLight: "#ffffff",
                });
            } else {
                document.getElementById("directLink").value = "لینک معتبر نیست!";
                document.getElementById("qrcode").innerHTML = ""; // پاک کردن QR کد در صورت نامعتبر بودن لینک
            }
        }

        function copyToClipboard() {
            var copyText = document.getElementById("directLink");
            copyText.select();
            copyText.setSelectionRange(0, 99999); // برای مرورگرهای موبایل
            document.execCommand("copy");
            alert("لینک کپی شد: " + copyText.value);
        }

        async function pasteFromClipboard() {
            try {
                const text = await navigator.clipboard.readText();
                document.getElementById("driveLink").value = text;
            } catch (err) {
                alert("دسترسی به کلیپ‌بورد امکان‌پذیر نیست.");
            }
        }
    </script>
</head>
<body>
    <div class="container">
        <h2>تبدیل لینک گوگل درایو به لینک مستقیم و QR کد</h2>
        <label for="driveLink">لینک اشتراک‌گذاری گوگل درایو را وارد کنید:</label>
        <div class="input-group">
            <input type="text" id="driveLink" placeholder="https://drive.google.com/file/d/FILE_ID/view?usp=sharing">
            <button onclick="pasteFromClipboard()">Paste</button>
        </div>
        <button onclick="convertLink()">تبدیل</button>
        <div class="output">
            <input type="text" id="directLink" readonly placeholder="لینک مستقیم اینجا نمایش داده می‌شود">
            <button onclick="copyToClipboard()">کپی</button>
        </div>
        <div id="qrcode"></div> <!-- محلی برای نمایش QR کد -->
    </div>
</body>
</html>
](https://drive.google.com/file/d/1xTpwIeqkWATnXezVtMidlQYrC9VfBdtK/view?usp=sharing)