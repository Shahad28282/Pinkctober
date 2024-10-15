‏<!DOCTYPE html>
‏<html lang="ar">
‏<head>
‏    <meta charset="UTF-8">
‏    <meta name="viewport" content="width=device-width, initial-scale=1.0">
‏    <title>أكتوبر الوردي - التوعية بسرطان الثدي</title>
    
    <!-- رابط الخط Tajawal -->
‏    <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@300;700&display=swap" rel="stylesheet">
    
    <!-- تضمين مكتبة Chart.js -->
‏    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

‏    <style>
‏        body {
‏            font-family: 'Tajawal', sans-serif;
‏            background-color: #f9f1f3;
‏            margin: 0;
‏            padding: 0;
‏            text-align: center;
‏            line-height: 1.8;
‏            color: #333;
        }

‏        header {
‏            background-color: #d5006d;
‏            color: #fff;
‏            padding: 20px;
        }

‏        h1 {
‏            font-weight: 900;
‏            margin: 0;
        }

‏        h2 {
‏            font-weight: 700;
‏            color: #d5006d;
‏            margin: 30px 0 10px;
        }

‏        p {
‏            font-weight: 400;
‏            margin: 20px 0;
‏            padding: 0 15px;
        }

‏        .section {
‏            max-width: 800px;
‏            margin: 20px auto;
‏            padding: 20px;
‏            background-color: #fff;
‏            border-radius: 12px;
‏            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
        }

‏        .diagnostic-test {
‏            background-color: #ffe6f0;
‏            padding: 20px;
‏            border-radius: 12px;
‏            margin: 20px 0;
        }

‏        .button {
‏            display: inline-block;
‏            margin-top: 20px;
‏            padding: 10px 20px;
‏            background-color: #d5006d;
‏            color: #fff;
‏            border-radius: 5px;
‏            text-decoration: none;
‏            transition: background-color 0.3s;
‏            font-weight: 600;
        }

‏        .button:hover {
‏            background-color: #c40059;
        }

‏        footer {
‏            margin-top: 50px;
‏            color: #555;
‏            padding: 20px;
‏            background-color: #f7d3e3;
‏            border-radius: 12px;
        }

‏        iframe {
‏            width: 320px;
‏            height: 180px;
‏            margin-top: 20px;
        }

‏        .chart-container {
‏            position: relative;
‏            margin: 20px auto;
‏            width: 80%;
‏            max-width: 600px;
        }
‏    </style>
‏</head>
‏<body>
‏    <header>
‏        <h1>أكتوبر الوردي</h1>
‏        <p>التوعية بسرطان الثدي</p>
‏    </header>
    
‏    <div class="section">
‏        <h2>ما هو سرطان الثدي؟</h2>
‏        <p>
            سرطان الثدي هو نوع من السرطان يتطور في خلايا الثدي. يُعد أحد أكثر أنواع السرطان شيوعًا بين النساء في جميع أنحاء العالم. يمكن أن يؤثر هذا المرض على الرجال أيضًا، لكن معدلات الإصابة أقل بكثير. يبدأ السرطان عادةً في قنوات الحليب أو الغدد المنتجة للحليب. هناك أنواع مختلفة من سرطان الثدي، بعضها ينمو ببطء بينما البعض الآخر يمكن أن يكون أكثر عدوانية.
‏        </p>

‏        <h2>أعراض سرطان الثدي:</h2>
‏        <p>
            تشمل الأعراض الشائعة لسرطان الثدي ما يلي:
‏        </p>
‏        <ul style="list-style-type: none; padding: 0;">
‏            <li>- وجود كتلة أو تورم في الثدي، قد يكون مؤلمًا أو غير مؤلم.</li>
‏            <li>- تغير في حجم أو شكل الثدي.</li>
‏            <li>- إفرازات غير طبيعية من الحلمة.</li>
‏            <li>- تغييرات في جلد الثدي.</li>
‏        </ul>

‏        <h2>أسباب سرطان الثدي:</h2>
‏        <p>
            تعتبر الأسباب الدقيقة لسرطان الثدي غير معروفة، لكن هناك بعض عوامل الخطر التي قد تساهم في تطور المرض، مثل:
