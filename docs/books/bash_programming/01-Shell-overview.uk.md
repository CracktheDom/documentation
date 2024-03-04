---
title: Огляд Shell
author: tianci li
contributors: Ganna Zhyrnova
tags:
  - Вступ до Shell
---

# Основна Інформація

**Що таке Shell?**

Shell називається **командним інтерфейсом** або **інтерпретатором команд**. Він забезпечує програму інтерфейсу системного рівня для користувачів, щоб надсилати запити до ядра Linux для запуску програм.

Представляючи операційну систему, ми згадали таке речення:

> Перехопити **доступ до периферійних пристроїв**. Програмне забезпечення рідко може отримати прямий доступ до апаратного забезпечення (за винятком відеокарт для особливих потреб).

![Shell01](./images/Shell01.png)

Нижній рівень - це апаратні пристрої, керовані ядром Linux. Коли люди віддалено підключаються до сервера через SSH і вводять різні команди, ядро Linux не розпізнає ці слова чи букви. Як відомо, комп’ютери можуть розпізнавати машинні мови, такі як 0 і 1. Щоб завершити перетворення людської та машинної мови, в операційну систему, тобто Shell, було введено агента двостороннього перекладу, подібного до реального.

Це працює так:

**Люди з країни A** <<--->> **Shell** <<--->> **Люди з країни B**

З точки зору користувача, Shell — це інтерфейс взаємодії між людиною та комп’ютером, а інтерфейси взаємодії сучасних операційних систем в основному включають:

- Інтерфейс взаємодії командного рядка. Наприклад, такі операційні системи, як **RockyLinux** і **Debian**, виконують роль сервера.
- Графічний інтерактивний інтерфейс. Наприклад, операційна система **Windows 11** для дому та офісу.
- Командний рядок і змішаний графічний інтерактивний інтерфейс. Наприклад, **mint**, **Ubuntu** з графічним середовищем, **Windows Server** з Powershell тощо.

Класифікація Shell:

- Bourne Shell - Це сімейство включає, але не обмежується:
  - sh (Bourne Shell, /usr/bin/sh). Він був розроблений у Bell LABS у 1977 році Стівеном Борном і використовувався у V7 UNIX
  - ksh (Korn Shell, /usr/bin/ksh)
  - Bash (GNU Bourne-Again Shell, /bin/bash) - Народжений у 1987 році, він є продуктом проекту GNU. Більшість операційних систем GNU/Linux використовують bash як оболонку за замовчуванням
  - psh (POSIX Shell)
  - zsh (Z-shell)
- C Shell - Це сімейство включає, але не обмежується:
  - csh
  - tcsh
- Power Shell