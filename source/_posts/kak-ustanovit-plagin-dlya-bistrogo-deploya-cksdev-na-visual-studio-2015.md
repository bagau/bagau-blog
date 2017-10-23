---
title: Как установить плагин для быстрого деплоя cksdev на Visual studio 2015
categories:
  - Кодинг
date: 2016-07-27 09:58:21
---

Здравствуйте, читатели.

Быстрый деплой в Visual studio нужен для того, чтобы делать быстрый деплой, так как когда правишь стили или яваскрипты не обязательно делать полный деплой.

<!-- more -->

Как поставить плагин cksdev на Visual studio 2015?

1.  Скачать на сайте https://cksdev.codeplex.com/ версию для 2013
2.  Скачать отттуда .vsix файл
3.  Переименовать ее в .cab
4.  Открываем архиватором, например 7-Zip
5.  Правим файл внутри архива: extension.vsixmanifest
6.  Там в этих строках меняем 13.0 на 15.0:
    *   &lt;InstallationTarget Version=»[12.0,13.0)» Id=»Microsoft.VisualStudio.Pro» /&gt;
    *   &lt;InstallationTarget Version=»[12.0,13.0)» Id=»Microsoft.VisualStudio.Ultimate» /&gt;
    *   &lt;InstallationTarget Version=»[12.0,13.0)» Id=»Microsoft.VisualStudio.Premium» /&gt;
7.  Сохраняем файл в архив
8.  Меняем расширение снова в .vsix
9.  Двойным кликом открываем файл и устанавливаем

На этом все, быстрый деплой работает комбинацией клавиш Alt+C,C.

Благодарю за внимание.