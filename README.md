# access<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Доступ</title>

    <style>
        body {
            margin: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background: linear-gradient(135deg, #f5f7fa, #e4e8ee);
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
        }

        .box {
            background: #ffffff;
            padding: 30px;
            border-radius: 16px;
            width: 90%;
            max-width: 320px;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }

        h2 {
            margin-bottom: 20px;
            font-weight: 500;
            color: #333;
        }

        input {
            width: 100%;
            padding: 14px;
            font-size: 18px;
            text-align: center;
            border-radius: 12px;
            border: 1px solid #ddd;
            outline: none;
        }

        input:focus {
            border-color: #007aff;
        }

        .error {
            margin-top: 12px;
            color: #ff3b30;
            font-size: 14px;
            display: none;
        }
    </style>
</head>
<body>

    <div class="box">
        <h2>Введите код</h2>
        <input type="tel" id="code" maxlength="4" placeholder="••••" autofocus>
        <div class="error" id="error">Неверный код</div>
    </div>

    <script>
        const input = document.getElementById("code");
        const error = document.getElementById("error");

        input.addEventListener("input", () => {
            if (input.value.length === 4) {
                if (input.value === "2026") {
                    window.location.href = "https://t.me/+Jhwx3IgNcYgxODQy";
                } else {
                    error.style.display = "block";
                    input.value = "";
                }
            }
        });
    </script>

</body>
</html>
