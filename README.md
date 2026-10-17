# J5 Prime Lag OS — Lagsung Labs

**Целевой адрес после переименования репозитория:** https://validityvalues.github.io/

**Превью текущей версии:** [Открыть сайт через CDN](https://raw.githack.com/ValidityValues/j5primelagweb/main/index.html)

**Исходный код:** [GitHub repository](https://github.com/ValidityValues/j5primelagweb)

## Что внутри

- Интерактивный виртуальный Samsung J5 Prime с приложениями: телефон, сообщения, камера, галерея, браузер, YouTube-пародия, музыка, файлы, настройки, магазин, терминал, доска объявлений и Касперский.
- Каждое приложение ждёт **20 секунд**, затем на короткое время открывается и вызывает стилизованный **Linux Kernel Panic / TTY1**.
- Касперский бегает по экрану, показывает абсурдные предупреждения и отказывается нормально закрываться.
- Системная реклама на рабочем столе и дополнительные всплывающие рекламные окна.
- Случайный видео-клип поверх телефона каждые **20 секунд** из `videos/playlist.json`; плеер выставляет громкость на **50%**. Современные браузеры могут потребовать одно нажатие для разрешения автоматического воспроизведения со звуком.
- Адаптивная верстка без npm и сторонних библиотек для основного сайта.

## Настроить постоянный адрес `validityvalues.github.io`

GitHub требует, чтобы user-site репозиторий назывался точно `validityvalues.github.io`. В текущем проекте workflow публикации уже лежит в `.github/workflows/pages.yml`.

1. Открой [Settings → General текущего репозитория](https://github.com/ValidityValues/j5primelagweb/settings) и переименуй **Repository name** в `validityvalues.github.io`.
2. Открой [Settings → Pages](https://github.com/ValidityValues/validityvalues.github.io/settings/pages) и выбери **Source → GitHub Actions**.
3. На вкладке [Actions](https://github.com/ValidityValues/validityvalues.github.io/actions) проверь запуск workflow **Deploy J5 Prime Lag Edition**.

После успешной публикации адрес будет `https://validityvalues.github.io/`. Репозиторий нужно переименовать под владельцем `ValidityValues`; одного изменения файлов или имени ветки недостаточно.

## Добавить собственные видео

Положи `.mp4` или `.webm` в папку `videos/` и укажи их имена в `videos/playlist.json`. GitHub Pages статический и не умеет автоматически перечислять файлы каталога.
