# Cold-Hot Game

## Описание проекта

Проект "Cold-Hot" представляет собой игру, в которой игрок должен найти спрятанный объект, используя подсказки о его местоположении. Игра разработана с использованием языка PHP и базы данных SQLite для хранения результатов и истории игр. Цель игры — найти объект как можно быстрее, следуя указаниям "тепло" и "холодно", которые даются в зависимости от того, насколько близко игрок к объекту.

Цель игры "Cold-Hot" — найти спрятанный объект на игровом поле как можно быстрее, используя подсказки о близости к объекту. Игрок стремится минимизировать количество ходов и время, необходимое для нахождения объекта.

### Правила игры

- **Игровое поле:** Представляет собой пространство (например, координатную сетку), где спрятан объект.
- **Движения игрока:** Игрок вводит координаты, чтобы угадать, где спрятан объект.
- **Подсказки:** После каждой попытки система сообщает игроку, насколько он близок к объекту:
   - "Горячо" — объект рядом.
   - "Тепло" — игрок приближается к объекту.
   - "Холодно" — игрок далеко от объекта.
- **Победа:** Игрок выигрывает, когда находит точные координаты спрятанного объекта.

## Особенности
- **Игра с использованием IndexedDB**: Все данные о играх (результаты и история) сохраняются в браузере с помощью IndexedDB.
- **История игр**: Игроки могут просматривать историю своих игр, включая количество попыток и результаты.
- **Очистка истории**: Возможность очищать историю игр по запросу.
- **Простой интерфейс**: Чистый и простой в использовании интерфейс для удобных игр.

## Установка и запуск проекта 

1. **Склонируйте репозиторий**:
   ```bash
   git clone https://github.com/KirillSher/cold-hot.git
   ```

2. **Перейдите в каталог проекта**:
   ```bash
   cd cold-hot-web
   ```

3. **Откройте файл index.html в вашем браузере**

4. **Запуск через GitHub Pages**:
    Проект доступен онлайн через GitHub Pages: [Играть в cold-hot](https://kirillsher.github.io/cold-hot-web/)

## Данные и сохранение игр
- **Сохранение ходов**: Все ходы игры автоматически сохраняются в базе данных IndexedDB при помощи библиотеки idb.
- **Воспроизведение игр**: Игроки могут воспроизводить свои предыдущие игры, выбрав их из истории.
- **Запрос историй**: На странице представлена возможность просмотреть все сыгранные партии и их результаты.
