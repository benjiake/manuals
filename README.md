<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cai Lab Product Support</title>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            background-color: #f9f9f9;
            color: #333;
            margin: 0;
            padding: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        /* 顶部合规声明 - 灰色小字，降低侵略性 */
        .compliance-note {
            background-color: #fff;
            border: 1px solid #e0e0e0;
            border-radius: 8px;
            padding: 12px;
            font-size: 12px;
            color: #666;
            text-align: center;
            max-width: 400px;
            margin-bottom: 30px;
            line-height: 1.4;
        }

        h1 {
            font-size: 18px;
            margin-bottom: 20px;
            color: #222;
        }

        /* 说明书列表样式 */
        .manual-list {
            width: 100%;
            max-width: 400px;
            display: flex;
            flex-direction: column;
            gap: 10px;
        }

        .manual-btn {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background-color: #fff;
            padding: 15px 20px;
            border-radius: 8px;
            text-decoration: none;
            color: #333;
            box-shadow: 0 1px 3px rgba(0,0,0,0.05);
            transition: background-color 0.2s;
            border: 1px solid #eee;
            font-size: 14px;
            font-weight: 500;
        }

        .manual-btn:hover {
            background-color: #f0f0f0;
        }

        .icon {
            color: #888;
        }

        /* 底部支持按钮 */
        .support-section {
            margin-top: 40px;
            text-align: center;
            width: 100%;
        }

        .support-btn {
            background-color: #333;
            color: #fff;
            border: none;
            padding: 12px 30px;
            border-radius: 25px;
            font-size: 14px;
            cursor: pointer;
            box-shadow: 0 2px 5px rgba(0,0,0,0.2);
        }

        .support-btn:active {
            transform: scale(0.98);
        }

        /* 弹窗样式 */
        .modal-overlay {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5);
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }

        .modal-content {
            background: white;
            padding: 25px;
            border-radius: 12px;
            text-align: center;
            width: 80%;
            max-width: 300px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.3);
        }

        .email-text {
            font-size: 16px;
            font-weight: bold;
            margin: 15px 0;
            word-break: break-all;
            color: #333;
            padding: 10px;
            background: #f4f4f4;
            border-radius: 4px;
            user-select: text; /* 允许用户复制 */
        }

        .close-btn {
            margin-top: 15px;
            background: transparent;
            border: 1px solid #ccc;
            padding: 8px 20px;
            border-radius: 20px;
            cursor: pointer;
            font-size: 14px;
        }
    </style>
</head>
<body>

    <div class="compliance-note">
        For any issues, you can also contact us via the Temu app's Message Center for a faster resolution.
    </div>

    <h1>Product Manuals (PDF)</h1>

    <div class="manual-list">
        <a href="https://drive.google.com/file/d/1S2mjOAceT_FHzPprjji-CeDzd_G-_iZu/view?usp=drive_link" class="manual-btn" target="_blank">
            <span>PLA Matte Manual</span>
            <span class="icon">⬇</span>
        </a>

        <a href="https://drive.google.com/file/d/15Y0XXCJ1Lg1jKd4s6Z8T2xbDvPU9AwRP/view?usp=drive_link" class="manual-btn" target="_blank">
            <span>PLA+Bio Manual</span>
            <span class="icon">⬇</span>
        </a>

        <a href="https://drive.google.com/file/d/1ICeYh5Yy4ZRMjEth-vyw_68Dso-Xok1r/view?usp=drive_link" class="manual-btn" target="_blank">
            <span>PLA Silk Manual</span>
            <span class="icon">⬇</span>
        </a>

        <a href="https://drive.google.com/file/d/1iVgSAMeONdy6AcBLYtQsdtD9hjYPp1HA/view?usp=drive_link" class="manual-btn" target="_blank">
            <span>PETG Manual</span>
            <span class="icon">⬇</span>
        </a>

        <a href="https://drive.google.com/file/d/12YqXuNiCBfPU3vmChnkKBRqtrHdOkoHP/view?usp=drive_link" class="manual-btn" target="_blank">
            <span>PETG-CF (Carbon Fiber) Manual</span>
            <span class="icon">⬇</span>
        </a>
    </div>

    <div class="support-section">
        <button class="support-btn" onclick="openModal()">Contact Support</button>
    </div>

    <div class="modal-overlay" id="contactModal">
        <div class="modal-content">
            <h3>Need Help?</h3>
            <p style="font-size: 13px; color:#666; margin-bottom:5px;">You can email us at:</p>
            <div class="email-text">2209066217@qq.com</div>
            <p style="font-size: 12px; color:#999;">Long press to copy</p>
            <button class="close-btn" onclick="closeModal()">Close</button>
        </div>
    </div>

    <script>
        function openModal() {
            document.getElementById('contactModal').style.display = 'flex';
        }

        function closeModal() {
            document.getElementById('contactModal').style.display = 'none';
        }

        // 点击弹窗外部也可以关闭
        window.onclick = function(event) {
            var modal = document.getElementById('contactModal');
            if (event.target == modal) {
                modal.style.display = "none";
            }
        }
    </script>
</body>
</html>
