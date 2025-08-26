#Home-work-36   (TypeScript homework)


## 📌 Опис
Ця домашка містить розв'язання базових завдань на **TypeScript**:
1. `sumArray` — функція для підрахунку суми елементів масиву.
2. `createUser` — функція для створення користувача з використанням типу `User`.
3. `getOrderStatus` — функція для визначення статусу замовлення з використанням `enum`.

Проєкт налаштований так, щоб можна було запускати код у браузері та переглядати результати у **Console**.

---

## ⚙️ Встановлення та запуск

## 1. Клонування репозиторію :

git clone <repo-url>
cd <project-folder>

## 2. Ініціалізація проєкту :

npm init -y
npm install typescript --save-dev

## 3. Налаштування TypeScript
У файлі tsconfig.json приклад мінімальних налаштувань:
{
  "compilerOptions": {
    "target": "es6",
    "module": "es6",
    "outDir": "./dist",
    "rootDir": "./src",
    "strict": true
  }
}


## 4. Компіляція TypeScript :

npx tsc

Файл main.ts з каталогу src/ буде скомпільовано у dist/main.js.

## 5. Запуск у браузері :

Використовуй Live Server у VS Code (або інший локальний сервер).

Відкрий index.html, і результати побачиш у Console.


📂 Структура проєкту

home-work-36/
│── src/
│   ├── main.ts       # TypeScript код із завданнями
│── dist/
│   └── main.js       # Скомпільований JS
│── tsconfig.json
│── package.json
│── README.md
└── index.html    # HTML для запуску в браузері


🚀 Приклади використання

// #1
console.log(sumArray([1, 2, 3, 4])); // 10
console.log(sumArray([]));           // 0

// #2
const newUser = createUser('Анна', 25);
console.log(newUser); // { name: "Анна", age: 25, isActive: true }

// #3
console.log(getOrderStatus(OrderStatus.Pending));       // 'Замовлення очікує на обробку'
console.log(getOrderStatus(OrderStatus.Shipped));      // 'Замовлення було відправлено'
console.log(getOrderStatus(OrderStatus.Delivered));   // 'Замовлення доставлено'
console.log(getOrderStatus(OrderStatus.Cancelled));  //  'Замовлення скасовано'

- export { sumArray, createUser, OrderStatus, getOrderStatus }



📖 Примітки

- Використовуй npx tsc --watch, щоб автоматично перекомпілювати файли при зміні коду.

- Переконайся, що відкриваєш index.html через Live Server, а не напряму з файлової системи (file://).
