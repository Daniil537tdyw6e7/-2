<!DOCTYPE html>
<html lang="ru">
  <head>
    <meta charset="UTF-8" />
    <meta
      name="viewport"
      content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0"
    />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <link rel="stylesheet" href="../static/css/style.css" />
    <title>Портфолио</title>
  </head>
  <body>
    <header class="header">
      <nav class="header__nav main-nav">
        <ul class="main-nav__list main-list">
          <li class="main-list__item list-item">
            <a class="list-item__link" href="#дом">ДОМ</a>
          </li>
          <li class="main-list__item list-item">
            <a class="list-item__link" href="#обо мне">обо мне</a>
          </li>
          <li class="main-list__item list-item">
            <a class="list-item__link" href="#способности">мои спсобности</a>
          </li>
        </ul>
      </nav>
    </header>
    <main class="main">
      <!-- Секция превью -->
      <section class="main__home home" id="ДОМ">
        <h1 class="home__title">Даниил Сальшин</h1>
        <p class="home__subtitle">программы на пайтоне</p>
      </section>
      <!-- Секция с рассказом о себе -->
      <section class="main__about about" id="обо мне">
        <h2 class="about__title">ABOUT ME</h2>
        <div class="about__info info-block">
          <p class="info-block__text">
            Меня зовут Сальшин Даниил живу в Астрахани, есть малый опыт в програмировании. могу сделать хорошего проработанного бота в тг.
            Учусь в 7 классе в обычной школе, обучаюсь програмированию в онлайн школе Kodland 
          </p>
          <img
            class="info-block__img"
            src="../static/img/profile.png"
            alt="me"
            width="250"
            height="250"
          />
        </div>
      </section>
      <!-- Секция со скиллами -->
      <section class="main__skills skills" id="skills">
        <h2 class="skills__title">мои спсобности</h2>
        <form action="/" method="POST">
          <ul class="skills__list skills-list">
            <li class="skills-list__skill skill">
              <img
                class="skill__img"
                src="../static/img/python.png"
                alt="python"
                width="150"
                height="150"
              />
              <span class="skill__info">Skill info</span>
              <input class="skill__button" type="submit" name="button_python" value="SHOW PROJECT">
            </li>
            <li class="skills-list__skill skill">
              <img
                class="skill__img"
                src="../static/img/discord.png"
                alt="discord"
                width="150"
                height="150"
              />
              <span class="skill__info">Skill info</span>
              <input class="skill__button" type="submit" name="button_discord" value="SHOW PROJECT">
            </li>
            <li class="skills-list__skill skill">
              <img
                class="skill__img"
                src="../static/img/html.png"
                alt="html"
                width="150"
                height="150"
              />
              <span class="skill__info">Skill info</span>
              <input class="skill__button" type="submit" name="button_html" value="SHOW PROJECT">
            </li>
            <li class="skills-list__skill skill">
              <img
                class="skill__img"
                src="../static/img/db.webp"
                alt="SQL"
                width="150"
                height="150"
              />
              <span class="skill__info">Skill info</span>
              <input class="skill__button" type="submit" name="button_db" value="SHOW PROJECT">
            </li>
          </ul>
        </form>
        {% if button_python%}
          <div class="skills__project project" id="project">
              <img class="project__img" src="../static/img/python-project.png" alt="project" width="500">
              <a class="project__link" href="">Открыть на GitHub</a>
          </div>
        {% endif %}
      </section>
      <!-- Секция с формой обратной связи -->
      <section class="main__feedback feedback" id="feedback">
        <h2 class="feedback__title">FEEDBACK</h2>
        <form action="" method="POST" class="feedback__form form">
          <label for="email">
            <input type="email" class="form__input" name="email" id="email" placeholder="сюда почту всою напиши" required>
          </label>
          <label for="text">
            <textarea name="text" class="form__input" id="text" cols="70" rows="10" required placeholder="напиши что нибудь..."></textarea>
          </label>
          <button class="form__button" type="submit">тык</button>
        </form>
      </section>
    </main>
    <!-- Подвал для ссылок на соц-сети -->
    <footer>
мой телеграм @BsDan3
    </footer>
  </body>
</html>
