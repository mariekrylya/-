<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="description" content="Портфолио фотографа: съёмки, цены и авторская фотокнига.">
<title>Имя Фотографа — фотографии и истории</title>
<style>
:root {
 
  --paper: #f5f2ec;
 
  --ink: #292923;
 
  --muted: #77756e;
 
  --accent: #a36f4f;
 
  --line: #ded9d0;
 
  --white: #fffefa;
 
}
 
* { box-sizing: border-box; margin: 0; padding: 0; }
 
html { scroll-behavior: smooth; }
 
body {
 
  background: var(--paper);
 
  color: var(--ink);
 
  font-family: Georgia, "Times New Roman", serif;
 
  line-height: 1.6;
 
}
 
a { color: inherit; text-decoration: none; }
 
.wrap {
 
  width: min(1160px, calc(100% - 44px));
 
  margin: 0 auto;
 
}
 
.topbar {
 
  position: absolute;
 
  z-index: 2;
 
  top: 0;
 
  width: 100%;
 
  padding: 25px 0;
 
  color: white;
 
}
 
.nav {
 
  display: flex;
 
  align-items: center;
 
  justify-content: space-between;
 
  gap: 24px;
 
}
 
.brand {
 
  font-size: 16px;
 
  letter-spacing: 2px;
 
  text-transform: uppercase;
 
  white-space: nowrap;
 
}
 
.nav-links {
 
  display: flex;
 
  gap: 25px;
 
  font: 13px Arial, sans-serif;
 
}
 
