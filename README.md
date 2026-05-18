# VideoDigest

Сервис для автоматической обработки видео:
- загрузка видеофайла через веб-интерфейс;
- постановка задачи в очередь;
- транскрибация речи через `faster-whisper`;
- extractive summary без внешних LLM API;
- выделение ключевых фрагментов по таймкодам;
- просмотр результата и файлов обработки в браузере.

## Стек

- FastAPI
- Redis + RQ
- faster-whisper
- ffmpeg
- SQLite
- Jinja2 templates + простой CSS/JS
- Docker + Docker Compose

## Запуск

```bash
docker compose up --build
```

После старта сервис доступен по адресам:
- `http://localhost:8000`
- `http://localhost:8000/dashboard`
- `http://localhost:8000/docs`

Видеозапись функций приложения:
https://rutube.ru/video/private/ecb5c8bed4d5f722443a1daef838ad8c/?p=8FTURPX6EusO1L95jIUZMA
