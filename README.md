<!DOCTYPE html>
<html lang="uk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Feedback Board</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(135deg, #a855f7, #ec4899, #f97316);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 0;
            padding: 20px;
            box-sizing: border-box;
        }
        .container {
            background: rgba(255, 255, 255, 0.95);
            padding: 30px;
            border-radius: 16px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.2);
            width: 100%;
            max-width: 450px;
        }
        h2 {
            margin-top: 0;
            color: #1f2937;
            text-align: center;
        }
        .form-group {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            color: #4b5563;
            font-weight: bold;
        }
        input, textarea {
            width: 100%;
            padding: 10px;
            border: 1px solid #d1d5db;
            border-radius: 8px;
            box-sizing: border-box;
            font-size: 14px;
        }
        textarea {
            resize: vertical;
            height: 100px;
        }
        button {
            width: 100%;
            background: #ec4899;
            color: white;
            border: none;
            padding: 12px;
            border-radius: 8px;
            font-size: 16px;
            font-weight: bold;
            cursor: pointer;
            transition: background 0.2s;
        }
        button:hover {
            background: #db2777;
        }
    </style>
</head>
<body>

<div class="container">
    <h2>Шкільна дошка відгуків 📝</h2>
    
    <form action="https://api.web3forms.com/submit" method="POST">
        <!-- ВСТАВ СВІЙ КЛЮЧ WEB3FORMS У VALUE НИЖЧЕ -->
        <input type="hidden" name="access_key" value="ТВІЙ_WEB3FORMS_KEY_СЮДИ">
        
        <div class="form-group">
            <label for="name">Ваше ім'я або клас (необов'язково):</label>
            <input type="text" id="name" name="name" placeholder="Наприклад: Артем (8 клас)">
        </div>

        <div class="form-group">
            <label for="message">Ваше повідомлення або пропозиція:</label>
            <textarea id="message" name="message" required placeholder="Напишіть свій відгук тут..."></textarea>
        </div>

        <button type="submit">Надіслати відгук</button>
    </form>
</div>

</body>
</html># feedback-board
