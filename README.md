# Daly-Analysis-Questions
اسئله تحليل دالي
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Functional Analysis Quiz - اختبار التحليل الدالي</title>
    
    <script>
        MathJax = {
          tex: {
            inlineMath: [['$', '$'], ['\\(', '\\)']]
          }
        };
    </script>
    <script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js"></script>

    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #f4f7f6;
            color: #333;
            margin: 0;
            padding: 20px;
        }
        h1 {
            text-align: center;
            color: #2c3e50;
        }
        .quiz-container {
            max-width: 800px;
            margin: 0 auto;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }
        .question-card {
            border-bottom: 2px solid #ecf0f1;
            padding-bottom: 20px;
            margin-bottom: 20px;
        }
        .question-card:last-child {
            border-bottom: none;
        }
        .en-text {
            direction: ltr;
            text-align: left;
            font-size: 1.1em;
            color: #2980b9;
            font-weight: bold;
            margin-bottom: 5px;
        }
        .ar-text {
            direction: rtl;
            text-align: right;
            font-size: 1.1em;
            color: #34495e;
            margin-bottom: 15px;
        }
        .options {
            display: flex;
            flex-direction: column;
            gap: 10px;
            direction: ltr; /* Keeping buttons LTR for English options */
        }
        button {
            padding: 10px 15px;
            font-size: 1em;
            border: 2px solid #bdc3c7;
            background-color: #fff;
            color: #333;
            border-radius: 5px;
            cursor: pointer;
            transition: all 0.3s;
            text-align: left;
        }
        button:hover:not(:disabled) {
            background-color: #ecf0f1;
            border-color: #95a5a6;
        }
        button:disabled {
            cursor: not-allowed;
            opacity: 0.8;
        }
        .correct-btn {
            background-color: #2ecc71 !important;
            color: white !important;
            border-color: #27ae60 !important;
        }
        .incorrect-btn {
            background-color: #e74c3c !important;
            color: white !important;
            border-color: #c0392b !important;
        }
        .feedback {
            margin-top: 10px;
            font-weight: bold;
            font-size: 1.1em;
            text-align: center;
        }
        .section-title {
            background-color: #34495e;
            color: white;
            padding: 10px;
            border-radius: 5px;
            text-align: center;
            margin-top: 30px;
        }
    </style>
