# Використовуємо базовий образ Python
FROM python:3.11.4


ENV APP_HOME /app

# Встановлюємо необхідні залежності
RUN pip install jinja2

# Створюємо робочий каталог для додатка
WORKDIR $APP_HOME

# Копіюємо всі файли додатка у контейнер
COPY . .

# Встановлюємо необхідні пакети для сервера
#RUN apt-get update && apt-get install -y \
#    vim

RUN pip install -r reguirements.txt


EXPOSE 3000

# Запускаємо додаток при старті контейнера
CMD ["python", "main.py"]