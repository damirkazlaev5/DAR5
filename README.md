<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>Мой сайт</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', sans-serif; }
    body {
      background: linear-gradient(135deg, #8BC34A 0%, #FFEB3B 100%);
      color: #212121; line-height: 1.6; min-height: 200vh; /* чтобы можно было листать */
      position: relative; overflow-x: hidden;
    }
    .snowflake {
      position: fixed; top: -20px; pointer-events: none;
      user-select: none; z-index: 1; opacity: 0.8;
    }
    .container {
      max-width: 900px; margin: 0 auto; padding: 40px 20px;
      position: relative; z-index: 2;
    }
    header { text-align: center; margin-bottom: 50px; }
    h1 {
      font-size: 2.8em; color: #388E3C; text-shadow: 0 2px 4px rgba(0,0,0,0.2);
      animation: glow 2s infinite alternate;
    }
    @keyframes glow {
      0% { text-shadow: 0 0 5px #7CB342; }
      100% { text-shadow: 0 0 20px #FBC02D, 0 0 30px #FFA000; }
    }
    p { font-size: 1.1em; margin: 20px 0; }
    .photo-circle {
      width: 220px; height: 220px; border-radius: 50%; object-fit: cover;
      border: 6px solid #388E3C; display: block; margin: 30px auto;
      box-shadow: 0 8px 25px rgba(56, 142, 60, 0.4);
      animation: pulse 3s infinite ease-in-out;
    }
    @keyframes pulse {
      0%, 100% { transform: scale(1); }
      50% { transform: scale(1.08); }
    }
    .sticker {
      text-align: center; margin: 40px 0;
    }
    .sticker img {
      width: 160px; height: 160px; border-radius: 25px;
      border: 4px dashed #F57F17; animation: rotate 8s linear infinite;
    }
    @keyframes rotate {
      from { transform: rotate(0deg); }
      to { transform: rotate(360deg); }
    }
    .social-links {
      text-align: center; margin: 40px 0;
    }
    .social-links a {
      display: inline-block; margin: 0 18px; color: #388E3C;
      text-decoration: none; font-weight: 600; font-size: 1.15em;
      padding: 14px 28px; border-radius: 60px;
      background: rgba(255, 235, 59, 0.3); backdrop-filter: blur(8px);
      transition: all 0.4s cubic-bezier(0.25, 0.8, 0.25, 1);
    }
    .social-links a:hover {
      background: #F57F17; color: white; transform: translateY(-4px);
      box-shadow: 0 10px 25px rgba(245, 127, 23, 0.5);
    }
    .facts {
      background-color: rgba(255, 255, 255, 0.9); padding: 30px;
      border-radius: 20px; margin: 40px 0; border: 3px solid #8BC34A;
      backdrop-filter: blur(12px);
    }
    .facts h3 {
      color: #388E3C; margin-bottom: 25px; text-align: center;
      font-size: 1.5em; text-shadow: 0 1px 3px rgba(0,0,0,0.1);
    }
    .facts ul { list-style: none; padding: 0; }
    .facts li {
      margin: 20px 0; padding-left: 40px; position: relative;
      animation: slideIn 1.2s forwards; opacity: 0;
    }
    .facts li::before {
      content: '✓'; position: absolute; left: 0; color: #F57F17;
      font-weight: bold;
    }
    .facts li:nth-child(1) { animation-delay: 0.2s; }
    .facts li:nth-child(2) { animation-delay: 0.4s; }
    .facts li:nth-child(3) { animation-delay: 0.6s; }
    .facts li:nth-child(4) { animation-delay: 0.8s; }
    .facts li:nth-child(5) { animation-delay: 1s; }
    @keyframes slideIn {
      from { transform: translateX(-40px); opacity: 0; }
      to { transform: translateX(0); opacity: 1; }
    }
    .course {
      background-color: rgba(255, 255, 255, 0.9); padding: 30px;
      border-radius: 20px; margin: 40px 0; border: 3px solid #FFEB3B;
      backdrop-filter: blur(12px);
    }
    .course h3 {
      color: #F57F17; margin-bottom: 25px; text-align: center;
      font-size: 1.5em; text-shadow: 0 1px 3px rgba(0,0,0,0.1);
    }
    .course a {
      display: block; margin: 18px 0; color: #388E3C;
      text-decoration: none; padding: 14px; border-radius: 10px;
      transition: background 0.3s, transform 0.3s;
      font-size: 1.1em;
    }
    .course a:hover {
      background: rgba(139, 195, 74, 0.2); transform: translateX(8px);
      border-left: 4px solid #388E3C;
    }
    footer {
      text-align: center; margin-top: 60px; color: #555;
      font-size: 0.95em; padding: 20px 0;
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <h1>Обо мне</h1>
      <p>Привет! Меня зовут Дамир. Здесь — моя маленькая онлайн‑вселенная.</p>
    </header>


    <img src="https://media1.tenor.com/m/6GVWF941OdoAAAAC/artem686.gif" alt="Моё фото" class="photo-circle">


    <div class="sticker">
      <img src="https://media1.tenor.com/m/6GVWF941OdoAAAAC/artem686.gif" alt="Стикер">
    </div>


   <h1>t.me/Scratch5pro - Мой тг канал </h1>
    <div class    <div class="facts">
      <h3>Несколько фактов обо мне:</h3>
      <ul>
        <li>Люблю программировать на HTML.</li>
        <li>Увлекаюсь программирование.</li>
        <li>Люблю математику.</li>
        <li>Мечтаю побывать в Японии.</li>
        <li>Ноутбук — мой лучший друг утром.</li>
      </ul>
    </div>


    <footer>
      &copy; 2025 [Ваше имя]. Все права защищены. Создателю картинки выражается благодарность.
    </footer>
  </div>

  <script>
    // Массив смайликов для снега (15 видов)
    const snowflakes = [
      '☃', '❄️', '🌨', '❅', '❆', '✽', '✾', '❁',
      '❀', '❂', '❃', '❊', '❋', '❍', '❎'
    ];

    function createSnowflake() {
      const snowflake = document.createElement('div');
      snowflake.classList.add('snowflake');
      
      // Выбираем случайный смайлик
      snowflake.innerHTML = snowflakes[Math.floor(Math.random() * snowflakes.length)];
      
      // Случайные параметры
      snowflake.style.fontSize = `${Math.random() * 20 + 10}px`;
      snowflake.style.left = `${Math.random() * window.innerWidth}px`;
      snowflake.style.opacity = Math.random() * 0.7 + 0.3;
      snowflake.style.animationDuration = `${Math.random() * 12 + 10}s`; // Медленное падение (10–22 сек)
      snowflake.style.animationTimingFunction = 'linear';

      document.body.appendChild(snowflake);

      // Анимация падения
      const fallAnimation = snowflake.animate([
        { transform: 'translateY(0)' },
        { transform: `translateY(${window.innerHeight + 100}px)` }
      ], {
        duration: parseInt(snowflake.style.animationDuration) * 1000,
        fill: 'forwards'
      });

      // Перезапуск анимации при завершении (бесконечный цикл)
      fallAnimation.onfinish = () => {
        // Возвращаем снежинку наверх и меняем горизонтальную позицию
        snowflake.style.top = '-50px';
        snowflake.style.left = `${Math.random() * window.innerWidth}px`;
        
        // Запускаем анимацию заново
        fallAnimation.play();
      };
    }

    // Создаём снежинки каждые 600 мс
    setInterval(createSnowflake, 600);

    // Первоначальное создание 25 снежинок
    for (let i = 0; i < 25; i++) {
      createSnowflake();
    }
  </script>
</body>
</html>
