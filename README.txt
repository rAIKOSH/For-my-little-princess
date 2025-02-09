<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Для Любимой Девочки ❤️</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Arial', sans-serif;
      background: linear-gradient(135deg, #ff7eb3, #ffc3a0);
      color: #fff;
      position: relative;
      min-height: 100vh;
      overflow: hidden;
    }
    .container {
      text-align: center;
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      z-index: 10;
    }
    h1 {
      font-size: 3rem;
      color: #fff;
      animation: fadeIn 2s ease-in-out;
    }
    #message {
      font-size: 1.5rem;
      animation: fadeText 3s linear infinite alternate;
    }

    @keyframes fadeText {
      0% { opacity: 0; }
      100% { opacity: 1; }
    }

    /* Водопад сердечек и эмодзи */
    .emoji {
      position: absolute;
      font-size: 24px;
      animation: fallDown 5s infinite ease-in;
    }

    @keyframes fallDown {
      0% {
        transform: translateY(-10vh) rotate(0deg);
        opacity: 1;
      }
      100% {
        transform: translateY(100vh) rotate(720deg);
        opacity: 0;
      }
    }

    /* Кнопка для открытия романтического письма */
    button {
      margin-top: 20px;
      padding: 10px 20px;
      font-size: 1.2rem;
      background-color: #e63946;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      transition: background-color 0.3s;
    }

    button:hover {
      background-color: #ff1b5b;
    }

    /* Письмо */
    .letter {
      display: none;
      background: white;
      color: #333;
      padding: 20px;
      border-radius: 10px;
      max-width: 600px; /* Увеличена ширина */
      margin: 20px auto;
      font-size: 1rem;
      text-align: left;
      line-height: 1.5;
      max-height: 80vh; /* Ограничение по высоте */
      overflow-y: auto; /* Добавляем прокрутку для письма */
      box-shadow: 0 0 15px rgba(0, 0, 0, 0.2);
    }

    .letter.show {
      display: block;
      animation: fadeInLetter 1.5s ease-out forwards;
    }

    @keyframes fadeInLetter {
      0% {
        opacity: 0;
        transform: translateY(20px);
      }
      100% {
        opacity: 1;
        transform: translateY(0);
      }
    }

    /* Анимация появления текста "Я люблю тебя ❤️" */
    .floating-text {
      position: absolute;
      font-size: 1.5rem;
      color: white;
      opacity: 0;
      animation: fadeInOutText 6s infinite;
      word-wrap: break-word; /* Предотвращаем выход текста за пределы */
    }

    @keyframes fadeInOutText {
      0%, 100% { opacity: 0; transform: translateY(10px); }
      50% { opacity: 1; transform: translateY(0); }
    }

    /* Медиазапросы для адаптивности */
    @media (max-width: 768px) {
      h1 {
        font-size: 2.5rem;
      }

      #message {
        font-size: 1.2rem;
      }

      .letter {
        max-width: 90%; /* Уменьшаем ширину письма для мобильных устройств */
        font-size: 0.9rem;
      }

      .floating-text {
        font-size: 1.2rem; /* Уменьшаем размер текста */
      }

      button {
        font-size: 1rem;
        padding: 8px 16px;
      }
    }

    @media (max-width: 480px) {
      h1 {
        font-size: 2rem;
      }

      #message {
        font-size: 1rem;
      }

      .letter {
        max-width: 90%;
        font-size: 0.85rem;
      }

      .floating-text {
        font-size: 1rem;
      }

      button {
        font-size: 0.9rem;
        padding: 8px 16px;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Я люблю тебя ❤️</h1>
    <p id="message">Ты моя маленькая принцесса!!!</p>
    <button onclick="showLetter()">Клик 💌</button>
    <div class="letter" id="romanticLetter">
      Дорогая Дәшөн❤️,
      <br><br>
      Каждое мгновение с тобой — это подарок. Твоя улыбка озаряет мои дни, а твое тепло наполняет мое сердце любовью. Ты вдохновляешь меня быть лучше каждый день.
      <br><br>
      Ты моё счастье и радость в этом пустом и черном мире. Благодаря тебе я узнал что такое любовь, что такое жизнь, рядом с тобой я словно маленький ребенок. Твоя поддержка, забота, любовь спасают меня каждый день, я не знаю как тебя отблагодарить за всё что ты делаешь и делала для меня. Я тебя очень сильно люблю и горжусь тобой, я верю тебе и в твои усилий, ты много учишся и стараешься, я верю что у тебя всё получиться и сдашь все экзамены тоже на все 100%. Я буду всегда рядом, в горе и радости я  буду с тобой, даже если весь мир станет против тебя, я буду вериь только одной тебе. Ты моё чудо и спасибо тебе за появление и спасение в моей темной жизни, ты изменила меня в лучшую сторону, я буду стараться ради тебя одного, ведь ты единсвенное что у меня есть на это белом свете. Я тебя очень сильно люблю моя маленькая принцесса❤️
      <br><br>
      Твой Райкош ❤️
    </div>
  </div>

  <script>
    const emojis = ['❤️', '💖', '💘', '💕', '🌹', '✨', '💑', '💍', '🎶', '💌', '💫', '🌸', '💙', '💚', '💛'];
    const phrases = ["Я люблю тебя ❤️", "Ты моё счастье ❤️", "Навсегда вместе 💑", "Ты моё вдохновение 🌹", "Ты моё чудо 💘", "Ты моя звезда ✨", "Моя маленькая принцесса 💖"];

    function createEmojiFall() {
      const emojiElement = document.createElement('div');
      emojiElement.className = 'emoji';
      emojiElement.textContent = emojis[Math.floor(Math.random() * emojis.length)];
      emojiElement.style.left = `${Math.random() * 100}vw`;
      emojiElement.style.animationDuration = `${4 + Math.random() * 3}s`;
      document.body.appendChild(emojiElement);

      setTimeout(() => emojiElement.remove(), 7000);
    }

    function createFloatingText() {
      const textElement = document.createElement('div');
      textElement.className = 'floating-text';
      textElement.textContent = phrases[Math.floor(Math.random() * phrases.length)];
      textElement.style.left = `${Math.random() * 100}vw`;
      textElement.style.top = `${Math.random() * 80}vh`;
      textElement.style.animationDuration = `${5 + Math.random() * 3}s`;
      document.body.appendChild(textElement);

      setTimeout(() => textElement.remove(), 7000);
    }

    function showLetter() {
      const letter = document.getElementById('romanticLetter');
      letter.classList.add('show');
    }

    // Запуск водопада эмодзи и появления текста
    setInterval(createEmojiFall, 500);
    setInterval(createFloatingText, 3000);
  </script>
</body>
</html>