.nav-links a:hover { color: #e6cbb6; }
 
.hero {
 
  min-height: 720px;
 
  display: grid;
 
  place-items: center;
 
  padding: 130px 20px 80px;
 
  color: white;
 
  text-align: center;
 
  background:
 
    linear-gradient(0deg, rgba(22, 20, 18, .48), rgba(22, 20, 18, .25)),
 
    url("images/hero.jpg") center 45% / cover,
 
    #62594f;
 
}
 
.hero-inner { max-width: 780px; }
 
.eyebrow {
 
  font: 11px Arial, sans-serif;
 
  letter-spacing: 4px;
 
  text-transform: uppercase;
 
}
 
h1 {
 
  margin: 20px 0;
 
  font-size: clamp(46px, 8vw, 88px);
 
  font-weight: 400;
 
  line-height: 1.02;
 
}
 
.hero p {
 
  max-width: 570px;
 
  margin: 0 auto 32px;
 
  font-size: 18px;
 
}
 
.button {
 
  display: inline-block;
 
  padding: 13px 24px;
 
  border: 1px solid currentColor;
 
  font: 12px Arial, sans-serif;
 
  letter-spacing: 1.3px;
 
  text-transform: uppercase;
 
  transition: .2s ease;
 
}
 
.button:hover { background: white; color: var(--ink); }
 
section { padding: 92px 0; }
 
.section-title {
 
  margin-bottom: 38px;
 
  text-align: center;
 
}
 
.section-title h2 {
 
  margin-bottom: 8px;
 
  font-size: clamp(34px, 5vw, 52px);
 
  font-weight: 400;
 
  line-height: 1.1;
 
}
 
.section-title p {
 
  color: var(--muted);
 
  font: 14px Arial, sans-serif;
 
}
 
.gallery {
 
  display: grid;
 
  grid-template-columns: repeat(3, 1fr);
 
  gap: 15px;
 
}
 
.gallery img {
 
  display: block;
 
  width: 100%;
 
  aspect-ratio: 4 / 5;
 
  object-fit: cover;
 
  background: #ddd6ca;
 
  transition: transform .35s;
 
}
 
.gallery a { overflow: hidden; }
 
.gallery a:hover img { transform: scale(1.035); }
 
.about {
 
  background: #eae5dc;
 
}
 
.about-grid {
 
  display: grid;
 
  grid-template-columns: 1fr 1fr;
 
  align-items: center;
 
  gap: 60px;
 
}
 
.about-grid img {
 
  width: 100%;
 
  max-height: 570px;
 
  object-fit: cover;
 
  background: #d7cfc3;
 
}
 
.about-copy h2 {
 
  margin-bottom: 20px;
 
  font-size: clamp(35px, 5vw, 54px);
 
  font-weight: 400;
 
  line-height: 1.1;
 
}
 
.about-copy p {
 
  margin-bottom: 16px;
 
  color: #5f5c55;
 
}
 
.text-link {
 
  display: inline-block;
 
  margin-top: 10px;
 
  padding-bottom: 4px;
 
  border-bottom: 1px solid var(--accent);
 
  color: var(--accent);
 
  font: 13px Arial, sans-serif;
 
}
 
.services {
 
  display: grid;
 
  grid-template-columns: repeat(3, 1fr);
 
  gap: 18px;
 
}
 
.card {
 
  padding: 30px 25px;
 
  border: 1px solid var(--line);
 
  background: rgba(255, 254, 250, .4);
 
}
 
.card h3 {
 
  margin-bottom: 10px;
 
  font-size: 25px;
 
  font-weight: 400;
 
}
 
.card p, .card li {
 
  color: var(--muted);
 
  font: 14px/1.75 Arial, sans-serif;
 
}
 
.price {
 
  display: block;
 
  margin: 22px 0 12px;
 
  color: var(--accent);
 
  font-size: 25px;
 
}
 
.book {
 
  background: #292923;
 
  color: var(--white);
 
}
 
.book-grid {
 
  display: grid;
 
  grid-template-columns: 1fr 1fr;
 
  align-items: center;
 
  gap: 65px;
 
}
 
.book-image {
 
  width: 100%;
 
  max-height: 560px;
 
  object-fit: cover;
 
  background: #59564e;
 
}
 
.book-copy .eyebrow { color: #d6b79c; }
 
.book-copy h2 {
 
  margin: 14px 0 20px;
 
  font-size: clamp(38px, 5vw, 58px);
 
  font-weight: 400;
 
  line-height: 1.08;
 
}
 
.book-copy p {
 
  margin-bottom: 16px;
 
  color: #d0cdc5;
 
}
 
.book-details {
 
  margin: 22px 0 28px;
 
  color: #d0cdc5;
 
  font: 13px/1.9 Arial, sans-serif;
 
}
 
.book .button:hover { background: var(--white); }
 
.contacts {
 
  text-align: center;
 
}
 
.contact-list {
 
  display: flex;
 
  justify-content: center;
 
  flex-wrap: wrap;
 
  gap: 14px;
 
  margin-top: 28px;
 
}
 
.contact-list a {
 
  min-width: 150px;
 
  padding: 14px 20px;
 
  border: 1px solid var(--line);
 
  font: 13px Arial, sans-serif;
 
  transition: .2s;
 
}
 
.contact-list a:hover {
 
  border-color: var(--accent);
 
  color: var(--accent);
 
}
 
footer {
 
  padding: 22px 0;
 
  background: #201f1b;
 
  color: #aaa69e;
 
  text-align: center;
 
  font: 12px Arial, sans-serif;
 
}
 
@media (max-width: 760px) {
 
  .nav { align-items: flex-start; }
 
  .nav-links { justify-content: flex-end; flex-wrap: wrap; gap: 8px 14px; }
 
  .hero { min-height: 620px; }
 
  .gallery { grid-template-columns: repeat(2, 1fr); gap: 10px; }
 
  .about-grid, .book-grid { grid-template-columns: 1fr; gap: 30px; }
 
  .services { grid-template-columns: 1fr; }
 
  section { padding: 68px 0; }
 
}
 
@media (max-width: 480px) {
 
  .wrap { width: min(100% - 30px, 1160px); }
 
  .brand { font-size: 13px; }
 
  .nav-links { font-size: 12px; }
 
  .hero p { font-size: 16px; }
 
}
 
</style>
</head>
<body>
<header class="topbar">
<nav class="wrap nav">
 
  <a class="brand" href="#">Имя Фотографа</a>
 
  <div class="nav-links">
 
    <a href="#works">Работы</a>
 
    <a href="#about">Обо мне</a>
 
    <a href="#prices">Съёмки и цены</a>
 
    <a href="#book">Фотокнига</a>
 
    <a href="#contacts">Контакты</a>
 
  </div>
 
</nav>
 
</header>
<main>
<section class="hero">
 
  <div class="hero-inner">
 
    <div class="eyebrow">Фотограф · Ваш город</div>
 
    <h1>Сохраняю то,<br>что хочется помнить</h1>
 
    <p>Естественные фотографии о людях, близости и моментах, которые делают жизнь особенной.</p>
 
    <a class="button" href="#works">Смотреть работы</a>
 
  </div>
 
</section>
 
<section id="works">
 
  <div class="wrap">
 
    <div class="section-title">
 
      <h2>Избранные работы</h2>
 
      <p>Живые истории — без лишней постановки</p>
 
    </div>
 
    <div class="gallery">
 
      <a href="#contacts"><img src="images/work-1.jpg" alt="Портретная съёмка"></a>
 
      <a href="#contacts"><img src="images/work-2.jpg" alt="Свадебная съёмка"></a>
 
      <a href="#contacts"><img src="images/work-3.jpg" alt="Семейная съёмка"></a>
 
      <a href="#contacts"><img src="images/work-4.jpg" alt="Портрет на природе"></a>
 
      <a href="#contacts"><img src="images/work-5.jpg" alt="История пары"></a>
 
      <a href="#contacts"><img src="images/work-6.jpg" alt="Фотография из путешествия"></a>
 
    </div>
 
  </div>
 
</section>
 
<section class="about" id="about">
 
  <div class="wrap about-grid">
 
    <img src="images/photographer.jpg" alt="Фотограф за работой">
 
    <div class="about-copy">
 
      <div class="eyebrow">Немного обо мне</div>
 
      <h2>Привет, я — фотограф</h2>
 
      <p>Мне важно не просто сделать красивые кадры, а сохранить атмосферу и ваши настоящие эмоции.</p>
 
      <p>Помогу выбрать место, подскажу с образами и бережно проведу через съёмку — даже если вы впервые перед камерой.</p>
 
      <a class="text-link" href="#contacts">Обсудить съёмку →</a>
 
    </div>
 
  </div>
 
</section>
 
<section id="prices">
 
  <div class="wrap">
 
    <div class="section-title">
 
      <h2>Съёмки и цены</h2>
 
      <p>Выберите подходящий формат — детали обсудим лично</p>
 
    </div>
 
    <div class="services">
 
      <article class="card">
 
        <h3>Портретная</h3>
 
        <p>Индивидуальная съёмка в студии или на улице. Помощь с идеей и образами.</p>
 
        <span class="price">от 8 000 ₽</span>
 
        <p>1 час · 20 фотографий в обработке</p>
 
      </article>
 
      <article class="card">
 
        <h3>Семейная</h3>
 
        <p>Тёплая прогулка или домашняя съёмка для семьи, пары или будущих родителей.</p>
 
        <span class="price">от 10 000 ₽</span>
 
        <p>1–1,5 часа · 30 фотографий в обработке</p>
 
      </article>
 
      <article class="card">
 
        <h3>Свадебная</h3>
 
        <p>Репортаж и портреты — с вниманием к деталям и важным моментам вашего дня.</p>
 
        <span class="price">от 15 000 ₽</span>
 
        <p>Стоимость зависит от продолжительности съёмки</p>
 
      </article>
 
    </div>
 
  </div>
 
</section>
 
<section class="book" id="book">
 
  <div class="wrap book-grid">
 
    <img class="book-image" src="images/photobook.jpg" alt="Авторская фотокнига">
 
    <div class="book-copy">
 
      <div class="eyebrow">Авторское издание</div>
 
      <h2>Фотокнига<br>«Название книги»</h2>
 
      <p>Это не просто сборник фотографий, а цельная история о свете, местах и людях. Книга создана для неспешного просмотра и возвращения к любимым кадрам.</p>
 
      <p>Плотные страницы, лаконичная обложка и авторская последовательность снимков превращают её в вещь, которую приятно хранить и дарить.</p>
 
      <div class="book-details">
 
        Формат: 20 × 25 см<br>
 
        Объём: 80 страниц<br>
 
        Цена: 3 500 ₽
 
      </div>
 
      <a class="button" href="https://example.com" target="_blank" rel="noopener">
 
        Купить фотокнигу
 
      </a>
 
    </div>
 
  </div>
 
</section>
 
<section class="contacts" id="contacts">
 
  <div class="wrap">
 
    <div class="section-title">
 
      <h2>Давайте создадим вашу историю</h2>
 
      <p>Напишите мне, чтобы узнать свободные даты и обсудить идею съёмки</p>
 
    </div>
 
    <div class="contact-list">
 
      <a href="mailto:hello@example.com">Email</a>
 
      <a href="https://t.me/your_username" target="_blank" rel="noopener">Telegram</a>
 
      <a href="https://instagram.com/your_username" target="_blank" rel="noopener">Instagram</a>
 
    </div>
 
  </div>
 
</section>
 
</main>
<footer>
© <span id="year"></span> Имя Фотографа · Все права защищены
 
</footer>
<script>
document.getElementById("year").textContent = new Date().getFullYear();
 
</script>
</body>
</html>
 
