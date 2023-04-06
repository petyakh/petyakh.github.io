---
layout: post
comments: true
excerpt_separator: "<!--more-->"
published: true
title: Як швидко дізнатись збережений пароль від WiFI у Windows
categories: windows

---
Відкриваємо консоль (для цього у пошуковому вікні пишемо: cmd) та вводимо команду:

**netsh wlan show profile “_MyHomeNetwok_” key=clear**

де MyHomeNetwok - назва мережі, пароль якої нас цікавить.

Отримуємо відповідь з деталями про нашу мережу. Значенння в полі Key Content - це і є наш пароль.

Якщо ми не пам'ятаємо точну назву мережі. то список усіх збережених мереж можна отримати за допомогою команди:

**netsh wlan show profile**