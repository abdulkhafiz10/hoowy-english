# FluentPath — AI English Tutor

Самостоятельный локальный сервер школьной платформы: Grammar, Vocabulary, Writing, Speaking, AI Tutor и Progress.

## Запуск

В PowerShell:

```powershell
cd "C:\Abeke\проекты\English Ai Tutor\оффиц"
npm install
npm start
```

Откройте `http://127.0.0.1:3001`.

## AI-функции

Grammar и Vocabulary работают без ключа. Для AI Tutor, проверки Writing и Speaking создайте файл `.env` рядом с `server.js` по образцу `.env.example` и укажите свой `OPENAI_API_KEY` или TokenWave-ключ. После изменения `.env` перезапустите сервер.

## GitHub Pages

После включения Pages в настройках репозитория сайт публикуется автоматически из папки `web/` через GitHub Actions. Pages поддерживает только статические файлы: там работают интерфейс, локальные упражнения и сохранение прогресса в текущем браузере. Для AI Tutor, распознавания файлов и серверного профиля нужен отдельный Node.js сервер.

## Файлы

- `web/` — доступный в браузере интерфейс.
- `data/` — закрытый локальный прогресс; не публикуется веб-сервером.
