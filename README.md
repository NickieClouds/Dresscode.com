# Dresscode.com
Магазин одежды
/* === Общие анимации === */
* {
    box-sizing: border-box;
    transition: all 0.3s ease;
}

/* === Навигация === */
nav a:hover {
    color: #ffd700;
    transform: scale(1.1);
}

/* === Кнопки === */
.btn {
    display: inline-block;
    margin-top: 10px;
    padding: 10px 20px;
    background: #007bff;
    color: white;
    border: none;
    cursor: pointer;
    text-decoration: none;
    border-radius: 5px;
    transition: background 0.3s, transform 0.2s;
}

.btn:hover {
    background: #0056b3;
    transform: translateY(-3px);
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
}

/* === Карточки товаров === */
.product-card {
    border: 1px solid #ddd;
    padding: 10px;
    text-align: center;
    background: white;
    transition: transform 0.3s, box-shadow 0.3s;
}

.product-card:hover {
    transform: scale(1.05);
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
}

/* === Анимация для переключения темы === */
body {
    transition: background 0.5s, color 0.5s;
}

/* === Плавный скролл === */
html {
    scroll-behavior: smooth;
}

/* === Анимация появления (для секций) === */
section {
    opacity: 0;
    transform: translateY(20px);
    animation: fadeInUp 0.8s ease forwards;
}

/* === Ключевые кадры для анимации === */
@keyframes fadeInUp {
    from {
        opacity: 0;
        transform: translateY(20px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}
