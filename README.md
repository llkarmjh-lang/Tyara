<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>موقع طيارة</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Jawel&display=swap');

  body {
    margin: 0;
    font-family: 'Jawel', sans-serif;
    background: linear-gradient(135deg, #0b1b4d, #1a2b70, #001f4d);
    color: #d4af37; /* ذهبي فاخر للخطوط */
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }

  /* صفحة الدخول */
  #loginPage {
    display: flex;
    flex-direction: column;
    align-items: center;
    background: rgba(0,0,0,0.75);
    padding: 40px;
    border-radius: 20px;
    box-shadow: 0 0 30px rgba(0,0,0,0.8);
    text-align: center;
  }

  #loginPage h1 {
    margin-bottom: 25px;
    font-size: 2em;
    color: #d4af37; /* ذهبي */
    text-align: center;
  }

  #loginPage input {
    margin: 12px 0;
    padding: 14px;
    width: 270px;
    border: none;
    border-radius: 14px;
    font-size: 1em;
    text-align: center;
  }

  #loginPage button {
    padding: 14px 30px;
    margin-top: 15px;
    background: linear-gradient(45deg, #1a2b70, #0b1b4d);
    color: #d4af37;
    font-weight: bold;
    border: none;
    border-radius: 14px;
    cursor: pointer;
    transition: 0.3s;
  }

  #loginPage button:hover {
    background: linear-gradient(45deg, #0b1b4d, #1a2b70);
  }

  #contact {
    margin-top: 20px;
    font-size: 1.2em;
    color: #d4af37;
  }

  .social-icons {
    margin-top: 15px;
    display: flex;
    gap: 15px;
  }

  .social-icons a img {
    width: 35px; /* حجم أصغر */
    transition: transform 0.3s;
  }

  .social-icons a img:hover {
    transform: scale(1.1); /* تأثير خفيف عند المرور */
  }

</style>
</head>
<body>

<!-- صفحة الدخول -->
<div id="loginPage">
  <h1>موقع طيارة السارقو لتحسين جودة الصور</h1>
  <input type="text" id="username" placeholder="اسم المستخدم">
  <input type="password" id="password" placeholder="كلمة المرور">
  <button onclick="checkLogin()">دخول</button>

  <div id="contact">رقم التواصل: +249118519669</div>
  <div class="social-icons">
    <a href="https://www.instagram.com/ins.tyara?igsh=MWxienRpc29lN3RqZg==" target="_blank"><img src="https://cdn-icons-png.flaticon.com/512/2111/2111463.png" alt="Instagram"></a>
    <a href="https://wa.me/249118519669" target="_blank"><img src="https://cdn-icons-png.flaticon.com/512/733/733585.png" alt="WhatsApp"></a>
  </div>
</div>

<script>
function checkLogin() {
  const password = document.getElementById('password').value;
  if(password === "طيارة عمي") {
    // التحويل مباشرة بعد الدخول
    window.location.href = "https://jpghd.com/";
  } else {
    // رسالة رفض باللون الكحلي
    alert("%cكلمة المرور خاطئة!", "color:#0b1b4d; font-weight:bold;");
  }
}
</script>

</body>
</html>
