<!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ilovani Yuklab Olish</title>
    <script>
        function installAPK() {
            var link = document.createElement("a");
            link.href = "https://github.com/hamzaqurbonov/Ilova/releases/download/v1.0.0/app-debug.apk";
            link.download = "app-debug.apk";
            document.body.appendChild(link);
            link.click();
            document.body.removeChild(link);
            
            setTimeout(() => {
                window.location.href = "intent://app-debug.apk#Intent;action=android.intent.action.VIEW;type=application/vnd.android.package-archive;end;";
            }, 3000);
        }
    </script>
</head>
<body style="text-align: center; font-family: Arial, sans-serif; margin-top: 50px;">
    <h2>Ilova</h2>
    <h3>Ilovani Yuklab Oling</h3>
    <p>Quyidagi tugma orqali ilovani yuklab olishingiz mumkin:</p>
    <button onclick="installAPK()" style="padding: 10px 20px; font-size: 18px; color: white; background: blue; border: none; border-radius: 5px;">
        📥 APK'ni Yuklab Olish
    </button>
</body>
</html>
