---
layout: post
comments: true
excerpt_separator: "<!--more-->"
published: true
title: Як дізнатись збережений пароль від WiFI у Windows швидко
categories: windows

---
Відкриваємо консоль (для цього у пошуковому вікні пишемо: cmd) та вводимо команду:

**netsh wlan show profile**

Дана команда виведе список усіх збережених мереж.  

Наступна команда:

**netsh wlan show profile “_MyHomeNetwok_” key=clear**

де MyHomeNetwok - назва мережі, пароль якої нас цікавить. 

Отримуємо відповідь з деталями про нашу мережу. Значенння в полі Key Content - це і буде наш пароль. 