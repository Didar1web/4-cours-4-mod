# 4-cours-4-mod
/* Общие стили */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    color: #333;
}

header {
    background-color: #4CAF50;
    color: white;
    text-align: center;
    padding: 20px 0;
}

footer {
    background-color: #4CAF50;
    color: white;
    text-align: center;
    padding: 10px 0;
}

/* Контейнер для контента */
.container {
    display: flex;
    flex-direction: column;
    gap: 20px;
    padding: 20px;
}

.content-box {
    background-color: white;
    padding: 15px;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.content-box img {
    width: 100%;
    height: auto;
    border-radius: 5px;
}

/* Мобильный вид (по умолчанию) */
@media (max-width: 771px) {
    .container {
        flex-direction: column;
    }

    .content-box {
        width: 100%;
    }

    .content-box img {
        max-height: 30vh;
    }
}

/* Планшетный вид (размер экрана >= 772px) */
@media (min-width: 772px) {
    .container {
        flex-direction: row;
        justify-content: space-between;
    }

    .content-box {
        width: 45%;
    }

    .content-box img {
        max-height: 30vh;
    }
}

/* Широкоэкранный вид (размер экрана >= 998px) */
@media (min-width: 998px) {
    .container {
        flex-direction: row;
        justify-content: space-between;
    }

    .content-box {
        width: 30%;
    }
}