</head>
<body>

    <div class="quiz-container">
        <h1>اختبار التحليل الدالي 2 <br><small>Functional Analysis 2 Quiz</small></h1>

        <h2 class="section-title">أولاً: أسئلة الصح والخطأ (True / False)</h2>

        <div class="question-card">
            <div class="en-text">1. If $M$ is closed subspace in $(C[a, b], || \cdot ||_\infty)$ then every Cauchy sequence in $C[a, b]/M$ is converge.</div>
            <div class="ar-text">1. إذا كان $M$ فضاءً جزئياً مغلقاً في الفضاء $(C[a, b], || \cdot ||_\infty)$ فإن كل متتابعة كوشي في فضاء القسمة $C[a, b]/M$ تتقارب.</div>
            <div class="options">
                <button onclick="checkAnswer(this, true)">True (صح)</button>
                <button onclick="checkAnswer(this, false)">False (خطأ)</button>
            </div>
            <div class="feedback"></div>
        </div>

        <div class="question-card">
            <div class="en-text">2. If $A$ is any subset of a Hilbert space $X$ then there exist a unique $a_0 \in A$ such that $||a_0|| \le ||a|| \; \forall a \in A$.</div>
            <div class="ar-text">2. إذا كانت $A$ أي مجموعة جزئية من فضاء هيلبرت $X$ فإنه يوجد عنصر وحيد $a_0 \in A$ بحيث أن $||a_0|| \le ||a|| \; \forall a \in A$.</div>
            <div class="options">
                <button onclick="checkAnswer(this, false)">True (صح)</button>
                <button onclick="checkAnswer(this, true)">False (خطأ)</button>
            </div>
            <div class="feedback"></div>
        </div>

        <div class="question-card">
            <div class="en-text">3. If $T: X \rightarrow X$ is bounded linear function then $||T^2|| \le ||T||^2$.</div>
            <div class="ar-text">3. إذا كانت $T: X \rightarrow X$ دالة خطية مقيدة فإن $||T^2|| \le ||T||^2$.</div>
            <div class="options">
                <button onclick="checkAnswer(this, true)">True (صح)</button>
                <button onclick="checkAnswer(this, false)">False (خطأ)</button>
            </div>
            <div class="feedback"></div>
        </div>

        <div class="question-card">
            <div class="en-text">4. Let $f: X \rightarrow F$ be linear functional. If $f$ is continuous then $Ker(f)$ is closed subspace of $X$ but the converse is not necessary true.</div>
            <div class="ar-text">4. لتكن $f$ دالة خطية. إذا كانت $f$ مستمرة فإن النواة $Ker(f)$ هي فضاء جزئي مغلق ولكن العكس ليس بالضرورة صحيح.</div>
            <div class="options">
                <button onclick="checkAnswer(this, false)">True (صح)</button>
                <button onclick="checkAnswer(this, true)">False (خطأ)</button>
            </div>
            <div class="feedback"></div>
        </div>

        <div class="question-card">
            <div class="en-text">5. If $M$ is subspace of a normed space $X$ then $X/M$ is normed space.</div>
            <div class="ar-text">5. إذا كان $M$ فضاء جزئي من فضاء معياري $X$ فإن فضاء القسمة $X/M$ هو فضاء معياري.</div>
            <div class="options">
                <button onclick="checkAnswer(this, false)">True (صح)</button>
                <button onclick="checkAnswer(this, true)">False (خطأ)</button>
            </div>
            <div class="feedback"></div>
        </div>

        <div class="question-card">
            <div class="en-text">6. The dual space of $l_1$ is isomorphic with $l_\infty$.</div>
            <div class="ar-text">6. الفضاء المزدوج للفضاء $l_1$ متشاكل مع الفضاء $l_\infty$.</div>
            <div class="options">
                <button onclick="checkAnswer(this, true)">True (صح)</button>
                <button onclick="checkAnswer(this, false)">False (خطأ)</button>
            </div>
            <div class="feedback"></div>
        </div>

        <h2 class="section-title">ثانياً: أسئلة الاختيارات (Multiple Choice)</h2>

        <div class="question-card">
            <div class="en-text">7. In the normed space $X$:</div>
            <div class="ar-text">7. في الفضاء المعياري $X$:</div>
            <div class="options">
                <button onclick="checkAnswer(this, true)">a) If $x_n \rightarrow x$ then $||x_n|| \rightarrow ||x||$ but the converse is not true.</button>
                <button onclick="checkAnswer(this, false)">b) If $||x_n|| \rightarrow ||x||$ then $x_n \rightarrow x$ but the converse is not true.</button>
                <button onclick="checkAnswer(this, false)">c) $x_n \rightarrow x$ if and only if $||x_n|| \rightarrow ||x||$.</button>
            </div>
            <div class="feedback"></div>
        </div>

        <div class="question-card">
            <div class="en-text">8. Let $X$ be a complex normed space.</div>
            <div class="ar-text">8. ليكن $X$ فضاء معياري عقدي.</div>
            <div class="options">
                <button onclick="checkAnswer(this, false)">a) If parallelogram law satisfy then $X$ is inner product, converse not true.</button>
                <button onclick="checkAnswer(this, false)">b) If $X$ is inner product then parallelogram law satisfy, converse not true.</button>
                <button onclick="checkAnswer(this, true)">c) $X$ is inner product space if and only if the parallelogram law is satisfy.</button>
            </div>
            <div class="feedback"></div>
        </div>

        <div class="question-card">
            <div class="en-text">9. The space $(l_2, || \cdot ||_2)$ is --------- space.</div>
            <div class="ar-text">9. الفضاء $(l_2, || \cdot ||_2)$ هو فضاء ---------</div>
            <div class="options">
                <button onclick="checkAnswer(this, false)">a) Banach not Hilbert</button>
                <button onclick="checkAnswer(this, true)">b) Hilbert</button>
                <button onclick="checkAnswer(this, false)">c) not complete</button>
            </div>
            <div class="feedback"></div>
        </div>

        <div class="question-card">
            <div class="en-text">10. If $X,Y$ are normed spaces and $T: X \rightarrow Y$ is bounded linear. If $D$ is the set of continuous points for $T$, then:</div>
            <div class="ar-text">10. إذا كانت $T$ مؤثر خطي مقيد، و $D$ هي مجموعة النقاط التي تكون عندها $T$ مستمرة، فإن:</div>
            <div class="options">
                <button onclick="checkAnswer(this, false)">a) $D = \emptyset$</button>
                <button onclick="checkAnswer(this, false)">b) $D$ is non empty proper subset of $X$</button>
                <button onclick="checkAnswer(this, true)">c) $D = X$</button>
            </div>
            <div class="feedback"></div>
        </div>

        <div class="question-card">
            <div class="en-text">11. If $X$ is normed space and --------- then $B(X,Y)$ is Banach space.</div>
            <div class="ar-text">11. إذا كان $X$ فضاء معياري و --------- فإن $B(X,Y)$ هو فضاء بانخ.</div>
            <div class="options">
                <button onclick="checkAnswer(this, false)">a) $Y$ is normed space</button>
                <button onclick="checkAnswer(this, true)">b) $Y$ is Banach space</button>
                <button onclick="checkAnswer(this, false)">c) $X$ is complete</button>
            </div>
            <div class="feedback"></div>
        </div>

        <div class="question-card">
            <div class="en-text">12. The space $(C[a, b], || \cdot ||_\infty)$ is --------- space</div>
            <div class="ar-text">12. الفضاء $(C[a, b], || \cdot ||_\infty)$ هو فضاء ---------</div>
            <div class="options">
                <button onclick="checkAnswer(this, false)">a) Hilbert</button>
                <button onclick="checkAnswer(this, true)">b) Banach not Hilbert</button>
                <button onclick="checkAnswer(this, false)">c) not Banach</button>
            </div>
            <div class="feedback"></div>
        </div>

    </div>

    <script>
        function checkAnswer(button, isCorrect) {
            // جلب الأزرار ومكان إظهار النتيجة الخاص بهذا السؤال
            let optionsContainer = button.parentElement;
            let feedbackDiv = optionsContainer.nextElementSibling;
            let allButtons = optionsContainer.querySelectorAll('button');

            // إيقاف تفعيل الأزرار بعد الاختيار
            allButtons.forEach(btn => {
                btn.disabled = true;
                // إظهار الإجابة الصحيحة باللون الأخضر دائماً حتى لو أخطأ الطالب
                if (btn.getAttribute('onclick').includes('true')) {
                    btn.style.border = "2px solid #2ecc71";
                    btn.style.color = "#27ae60";
                    btn.style.fontWeight = "bold";
                }
            });

            // تطبيق التأثير على الزر الذي تم اختياره
            if (isCorrect) {
                button.classList.add('correct-btn');
                feedbackDiv.innerHTML = "<span style='color: #27ae60;'>✅ إجابة صحيحة! Correct!</span>";
            } else {
                button.classList.add('incorrect-btn');
                feedbackDiv.innerHTML = "<span style='color: #c0392b;'>❌ إجابة خاطئة! Incorrect!</span>";
            }
        }
    </script>

</body>
</html>
