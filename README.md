<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <title>Tool Center</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background: #0f172a;
            color: #e5e7eb;
        }

        header {
            background: #020617;
            padding: 15px;
            text-align: center;
            font-size: 22px;
            font-weight: bold;
            color: #38bdf8;
        }

        nav {
            display: flex;
            justify-content: center;
            gap: 15px;
            background: #020617;
            padding: 10px;
        }

        nav button {
            background: #1e293b;
            color: white;
            border: none;
            padding: 10px 18px;
            cursor: pointer;
            border-radius: 6px;
            font-size: 15px;
        }

        nav button:hover {
            background: #38bdf8;
            color: black;
        }

        .container {
            padding: 20px;
            max-width: 800px;
            margin: auto;
        }

        .tool {
            display: none;
            background: #020617;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px #000;
        }

        .tool h2 {
            color: #38bdf8;
        }

        footer {
            text-align: center;
            padding: 15px;
            color: #94a3b8;
            font-size: 13px;
        }
    </style>
</head>
<body>

<header>
    TOOL CENTER
</header>

<nav>
    <button onclick="showTool('sicbo')">Tool Sicbo</button>
    <button onclick="showTool('txv2')">Tool TX V2</button>
</nav>

<div class="container">

    <div id="sicbo" class="tool">
        <h2>🎲 Tool Sicbo</h2>
        <p>Chức năng:</p>
        <ul>
            <li>Dự đoán Tài / Xỉu</li>
            <li>Thống kê lịch sử</li>
            <li>Tỷ lệ thắng theo cầu</li>
        </ul>
        <p><b>Trạng thái:</b> Đang phát triển</p>
    </div>

    <div id="txv2" class="tool">
        <h2>⚡ Tool TX V2</h2>
        <p>Chức năng:</p>
        <ul>
            <li>Phân tích cầu TX</li>
            <li>Tự động gợi ý</li>
            <li>Giao diện tối ưu</li>
        </ul>
        <p><b>Phiên bản:</b> v2.0</p>
    </div>

</div>

<footer>
    © 2025 | Tool Web chạy trên GitHub Pages
</footer>

<script>
    function showTool(id) {
        document.querySelectorAll('.tool').forEach(tool => {
            tool.style.display = 'none';
        });
        document.getElementById(id).style.display = 'block';
    }

    // Hiện mặc định tool đầu tiên
    showTool('sicbo');
</script>

</body>
</html>
