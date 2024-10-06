# Используем официальный образ Python
FROM python:3.9-slim

## Устанавливаем рабочую директорию
#WORKDIR /app
COPY openweather.py .
# Копируем файл с зависимостями в контейнер
COPY ../requirements.txt .
# Устанавливаем зависимости
RUN pip install --no-cache-dir -r requirements.txt
# Выполняем команду для запуска Python-файла

CMD ["python", "openweather.py"]

#  docker build -t sep_23 . #obraz

#  docker run --rm sep_23   # run

#  ssh -i C:\Users\PC\.ssh\id_ed25519 vlad@164.92.136.89

