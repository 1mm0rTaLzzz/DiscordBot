# Discord Music Bot

Этот бот позволяет воспроизводить аудио с YouTube в голосовых каналах Discord с использованием `yt-dlp` и `FFmpeg`.

## 📌 Функции
- Воспроизведение аудио с YouTube
- Подключение к голосовому каналу
- Отключение из голосового канала
- Использование `yt-dlp` и `FFmpeg` для потоковой передачи

---

## 🛠 Установка

### 1. Установите Python
Убедитесь, что у вас установлен Python **3.8 или выше**. Проверить версию можно командой:
```sh
python --version
```
Если Python не установлен, скачайте его с [официального сайта](https://www.python.org/downloads/).

### 2. Создайте виртуальное окружение (рекомендуется)
```sh
python -m venv venv
```
Активируйте виртуальное окружение:
- **Windows:**  
  ```sh
  venv\Scripts\activate
  ```
- **Linux/macOS:**  
  ```sh
  source venv/bin/activate
  ```

### 3. Установите зависимости
```sh
pip install -r requirements.txt
```

Если файла `requirements.txt` нет, установите зависимости вручную:
```sh
pip install discord.py yt-dlp pynacl ffmpeg dotenv
```

### 4. Установите FFmpeg
Бот использует `FFmpeg` для обработки аудио.
- **Windows:**
  1. Скачайте `ffmpeg` с [https://ffmpeg.org/download.html](https://ffmpeg.org/download.html)
  2. Распакуйте его в `C:\ffmpeg`
  3. Добавьте `C:\ffmpeg\bin` в переменную окружения `PATH`
  4. Проверьте установку:
     ```sh
     ffmpeg -version
     ```
- **Linux/macOS:**
  ```sh
  sudo apt install ffmpeg  # Для Debian/Ubuntu
  brew install ffmpeg  # Для macOS (Homebrew)
  ```

### 5. Создайте файл `.env`
Создайте `.env` файл и добавьте в него ваш **токен Discord-бота**:
```sh
DISCORD_TOKEN=ВАШ_ТОКЕН
```

---

## 🚀 Запуск бота

```sh
python bot.py
```

После запуска бот должен успешно подключаться к серверу и выполнять команды.

---

## 📜 Команды бота
- `!play <URL>` – Воспроизводит аудио с YouTube
- `!leave` – Отключает бота из голосового канала

---
