<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Показать приглашение</title>
<style>
  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background: linear-gradient(135deg, #74ebd5, #ACB6E5);
    height: 100vh;
    margin: 0;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    color: #333;
    padding: 20px;
  }

  button {
    padding: 15px 30px;
    font-size: 18px;
    border: none;
    border-radius: 30px;
    background: linear-gradient(135deg, #6a11cb 0%, #2575fc 100%);
    color: white;
    cursor: pointer;
    box-shadow: 0 5px 15px rgba(101, 41, 255, 0.4);
    transition: background 0.3s ease;
  }

  button:hover {
    background: linear-gradient(135deg, #2575fc 0%, #6a11cb 100%);
  }

  #imageContainer {
    margin-top: 30px;
    max-width: 100%;
    max-height: 60vh;
  }

  #imageContainer img {
    width: 100%;
    height: auto;
    border-radius: 20px;
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.3);
    display: none; /* Скрываем изначально */
  }
</style>
</head>
<body>

<button id="showBtn">Показать приглашение</button>

<div id="imageContainer" aria-hidden="true">
  <img id="theImage" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSSYboArEuUHNfMnLqXlzI36qiKGUk0Ds5sQw&s" alt="Красивый пейзаж" />
</div>

<script>
  const btn = document.getElementById('showBtn');
  const img = document.getElementById('theImage');

  btn.addEventListener('click', () => {
    if (img.style.display === 'none' || img.style.display === '') {
      img.style.display = 'block';
      btn.textContent = 'АРАЙ ЛОХУШКА ПОВЕЛАСЬ УЭЭЭЭ ХАХАХАХХАХАХАХАХ';
    } else {
      img.style.display = 'none';
      btn.textContent = 'Показать приглашение';
    }
  });
</script>

</body>
</html>
