[Ильяс открытка.html](https://github.com/user-attachments/files/25824333/default.html)
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>С 8 Марта! 🌷</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Roboto, 'Helvetica Neue', sans-serif;
            background: linear-gradient(145deg, #f9e3e3 0%, #f8d5d5 100%);
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 16px;
            position: relative;
            overflow-x: hidden;
        }

        /* анимированные цветы на фоне */
        .floating-flowers {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            pointer-events: none;
            z-index: 1;
            overflow: hidden;
        }

        .flower {
            position: absolute;
            font-size: 2.2rem;
            opacity: 0.2;
            animation: float 18s infinite ease-in-out;
            filter: drop-shadow(0 8px 12px rgba(232, 120, 168, 0.2));
            transform-origin: center;
        }

        .flower:nth-child(1) { top: 5%; left: 3%; animation-duration: 22s; font-size: 3rem; }
        .flower:nth-child(2) { bottom: 12%; right: 2%; animation-duration: 19s; font-size: 4rem; opacity: 0.18; }
        .flower:nth-child(3) { top: 20%; right: 15%; animation-duration: 24s; font-size: 2.8rem; }
        .flower:nth-child(4) { bottom: 25%; left: 12%; animation-duration: 21s; font-size: 3.5rem; }
        .flower:nth-child(5) { top: 70%; left: 25%; animation-duration: 26s; font-size: 2.5rem; }
        .flower:nth-child(6) { top: 10%; left: 40%; animation-duration: 20s; font-size: 3.2rem; }
        .flower:nth-child(7) { bottom: 40%; right: 20%; animation-duration: 23s; font-size: 3.8rem; }

        @keyframes float {
            0% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-25px) rotate(8deg); }
            100% { transform: translateY(0px) rotate(0deg); }
        }

        .card {
            position: relative;
            z-index: 10;
            max-width: 800px;
            width: 100%;
            background: rgba(255, 255, 255, 0.8);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border-radius: 56px 56px 48px 48px;
            box-shadow: 0 35px 90px -10px rgba(210, 90, 130, 0.45), 0 10px 25px -8px rgba(180, 60, 100, 0.3);
            padding: 40px 30px 45px 30px;
            border: 1px solid rgba(255, 220, 240, 0.6);
            transition: all 0.2s;
        }

        /* шапка с мимозой */
        .header-decoration {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-bottom: 10px;
            flex-wrap: wrap;
        }

        .blossom {
            font-size: 3.3rem;
            line-height: 1;
            filter: drop-shadow(2px 6px 12px #fba0c0);
            animation: gentleWave 4s infinite alternate;
        }

        .blossom:nth-child(2) { animation-delay: 0.7s; }
        .blossom:nth-child(3) { animation-delay: 1.3s; }

        @keyframes gentleWave {
            from { transform: translateY(0px) rotate(-2deg); }
            to { transform: translateY(-10px) rotate(3deg); }
        }

        h1 {
            font-size: 3.2rem;
            font-weight: 700;
            color: #b23b5e;
            text-align: center;
            margin: 10px 0 10px;
            letter-spacing: 2px;
            text-shadow: 3px 3px 0 #ffe2ec;
            line-height: 1.2;
        }

        .subhead {
            font-size: 1.5rem;
            color: #972b4f;
            text-align: center;
            font-weight: 400;
            background: rgba(255, 235, 245, 0.6);
            display: inline-block;
            padding: 8px 32px;
            border-radius: 60px;
            margin: 0 auto 30px;
            backdrop-filter: blur(4px);
            box-shadow: inset 0 1px 4px #ffd9e6;
            border: 1px solid #ffe3ef;
        }

        .greeting-message {
            background: rgba(255, 250, 245, 0.7);
            border-radius: 48px;
            padding: 38px 28px;
            margin: 25px 0 30px;
            box-shadow: inset 0 2px 10px #ffeef4, 0 18px 25px -16px #d98ba5;
            border: 1px solid #ffe1ed;
        }

        .greeting-message p {
            font-size: 1.5rem;
            line-height: 1.6;
            color: #3d232e;
            text-align: center;
            font-weight: 450;
        }

        .greeting-message p i {
            color: #c7426f;
            font-style: italic;
            font-weight: 500;
            background: linear-gradient(135deg, #fdd1df, #ffe7f0);
            padding: 4px 12px;
            border-radius: 40px;
            display: inline-block;
            margin: 4px 0;
        }

        .flower-bouquet {
            display: flex;
            justify-content: center;
            gap: 18px;
            margin: 30px 0 20px;
            font-size: 3rem;
            filter: drop-shadow(0 8px 16px #e1a0b6);
        }

        .flower-bouquet span {
            display: inline-block;
            animation: bounceFlower 2.4s infinite ease-in-out;
            transform-origin: bottom;
        }

        .flower-bouquet span:nth-child(2) { animation-delay: 0.2s; }
        .flower-bouquet span:nth-child(3) { animation-delay: 0.5s; }
        .flower-bouquet span:nth-child(4) { animation-delay: 0.1s; }
        .flower-bouquet span:nth-child(5) { animation-delay: 0.6s; }
        .flower-bouquet span:nth-child(6) { animation-delay: 0.3s; }
        .flower-bouquet span:nth-child(7) { animation-delay: 0.4s; }

        @keyframes bounceFlower {
            0%, 100% { transform: translateY(0) rotate(0deg); }
            50% { transform: translateY(-12px) rotate(2deg); }
        }

        .wishes-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 14px;
            justify-content: center;
            margin: 40px 0 30px;
        }

        .wish-item {
            background: rgba(255, 255, 255, 0.8);
            border-radius: 60px;
            padding: 12px 22px;
            font-size: 1.25rem;
            font-weight: 500;
            color: #851e44;
            box-shadow: 0 6px 0 #e6a6bc, 0 12px 22px -10px #c96f90;
            border: 1px solid white;
            backdrop-filter: blur(4px);
            transition: 0.15s;
            display: inline-flex;
            align-items: center;
            gap: 8px;
        }

        .wish-item:hover {
            transform: scale(1.07) translateY(-4px);
            background: #fff0f5;
            box-shadow: 0 8px 0 #d981a4, 0 20px 26px -12px #b94b74;
        }

        .signature {
            text-align: right;
            font-size: 1.8rem;
            font-weight: 600;
            color: #90284e;
            margin-top: 35px;
            border-top: 2px dashed #feb4cb;
            padding-top: 25px;
            padding-right: 12px;
            font-style: italic;
            background: linear-gradient(to left, #ffe3ed, transparent);
            border-radius: 0 0 30px 0;
        }

        .signature span {
            background: #ffe6f0;
            padding: 6px 22px;
            border-radius: 60px;
            font-size: 1.8rem;
            display: inline-block;
            box-shadow: 0 4px 0 #dd9bb3;
        }

        .button-music {
            display: flex;
            justify-content: center;
            margin: 25px 0 5px;
        }

        .play-btn {
            background: #ffe2ed;
            border: 2px solid white;
            padding: 14px 36px;
            border-radius: 50px;
            font-size: 1.3rem;
            font-weight: 600;
            color: #a12d55;
            box-shadow: 0 5px 0 #d88dab, 0 10px 18px -10px #b44c75;
            cursor: pointer;
            transition: 0.08s linear;
            display: inline-flex;
            align-items: center;
            gap: 12px;
            backdrop-filter: blur(6px);
            background: rgba(255, 241, 245, 0.85);
            border: 1px solid #ffc1d4;
        }

        .play-btn:active {
            transform: translateY(5px);
            box-shadow: 0 2px 0 #d88dab, 0 6px 14px -8px #b44c75;
        }

        /* пожелание внизу */
        .footer-note {
            text-align: center;
            font-size: 1.1rem;
            color: #ad4870;
            margin: 24px 0 0;
            font-weight: 400;
            opacity: 0.8;
            letter-spacing: 0.4px;
        }

        .footer-note span {
            display: inline-block;
            animation: sparkle 2s infinite;
        }

        @keyframes sparkle {
            0% { opacity: 1; transform: scale(1); }
            50% { opacity: 0.6; transform: scale(1.05); text-shadow: 0 0 8px #ffb8d2; }
        }

        /* адаптация */
        @media (max-width: 550px) {
            h1 { font-size: 2.6rem; }
            .subhead { font-size: 1.2rem; }
            .greeting-message p { font-size: 1.25rem; }
            .wish-item { font-size: 1rem; padding: 8px 16px; }
            .signature span { font-size: 1.4rem; }
            .card { padding: 30px 18px; }
            .flower-bouquet { font-size: 2.5rem; gap: 8px; }
        }
    </style>
</head>
<body>
    <!-- фон с парящими цветами (символ 8 марта) -->
    <div class="floating-flowers">
        <div class="flower">🌷</div>
        <div class="flower">🌸</div>
        <div class="flower">🌹</div>
        <div class="flower">🌼</div>
        <div class="flower">🌺</div>
        <div class="flower">💐</div>
        <div class="flower">🌻</div>
    </div>

    <main class="card">
        <!-- гирлянда из цветов сверху -->
        <div class="header-decoration">
            <span class="blossom">🌸</span>
            <span class="blossom">🌷</span>
            <span class="blossom">🌼</span>
        </div>

        <h1>С 8 Марта!</h1>
        <div style="text-align: center;">
            <span class="subhead">С праздником всех девушек и женщин</span>
        </div>

        <!-- основной текст и конверт с поздравлением -->
        <div class="greeting-message">
            <p>
                🌷 Дорогие и прекрасные наши дамы! 🌷<br><br>
                <i>Пусть каждый день дарит улыбки,<br>
                цветы и нежность. Оставайтесь<br>
                такими же вдохновляющими,<br>
                как сама весна.</i> ✨
            </p>
        </div>

        <!-- букет анимированный -->
        <div class="flower-bouquet">
            <span>🌷</span>
            <span>🌹</span>
            <span>🌸</span>
            <span>🌼</span>
            <span>🌺</span>
            <span>💐</span>
            <span>🌻</span>
        </div>

        <!-- Сетка тёплых пожеланий (комплименты) -->
        <div class="wishes-grid">
            <span class="wish-item">💖 Счастья</span>
            <span class="wish-item">🌹 Любви</span>
            <span class="wish-item">✨ Удачи</span>
            <span class="wish-item">🌺 Вдохновения</span>
            <span class="wish-item">🍃 Нежности</span>
            <span class="wish-item">🌟 Улыбок</span>
            <span class="wish-item">☀️ Тепла</span>
            <span class="wish-item">🌸 Цветов</span>
        </div>

        <!-- интерактивная кнопка (имитация музыки/поздравления) -->
        <div class="button-music">
            <button class="play-btn" id="magicBtn">
                <span>🎵</span> Поздравить <span>🎤</span>
            </button>
        </div>

        <!-- подпись с именем (можете изменить) -->
        <div class="signature">
            <span>С 8 Марта! 💐</span>
        </div>

        <!-- маленький футер с дополнительной тёплостью -->
        <div class="footer-note">
            <span>🌷</span> Пусть исполняются мечты <span>🌷</span>
        </div>
    </main>

    <script>
        (function() {
            const button = document.getElementById('magicBtn');
            // Массив тёплых сообщений, которые будут появляться при клике
            const messages = [
                "💐 Будьте счастливы, любимы и неповторимы!",
                "🌹 Пусть весна играет яркими красками в вашей душе!",
                "🌸 Сияйте, как миллион тюльпанов!",
                "🌼 С 8 Марта! Пусть каждый день пахнет цветами и радостью.",
                "💖 Оставайтесь королевами своего сердца!",
                "🌷 Море улыбок, океан цветов и любви!",
                "✨ Пусть все невзгоды обходят стороной.",
                "🎉 С праздником, наши прекрасные!"
            ];

            // Заранее подготовим скрытое аудио (можно было бы встроить, но без звука — только текст)
            // Но добавим шуточное "поздравление" через всплывающее уведомление и alert, но чтобы не раздражало,
            // сделаем красивое модальное окошко через свой попап (div), чтобы было стильно.
            // Но чтобы не усложнять — сделаем простой alert с ярким поздравлением,
            // а также добавим эффект конфетти (можно использовать простой канфетти через js).
            // Для эстетики — без навязчивости: используем не alert, а временное сообщение (тост) сверху кнопки.

            // Создадим элемент для отображения всплывающего сообщения
            const toast = document.createElement('div');
            toast.style.position = 'fixed';
            toast.style.bottom = '30px';
            toast.style.left = '50%';
            toast.style.transform = 'translateX(-50%)';
            toast.style.backgroundColor = '#ffd9e8';
            toast.style.color = '#911f4b';
            toast.style.padding = '18px 30px';
            toast.style.borderRadius = '80px';
            toast.style.fontSize = '1.5rem';
            toast.style.fontWeight = '600';
            toast.style.boxShadow = '0 15px 35px #e09bb6, 0 5px 0 #cf85a5';
            toast.style.zIndex = '9999';
            toast.style.border = '2px solid #ffffff';
            toast.style.backdropFilter = 'blur(12px)';
            toast.style.transition = 'opacity 0.3s, bottom 0.3s';
            toast.style.opacity = '0';
            toast.style.pointerEvents = 'none';
            toast.style.textAlign = 'center';
            toast.style.lineHeight = '1.4';
            toast.style.letterSpacing = '0.5px';
            document.body.appendChild(toast);

            // функция показа сообщения
            function showMessage(text) {
                toast.textContent = text;
                toast.style.opacity = '1';
                toast.style.bottom = '50px';
                // Добавим иконку в начало
                toast.innerHTML = '💐 ' + text + ' 🌷';
                setTimeout(() => {
                    toast.style.opacity = '0';
                    toast.style.bottom = '30px';
                }, 2800);
            }

            // при клике показываем рандомное пожелание
            button.addEventListener('click', () => {
                const randomIndex = Math.floor(Math.random() * messages.length);
                const msg = messages[randomIndex];
                showMessage(msg);

                // дополнительная "магия": немного цветов в консоль и анимация на кнопке
                button.style.transform = 'scale(0.95)';
                setTimeout(() => button.style.transform = '', 150);

                // можно менять местами цветочки в букете (шалость)
                const bouquet = document.querySelector('.flower-bouquet');
                if (bouquet) {
                    const children = bouquet.children;
                    if (children.length > 1) {
                        // просто легкая перестановка для веселья
                        let last = children[children.length-1].innerHTML;
                        for (let i = children.length-1; i > 0; i--) {
                            children[i].innerHTML = children[i-1].innerHTML;
                        }
                        children[0].innerHTML = last;
                    }
                }
            });

            // Ховер-эффект для кнопки (и так есть в css, но добавим дополнительный звук мысленно)
            // Также создадим приветствие при загрузке (тост)
            window.addEventListener('load', () => {
                setTimeout(() => {
                    showMessage('🌷 С праздником весны! 🌷');
                }, 600);
            });

            // второй вариант — добавить floating частицы при клике (можно было бы сделать конфетти),
            // но ограничимся изящным тостом. 
            // А еще красиво — меняем background градиента ненадолго при клике.
            button.addEventListener('click', () => {
                document.body.style.transition = 'background 0.8s';
                document.body.style.background = 'linear-gradient(145deg, #ffe0f0 0%, #fccfdf 100%)';
                setTimeout(() => {
                    document.body.style.background = 'linear-gradient(145deg, #f9e3e3 0%, #f8d5d5 100%)';
                }, 600);
            });

            // легкое дрожание цветов при наведении на карточку — необязательно
            // добавим реакцию на букет
            const flowers = document.querySelectorAll('.flower-bouquet span');
            flowers.forEach((f, index) => {
                f.addEventListener('mouseenter', () => {
                    f.style.animation = 'none';
                    f.offsetHeight; // форсим рефлоу
                    f.style.animation = 'bounceFlower 0.8s infinite';
                });
                f.addEventListener('mouseleave', () => {
                    f.style.animation = 'bounceFlower 2.4s infinite ease-in-out';
                });
            });
        })();
    </script>

    <!-- небольшой сюрприз: бегущая строка в консоли -->
    <script>
        console.log('%c🌷 С 8 МАРТА! 🌷', 'font-size: 30px; color: #c92f6b; background: #ffe9f2; padding: 8px 18px; border-radius: 40px;');
        console.log('%cПусть весна подарит нежность и цветы!', 'font-size: 18px; color: #942952;');
    </script>
</body>
</html>
