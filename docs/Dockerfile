# Используем Node.js 14 в качестве базового образа
FROM node:14

# Устанавливаем gitbook-cli глобально
RUN npm install -g gitbook-cli

# Создаем рабочую директорию
WORKDIR /gitbook

# Копируем все файлы из текущей директории в контейнер
COPY . /gitbook

# Устанавливаем зависимости и инициализируем GitBook
RUN gitbook init

# Команда по умолчанию для запуска GitBook сервера
CMD ["gitbook", "serve"]