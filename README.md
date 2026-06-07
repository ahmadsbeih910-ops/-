<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>سارة هل تقبلين؟</title>
    <style>
        body {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            background-color: #ffe6f2;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            overflow: hidden;
        }
        .container {
            text-align: center;
            background: white;
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }
        h1 {
            color: #ff4d94;
            font-size: 28px;
            margin-bottom: 20px;
        }
        .gif-container img {
            width: 200px;
            border-radius: 10px;
            margin-bottom: 20px;
        }
        .buttons {
            display: flex;
            justify-content: center;
            gap: 20px;
            position: relative;
            height: 60px;
            align-items: center;
        }
        button {
            padding: 12px 30px;
            font-size: 18px;
            border: none;
            border-radius: 25px;
            cursor: pointer;
            transition: all 0.3s ease;
            font-weight: bold;
        }
        #yesBtn {
            background-color: #ff4d94;
            color: white;
        }
        #yesBtn:hover {
            transform: scale(1.1);
            background-color: #e60067;
        }
        #noBtn {
            background-color: #b3b3b3;
            color: white;
            position: absolute;
        }
    </style>
</head>
<body>

    <div class="container">
        <!-- يمكنك استبدال رابط الصورة برابط جيف للقطط اللطيفة المماثلة للصورة -->
        <div class="gif-container">
            <img src="https://giphy.com" alt="Cute Cat">
        </div>
        
        <h1>سارة تحبيني لو لا؟ 💖</h1>
        
        <div class="buttons">
            <button id="yesBtn" onclick="accepted()">نعم</button>
            <button id="noBtn" onmouseover="moveButton()" onclick="moveButton()">لا</button>
        </div>
    </div>

    <script>
        function moveButton() {
            const noBtn = document.getElementById('noBtn');
            // حساب أبعاد عشوائية لهروب الزر داخل الشاشة
            const x = Math.random() * (window.innerWidth - noBtn.offsetWidth - 50);
            const y = Math.random() * (window.innerHeight - noBtn.offsetHeight - 50);
            
            noBtn.style.position = 'fixed';
            noBtn.style.left = x + 'px';
            noBtn.style.top = y + 'px';
        }

        function accepted() {
            alert('كنت عارف إنك بتحبيني يا سارة! 🥰❤️');
        }
    </script>

</body>
</html># -
