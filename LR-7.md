---
# 🧪 Лабораторна робота 7
---

### 🔹 Крок 1. Запуск контейнера

Виконайте команду в терміналі:

```bash
docker run -d --rm -p 7080:5000 gprestes/the-internet:v2.6.5
```
<img width="1163" height="250" alt="image" src="https://github.com/user-attachments/assets/e270126f-660c-46b8-b4f0-58e9062c07a4" />

---

### 🔹 Крок 2. Перевірка запуску

Відкрийте в браузері:

```
http://localhost:7080
```

<img width="1919" height="1019" alt="image" src="https://github.com/user-attachments/assets/b28a250c-9cb0-4c03-b78c-fc296188ede9" />


---

### 🔹 Крок 3. Ознайомлення з функціоналом

Вручну відкрийте сторінки:
- **Form Authentication**
  <img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/2fa79643-c101-49ff-9f62-0b344040c520" />

- **Add/Remove Elements**
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/42eb0b08-03f2-4377-a28a-6d1c4a0d95b3" />


---

## 🅱️ Частина B. Створення автотестів у Katalon Recorder

---

## 🔹 Крок 1. Встановлення інструменту

1. Відкрийте Chrome Web Store
2. Знайдіть **Katalon Recorder**
<img width="1919" height="1076" alt="image" src="https://github.com/user-attachments/assets/51b08361-dc89-4515-afae-d19d6058e7cc" />

3. Встановіть розширення
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/7642de54-9a2b-4081-9999-260cabaa9c54" />

4. Відкрийте його через меню розширень
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/1bad74f1-df4e-44d8-b4a5-97fe83695831" />

---

## 🔹 Крок 2. Створення проєкту

1. Створіть **Test Suite** з назвою:
   ```
   SmokeSuite
   ```
<img width="1324" height="759" alt="image" src="https://github.com/user-attachments/assets/f9b76bb8-c96e-4ff2-970e-327bfd267aba" />

---

## 🔹 Крок 3. Тест №1 — Успішний логін (Positive test)

### Сценарій
1. Відкрити сторінку **Form Authentication**
2. Ввести:
    - username: `tomsmith`
    - password: `SuperSecretPassword!`
  <img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/cf4ca567-4561-44c0-a34f-8e4a7bf44271" />

3. Натиснути кнопку **Login**
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/3a2c1028-d290-4d33-a248-d1f66ed05161" />
---

## 🔹 Крок 4. Тест №2 — Невдалий логін (Negative test)

### Сценарій
1. Відкрити сторінку логіну
2. Ввести неправильний пароль
3. Натиснути **Login**
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/f4c5b30a-227b-4295-9fc6-7024c037bd9f" />


---

## 🔹 Крок 5. Тест №3 — Add / Remove Elements

### Сценарій
1. Відкрити сторінку **Add/Remove Elements**
2. Натиснути **Add Element** 3 раз
3. Перевірити, що на сторінці 3 кнопки **Delete**
  <img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/f2616c82-e728-40fb-8194-f5ab5fed53f9" />
4. Видалити один елемент
5. Перевірити, що залишилось 2 кнопки **Delete**
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/830fb7d0-2b1b-4192-8d3f-fe233bf3f6e8" />

---
