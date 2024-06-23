<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>منصة بليكسو</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f5f5f5;
            color: #333;
            margin: 0;
            padding: 0;
            line-height: 1.6;
        }
        header {
            background-color: #0073e6;
            color: white;
            padding: 10px 0;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #333;
        }
        nav a {
            color: white;
            padding: 14px 20px;
            text-decoration: none;
            text-align: center;
        }
        nav a:hover {
            background-color: #575757;
        }
        .container {
            width: 80%;
            margin: 20px auto;
        }
        .section {
            background-color: white;
            padding: 20px;
            margin-bottom: 20px;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .section h2 {
            margin-top: 0;
        }
        .dark-mode {
            background-color: #333;
            color: white;
        }
    </style>
</head>
<body>
    <header>
        <h1>منصة بليكسو</h1>
        <p>منصة تدعم الذكاء الاصطناعي لتحليل الشموع</p>
    </header>
    <nav>
        <a href="#login">تسجيل الدخول</a>
        <a href="#posts">المنشورات</a>
        <a href="#profile">الملف الشخصي</a>
    </nav>
    <div class="container">
        <section id="login" class="section">
            <h2>تسجيل الدخول</h2>
            <form>
                <label for="email">الإيميل أو رقم التلفون:</label><br>
                <input type="text" id="email" name="email"><br><br>
                <label for="password">كلمة المرور:</label><br>
                <input type="password" id="password" name="password"><br><br>
                <input type="submit" value="تسجيل الدخول">
            </form>
        </section>
        <section id="posts" class="section">
            <h2>المنشورات</h2>
            <p>يمكنك مشاهدة منشورات المستخدمين، التعليق عليها، مشاركتها، وحفظها.</p>
            <!-- منشورات نموذجية -->
            <div class="post">
                <h3>منشور 1</h3>
                <p>هذا نص منشور نموذج.</p>
                <button>تعليق</button>
                <button>مشاركة</button>
                <button>حفظ</button>
            </div>
            <div class="post">
                <h3>منشور 2</h3>
                <p>هذا نص منشور نموذج آخر.</p>
                <button>تعليق</button>
                <button>مشاركة</button>
                <button>حفظ</button>
            </div>
        </section>
        <section id="profile" class="section">
            <h2>الملف الشخصي</h2>
            <p>يمكنك رؤية معلومات ملفك الشخصي، الإعدادات، ورابط الدعوة.</p>
            <ul>
                <li>اسم المستخدم: Blixou</li>
                <li>كلمة المرور: ******</li>
                <li><img src="profile.jpg" alt="الصورة الشخصية" width="100"></li>
                <li>رابط الدعوة: <a href="#">دعوة الأصدقاء</a></li>
                <li>عدد الأشخاص المدعوين: 10</li>
            </ul>
            <button onclick="toggleDarkMode()">تبديل الوضع الداكن/الأبيض</button>
            <button>تسجيل الخروج</button>
            <button>إضافة حساب آخر</button>
        </section>
    </div>

    <script>
        function toggleDarkMode() {
            document.body.classList.toggle('dark-mode');
        }
    </script>
</body>
</html>
