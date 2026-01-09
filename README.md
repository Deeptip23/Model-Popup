# Model-Popup
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Modal Popup</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            min-height: 100vh;
            background: #f2f4f7;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        
        .open-btn {
            padding: 12px 20px;
            font-size: 16px;
            background: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s;
        }

        .open-btn:hover {
            background: #43a047;
        }

       
        .modal-overlay {
            position: fixed;
            top: 0;
            left: 0;
            height: 100%;
            width: 100%;
            background: rgba(0, 0, 0, 0.5);
            display: none;  
            justify-content: center;
            align-items: center;
        }

       
        .modal {
            background: white;
            width: 350px;
            border-radius: 8px;
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.3);
            overflow: hidden;
            animation: fadeIn 0.3s ease-in-out;
        }

        
        .modal-header {
            background: #4CAF50;
            color: white;
            padding: 12px 15px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .modal-header h2 {
            font-size: 18px;
        }

       
        .close-btn {
            background: none;
            border: none;
            font-size: 20px;
            color: white;
            cursor: pointer;
        }
        
        .modal-content {
            padding: 15px;
            font-size: 14px;
            color: #444;
            line-height: 1.5;
        }
    </style>
</head>
<body>

    
    <button class="open-btn" onclick="openModal()">Open Modal</button>

   
    <div class="modal-overlay" id="modalOverlay">
        <div class="modal">
            <div class="modal-header">
                <h2>Modal Title</h2>
                <button class="close-btn" onclick="closeModal()">×</button>
            </div>

            <div class="modal-content">
                <p>
                    This is a simple modal popup. You can use it to show
                    messages, forms, alerts, or any important information
                    without leaving the page.
                </p>
            </div>
        </div>
    </div>


</body>
</html>

