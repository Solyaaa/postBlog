# Mini Blog

Простий блог додаток, побудований за допомогою Node.js, Express.js та MongoDB Atlas.

## Проєкт використовує базу даних MongoDB Atlas

Цей проєкт зберігає дані постів у базі даних MongoDB, розміщеній на **MongoDB Atlas**. Щоб налаштувати і запустити проєкт, виконайте наступні кроки:

### Кроки для запуску:

1. **Запустіть сервер:**
   - У терміналі (в папці проєкту) введіть команду:
     ```bash
     node server.js
     ```
   - Ця команда запустить сервер на порту `8001` і підключить ваш проєкт до MongoDB Atlas. Після успішного підключення до бази даних ви побачите повідомлення про успішне підключення.

2. **Запустіть клієнтську частину:**
   - Після запуску сервера, відкрийте файл `index.html` у браузері.
   - Клацніть правою кнопкою миші на `index.html` та виберіть **"Open with Live Server"**, щоб запустити клієнтську частину проєкту за допомогою плагіна Live Server в VSCode.

### Функціональні можливості:

- **Створення постів**: Через інтерфейс користувача ви можете створювати нові пости, заповнивши форму з заголовком, описом та автором.
  
- **Редагування постів**: Кожен пост має кнопку для редагування. Ви можете змінити заголовок, опис або автора посту безпосередньо через інтерфейс.

- **Видалення постів**: Кожен пост також має кнопку для видалення. Натискання на кнопку призведе до видалення посту з бази даних.

  Всі ці зміни (створення, редагування, видалення) здійснюються як на рівні інтерфейсу користувача, так і безпосередньо в базі даних MongoDB.

### Технології, які використовуються:

- **Node.js** для створення серверу.
- **Express.js** для обробки маршрутів.
- **MongoDB Atlas** для зберігання даних.
- **Live Server** для запуску клієнтської частини проєкту у браузері.

### Залежності:

- Express
- MongoDB
- Body-Parser
- CORS

### Підключення до MongoDB Atlas:

1. Створіть акаунт на [MongoDB Atlas](https://www.mongodb.com/cloud/atlas).
2. Створіть кластер і отримайте URI для підключення до вашої бази даних.
3. Замініть відповідні значення в `server.js` для підключення до вашої MongoDB бази даних (замість стандартного URI).
