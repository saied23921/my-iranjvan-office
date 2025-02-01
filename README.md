<!DOCTYPE html>
<html lang="fa">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>سیستم مدیریت حمل و نقل</title>
    <script>
        function searchCustomer() {
            let input = document.getElementById("searchInput").value.toLowerCase();
            let customers = document.getElementsByClassName("customer");
            
            for (let i = 0; i < customers.length; i++) {
                let name = customers[i].innerText.toLowerCase();
                if (name.includes(input)) {
                    customers[i].style.display = "block";
                } else {
                    customers[i].style.display = "none";
                }
            }
        }
    </script>
</head>
<body>
    <h1>جستجوی مشتریان</h1>
    <input type="text" id="searchInput" onkeyup="searchCustomer()" placeholder="نام مشتری را وارد کنید">
    
    <ul>
        <li class="customer">علی رضایی - 09121234567 - کامیون</li>
        <li class="customer">محمود احمدی - 09351234567 - تریلی</li>
        <li class="customer">سعید کریمی - 09981234567 - وانت</li>
    </ul>
</body>
</html><!DOCTYPE html>
<html lang="fa">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ورود به سیستم</title>
    <script>
        function login() {
            let username = document.getElementById("username").value;
            let password = document.getElementById("password").value;

            if (username === "admin" && password === "6569") {
                window.location.href = "dashboard.html"; // صفحه مدیریت
            } else {
                alert("نام کاربری یا رمز عبور اشتباه است!");
            }
        }
    </script>
</head>
<body>
    <h1>ورود به سیستم مدیریت حمل و نقل</h1>
    <input type="text" id="username" placeholder="نام کاربری"><br><br>
    <input type="password" id="password" placeholder="رمز عبور"><br><br>
    <button onclick="login()">ورود</button>
</body>
</html><!DOCTYPE html>
<html lang="fa">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>تماس با ما</title>
</head>
<body>
    <h1>تماس با شرکت حمل و نقل</h1>
    <p>آدرس: کرمان، خیابان ولیعصر، پلاک ۳۴</p>
    <p>تلفن: 034-12345678</p>
    <p>ایمیل: info@iranjvan.com</p>

    <h2>ارسال پیام</h2>
    <form>
        <input type="text" placeholder="نام شما">
        <input type="email" placeholder="ایمیل شما">
        <textarea placeholder="پیام خود را بنویسید"></textarea>
        <button type="submit">ارسال</button>
    </form>
</body>
</html><nav>
    <a href="dashboard.html">🏠 داشبورد</a> |
    <a href="contact.html">📞 تماس با ما</a> |
    <a href="index.html">🚪 خروج</a>
</nav><nav>
    <a href="dashboard.html">🏠 بازگشت به داشبورد</a>
</nav><!DOCTYPE html>
<html lang="fa">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ورود به سیستم</title>
    <script>
        function login() {
            let username = document.getElementById("username").value;
            let password = document.getElementById("password").value;

            if (username === "admin" && password === "6569") {
                window.location.href = "dashboard.html"; 
            } else {
                alert("نام کاربری یا رمز عبور اشتباه است!");
            }
        }
    </script>
</head>
<body>
    <h1>ورود به سیستم مدیریت حمل و نقل</h1>
    <input type="text" id="username" placeholder="نام کاربری"><br><br>
    <input type="password" id="password" placeholder="رمز عبور"><br><br>
    <button onclick="login()">ورود</button>
</body>
</html><!DOCTYPE html>
<html lang="fa">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>پنل مدیریت</title>
    <script>
        function searchCustomer() {
            let input = document.getElementById("searchInput").value.toLowerCase();
            let customers = document.getElementsByClassName("customer");
