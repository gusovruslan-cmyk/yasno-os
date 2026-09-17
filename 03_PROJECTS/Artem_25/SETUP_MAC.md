# Подключение проекта на Mac

## 1. Распаковать

Распаковать архив. Переместить папку `Artem_25` в:

`/Users/ruslangusov/Downloads/YASNO_OS/Projects/`

После этого проект появится в Obsidian.

## 2. Включить Git LFS

Открыть Terminal и выполнить:

```bash
cd /Users/ruslangusov/Downloads/YASNO_OS
git lfs install
git lfs track "Projects/Artem_25/**/*.png"
git lfs track "Projects/Artem_25/**/*.jpg"
git lfs track "Projects/Artem_25/**/*.jpeg"
git lfs track "Projects/Artem_25/**/*.mov"
git lfs track "Projects/Artem_25/**/*.MOV"
git lfs track "Projects/Artem_25/**/*.mp4"
git lfs track "Projects/Artem_25/**/*.MP4"
```

## 3. Сохранить в GitHub

1. Открыть GitHub Desktop.
2. Выбрать репозиторий `gusovruslan-cmyk/yasno-os`.
3. Проверить список новых файлов.
4. Commit summary: `Добавлен проект Артём 25`.
5. Нажать `Commit to main`.
6. Нажать `Push origin`.

Первый Push может идти дольше обычного, потому что загружаются изображения и видео.

## 4. Как работать дальше

- Перед началом работы в GitHub Desktop нажимать `Fetch origin`, затем при наличии изменений `Pull origin`.
- После новых кадров делать Commit и Push.
- Утверждённые кадры класть только в `Master_Frames`.
- Неудачные и промежуточные версии переносить в `Archive`, а не удалять сразу.
- После утверждения нового кадра обновлять `02_Реестр_кадров.md`.

## Важное ограничение

Codex получит устойчивый доступ только тогда, когда репозиторий `yasno-os` будет подключён к рабочей среде текущей задачи. Простого хранения файлов на Mac недостаточно: локальные изменения должны быть отправлены на GitHub через Push.