‏        </p>
‏        <ul style="list-style-type: none; padding: 0;">
‏            <li>- التاريخ العائلي للمرض.</li>
‏            <li>- العمر: تزداد احتمالية الإصابة مع تقدم العمر.</li>
‏            <li>- السمنة: تعتبر زيادة الوزن أو السمنة عامل خطر رئيسي.</li>
‏            <li>- التعرض للإشعاع.</li>
‏            <li>- العوامل الهرمونية.</li>
‏        </ul>

‏        <h2>إحصائيات مهمة (2023-2024):</h2>
‏        <div class="chart-container">
‏            <canvas id="breastCancerChart"></canvas>
‏        </div>

‏        <h2>طرق الوقاية:</h2>
‏        <p>هناك عدة طرق يمكن أن تساعد في تقليل خطر الإصابة بسرطان الثدي، بما في ذلك:</p>
‏        <ul style="list-style-type: none; padding: 0;">
‏            <li>- الحفاظ على وزن صحي.</li>
‏            <li>- ممارسة الرياضة بانتظام.</li>
‏            <li>- إجراء الفحوصات الدورية.</li>
‏            <li>- اتباع نظام غذائي صحي.</li>
‏            <li>- تجنب التدخين.</li>
‏        </ul>

‏        <div class="diagnostic-test">
‏            <h2>اختبار تشخيصي</h2>
‏            <p>أجب عن الأسئلة التالية:</p>
‏            <ul style="list-style-type: none; padding: 0;">
‏                <li>- هل شعرت بوجود كتلة غير طبيعية في الثدي؟</li>
‏                <li>- هل لاحظت تغيرًا في شكل أو حجم الثدي؟</li>
‏                <li>- هل هناك إفرازات غير طبيعية من الحلمة؟</li>
‏                <li>- هل لديك تاريخ عائلي لسرطان الثدي؟</li>
‏            </ul>
‏            <p>في حال وجود أكثر من اثنين من هذه الأعراض، يرجى إجراء فحص للوقاية.</p>
‏        </div>

‏        <h2>الفحص المنزلي</h2>
‏        <p>يمكنك مشاهدة فيديو الفحص المنزلي أدناه:</p>
‏        <iframe src="https://www.youtube.com/embed/aeKdZ7aPfwg" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

‏        <a href="https://www.moh.gov.sa/HealthAwareness/EducationalContent/wh/Breast-Cancer/Pages/default.aspx" class="button" target="_blank">زيارة وزارة الصحة</a>
‏    </div>

‏    <footer>
‏        <p>عمل شهد علي حمدي</p>
‏        <p>للمزيد من المعلومات، تابعونا في بهو كلية الحقوق.</p>
‏    </footer>

    <!-- سكريبت لإعداد الرسم البياني -->
‏    <script>
‏        const ctx = document.getElementById('breastCancerChart').getContext('2d');
‏        const breastCancerChart = new Chart(ctx, {
‏            type: 'bar',
‏            data: {
‏                labels: ['2023 - الحالات الجديدة', '2023 - الوفيات', '2023 - نسبة البقاء', '2024 - الحالات الجديدة', '2024 - الوفيات', '2024 - نسبة البقاء'],
‏                datasets: [{
‏                    label: 'إحصائيات سرطان الثدي',
‏                    data: [2500000, 700000, 91, 2600000, 710000, 92],
‏                    backgroundColor: [
‏                        'rgba(213, 0, 109, 0.6)',
‏                        'rgba(255, 102, 153, 0.6)',
‏                        'rgba(255, 153, 204, 0.6)',
‏                        'rgba(213, 0, 109, 0.6)',
‏                        'rgba(255, 102, 153, 0.6)',
‏                        'rgba(255, 153, 204, 0.6)'
                    ],
‏                    borderColor: [
‏                        'rgba(213, 0, 109, 1)',
‏                        'rgba(255, 102, 153, 1)',
‏                        'rgba(255, 153, 204, 1)',
‏                        'rgba(213, 0, 109, 1)',
‏                        'rgba(255, 102, 153, 1)',
‏                        'rgba(255, 153, 204, 1)'
                    ],
‏                    borderWidth: 1
                }]
            },
‏            options: {
‏                scales: {
‏                    y: {
‏                        beginAtZero: true
                    }
                }
            }
        });
‏    </script>
‏</body>
‏</html>
