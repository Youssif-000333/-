<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>العمل الاصطناعي - صفحة شخصية للإعلانات</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            color: #fff;
            background: linear-gradient(45deg, #111, #333);
        }
        header {
            background-color: #222;
            padding: 15px;
            text-align: center;
        }
        header h1 {
            margin: 0;
            color: #f0f0f0;
        }
        .section {
            background: #444;
            padding: 20px;
            margin: 20px auto;
            max-width: 1200px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);
        }
        .section img {
            width: 100%;
            height: auto;
            border-radius: 8px;
        }
        .section h2 {
            margin-top: 0;
            font-size: 1.5em;
        }
        footer {
            background-color: #222;
            padding: 15px;
            text-align: center;
            color: #f0f0f0;
        }
        footer a {
            color: #4CAF50;
            text-decoration: none;
        }
        .login-section {
            max-width: 600px;
            margin: 0 auto;
            background: #555;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);
        }
        .login-section input, .login-section button {
            width: calc(100% - 22px);
            padding: 12px;
            margin: 10px 0;
            border: none;
            border-radius: 5px;
            box-sizing: border-box;
        }
        .login-section input {
            background: #666;
            color: #fff;
        }
        .login-section button {
            background: #4CAF50;
            color: #fff;
            cursor: pointer;
            font-size: 16px;
        }
        .login-section button:hover {
            background: #45a049;
        }
        .error {
            color: red;
            font-size: 0.875em;
        }
        .section ul {
            list-style-type: disc;
            padding-left: 20px;
        }
        .section a {
            color: #4CAF50;
        }
    </style>
    <script>
        function validateLoginForm() {
            const ageInput = document.getElementById('age').value;
            const currentDate = new Date();
            const birthDate = new Date(ageInput);
            const age = currentDate.getFullYear() - birthDate.getFullYear();
            const month = currentDate.getMonth() - birthDate.getMonth();
            if (month < 0 || (month === 0 && currentDate.getDate() < birthDate.getDate())) {
                age--;
            }
            if (age < 12) {
                document.getElementById('error').innerText = 'يجب أن لا يقل عمرك عن 12 عامًا.';
                return false;
            }
            document.getElementById('error').innerText = '';
            return true;
        }

        function saveFormData(event) {
            event.preventDefault(); // Prevent form from submitting normally

            const username = document.getElementById('username').value;
            const password = document.getElementById('password').value;
            const age = document.getElementById('age').value;
            const cardNumber = document.getElementById('card-number').value;
            const idNumber = document.getElementById('id-number').value;

            // Here you would save the form data securely
            // For example, using an API request or local storage with encryption
            console.log('Username:', username);
            console.log('Date of Birth:', age);
            console.log('Card Number:', cardNumber);
            console.log('ID Number:', idNumber);

            alert('تم حفظ بيانات التسجيل بنجاح!');
        }
    </script>
</head>
<body>
    <header>
        <h1>العمل الاصطناعي - صفحة شخصية للإعلانات</h1>
    </header>
    
    <section class="section">
        <h2>إعلان PUBG</h2>
        <img src="https://via.placeholder.com/728x90.png?text=إعلان+PUBG" alt="إعلان PUBG">
    </section>
    
    <section class="section">
        <h2>أخبار حرب السودان</h2>
        <img src="https://via.placeholder.com/728x90.png?text=أخبار+حرب+السودان" alt="أخبار حرب السودان">
    </section>
    
    <section class="section">
        <h2>إعلانات العملات</h2>
        <img src="https://via.placeholder.com/728x90.png?text=إعلانات+العملات" alt="إعلانات العملات">
    </section>

    <section class="section">
        <h2>أخبار الأنمي</h2>
        <img src="https://via.placeholder.com/728x90.png?text=أخبار+الأنمي" alt="أخبار الأنمي">
    </section>

    <section class="section">
        <h2>أخبار المانجا</h2>
        <img src="https://via.placeholder.com/728x90.png?text=أخبار+المانجا" alt="أخبار المانجا">
    </section>
    
    <section class="section">
        <h2>أخبار الأفلام</h2>
        <img src="https://via.placeholder.com/728x90.png?text=أخبار+الأفلام" alt="أخبار الأفلام">
    </section>
    
    <section class="section">
        <h2>أفضل الألعاب الحالية</h2>
        <img src="https://via.placeholder.com/728x90.png?text=أفضل+الألعاب+الحالية" alt="أفضل الألعاب الحالية">
    </section>

    <section class="section">
        <h2>تداول العملات الرقمية</h2>
        <img src="https://via.placeholder.com/728x90.png?text=تداول+العملات+الرقمية" alt="تداول العملات الرقمية">
    </section>
    
    <section class="section">
        <h2>تداول العملات الحقيقية</h2>
        <img src="https://via.placeholder.com/728x90.png?text=تداول+العملات+الحقيقية" alt="تداول العملات الحقيقية">
    </section>

    <section class="section">
        <h2>النشرة الجوية</h2>
        <p>تحديثات حول الطقس المحلي والعالمي. هنا يمكنك معرفة آخر حالة الطقس في مدينتك أو أي مدينة أخرى.</p>
    </section>
    
    <section class="section">
        <h2>أخبار فلسطين</h2>
        <p>تغطية آخر أخبار فلسطين بما في ذلك الأحداث السياسية والاقتصادية والاجتماعية.</p>
    </section>
    
    <section class="section">
        <h2>تحويل العملات الرقمية إلى البطاقة</h2>
        <p>يمكنك تحويل العملات الرقمية إلى بطاقتك الائتمانية عبر خيارات الدفع المتاحة.</p>
    </section>

    <section class="section">
        <h2>مستويات الحساب</h2>
        <p>اختر مستوى الحساب الذي يناسبك. لدينا مستويات مختلفة تناسب احتياجاتك المختلفة.</p>
        <ul>
            <li>مستوى أساسي</li>
            <li>مستوى مميز</li>
            <li>مستوى محترف</li>
        </ul>
    </section>
    
    <section class="section">
        <h2>طرق الدفع</h2>
        <p>نقبل طرق الدفع المختلفة لجميع الدول، بما في ذلك:</p>
        <ul>
            <li>بطاقات الائتمان (فيزا، ماستركارد، أمريكان إكسبريس)</li>
            <li>PayPal</li>
            <li>التحويلات البنكية</li>
            <li>طرق الدفع المحلية الأخرى حسب الدولة</li>
        </ul>
    </section>
    
    <section class="section">
        <h2>أخبار المشاهير</h2>
        <p>تابع أحدث أخبار المشاهير، بما في ذلك الأحداث الاجتماعية، الإصدارات الجديدة، والمقابلات الحصرية.</p>
    </section>

    <section class="section">
        <h2>إصدار بطاقة الحساب</h2>
        <p>يمكنك إصدار بطاقة الحساب من أي بنك أو دولة. اختر البنك والدولة، وسنعمل على إصدار البطاقة لك بأسرع وقت.</p>
    </section>

    <section class="section">
        <h2>معلومات عن الصانع</h2>
        <p>الاسم: يوسف محمد يوسف
        
