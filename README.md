# Shark-story
<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>قصة القرش القوي</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>قصة القرش القوي</h1>
        <nav>
            <ul>
                <li><a href="#home">الرئيسية</a></li>
                <li><a href="#story">القصة</a></li>
                <li><a href="#puzzles">الألغاز</a></li>
                <li><a href="#contact">اتصل بنا</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section id="home">
            <h2>مرحبًا بكم في موقع قصة القرش القوي</h2>
            <p>اكتشفوا قصة القرش القوي وأصدقائه، واحلوا الألغاز المثيرة.</p>
        </section>
        <section id="story">
            <h2>القصة</h2>
            <p>كان هناك قرش قوي يعيش في أعماق البحر. كان لديه صديقان مقربان: ماريو، السمكة الصغيرة، وإلي، الأخطبوط. كان للقرش أيضًا علاقة خاصة مع الوشا، السلحفاة الذكية، ولكنه كان يحاول استعادة تلك العلاقة بعدما انفصلت عنه.</p>
            <p>واجه القرش وأصدقاؤه العديد من التحديات والمغامرات في البحر، وكان عليهم حل العديد من الألغاز للتقدم في مغامرتهم.</p>
        </section>
        <section id="puzzles">
            <h2>الألغاز</h2>
            <div id="puzzle-list">
                <!-- سيتم إضافة الألغاز هنا بواسطة JavaScript -->
            </div>
        </section>
        <section id="contact">
            <h2>اتصل بنا</h2>
            <form>
                <label for="name">الاسم:</label>
                <input type="text" id="name" name="name">
                <label for="email">البريد الإلكتروني:</label>
                <input type="email" id="email" name="email">
                <label for="message">رسالة:</label>
                <textarea id="message" name="message"></textarea>
                <button type="submit">إرسال</button>
            </form>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 قصة القرش القوي. جميع الحقوق محفوظة.</p>
    </footer>
    <script src="script.js"></script>
</body>
</html>body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 0;
}

header {
    background: #333;
    color: #fff;
    padding: 1em 0;
    text-align: center;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 1em;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
}

main {
    padding: 2em;
}

section {
    margin-bottom: 2em;
}

footer {
    text-align: center;
    padding: 1em 0;
    background: #333;
    color: #fff;
}const puzzles = [
    "ما هو الشيء الذي يقرصك دون أن تراه؟",
    "ما هو الشيء الذي يمشي بلا رجلين ويبكي بلا عينين؟",
    // ... أضف باقي الألغاز هنا
    "ما هو الشيء الذي يمكنه أن يكون قاسيًا أو ناعمًا بدون تغير في قساوته؟"
];

function displayPuzzles() {
    const puzzleList = document.getElementById('puzzle-list');
    puzzles.forEach((puzzle, index) => {
        const puzzleElement = document.createElement('div');
        puzzleElement.classList.add('puzzle');
        puzzleElement.innerHTML = `<p>${index + 1}. ${puzzle}</p>`;
        puzzleList.appendChild(puzzleElement);
    });
}

window.onload = displayPuzzles;
