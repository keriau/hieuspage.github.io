<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Thiệp Sinh Nhật - Thảo béo</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: 'Arial', sans-serif;
            background: linear-gradient(135deg, #ff9a9e, #fad0c4);
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            overflow: hidden;
            color: #333;
        }
        .card {
            background: white;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
            border-radius: 15px;
            padding: 20px;
            width: 80%;
            max-width: 600px;
            text-align: center;
            animation: fadeIn 1.5s ease;
            position: relative;
            overflow: hidden;
        }

        .balloons {
            position: absolute;
            top: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 100%;
            height: 100%;
            pointer-events: none;
        }

        .balloon {
            position: absolute;
            width: 50px;
            height: 70px;
            background: radial-gradient(circle, #ff6f61, #ff4757);
            border-radius: 50%;
            animation: float 6s ease-in-out infinite;
        }

        .balloon:nth-child(2) {
            background: radial-gradient(circle, #2ed573, #1e90ff);
            animation-delay: 2s;
        }

        .balloon:nth-child(3) {
            background: radial-gradient(circle, #ffa502, #ff6348);
            animation-delay: 4s;
        }

        @keyframes float {
            0% {
                transform: translateX(-50%) translateY(100%);
                opacity: 0;
            }
            50% {
                opacity: 1;
            }
            100% {
                transform: translateX(-50%) translateY(-100%);
                opacity: 0;
            }
        }

        h1 {
            color: #e63946;
            font-size: 2.5rem;
            animation: popIn 1s ease-out;
        }

        h2 {
            color: #457b9d;
            font-size: 1.5rem;
            margin: 10px 0;
            animation: fadeIn 2s ease;
        }

        p {
            margin: 15px 0;
            line-height: 1.8;
            animation: fadeIn 2.5s ease;
        }

        .footer {
            margin-top: 20px;
            font-size: 1rem;
            color: #2a9d8f;
            animation: fadeIn 3s ease;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes popIn {
            0% {
                transform: scale(0.8);
                opacity: 0;
            }
            100% {
                transform: scale(1);
                opacity: 1;
            }
        }
    </style>
</head>
<body>
    <div class="balloons">
        <div class="balloon" style="left: 20%;"></div>
        <div class="balloon" style="left: 50%;"></div>
        <div class="balloon" style="left: 80%;"></div>
    </div>
    <div class="card">
        <h1>Chúc mừng sinh nhật, Thảo béo!</h1>
        <h2>Từ: Hiếu</h2>
        <p>
            HÔM NAY SINH NHẬT CHỊ BÉO ĐÃ TỚI<br>
            CHÚC BÉO TUỔI MỚI, CON ĐƯỜNG PHẤP PHỚI<br>
            CƠ HỘI ÀO TỚI RỒI ÔM KHÔNG RỜI<br>
            VÍ THÊM NHIỀU HỜI, TÀI KHOẢN THÊM LỜI<br><br>

            CUỘC SỐNG THẢNH THƠI, ĐƯỢC HẾT MÌNH CHƠI<br>
            BÊN NGOÀI TẢ TƠI THÌ VỀ XẢ HƠI<br>
            SỨC KHOẺ KHÔNG RỜI, NỤ CƯỜI KHÔNG VƠI<br>
            HÍT SÂU MỘT HƠI, LÀM ĐIỀU MÌNH “MƠI”<br><br>

            CÒN BỒ THÌ THÔI, CÓ VẺ XA XÔI<br>
            NHƯNG BÌNH THƯỜNG THÔI, CỨ BÌNH TĨNH THÔI<br>
            DẪU CÓ SỤC SÔI VẪN PHẢI LỰA MỒI<br>
            ĐỪNG QUÁ BỒI HỒI RỒI LỰA NGƯỜI TỒI<br>
        </p>
        <div class="footer">Chúc một ngày thật vui và ý nghĩa!</div>
    </div>
</body>
</html>
