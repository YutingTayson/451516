# Используем базовый образ Node.js
FROM node:latest

# Устанавливаем рабочую директорию внутри контейнера
WORKDIR /app

# Копируем файлы из локальной директории в контейнер
COPY node-app/package.json .
COPY node-app/index.js .

# Устанавливаем зависимости Node.js
RUN npm install

# Запускаем приложение при запуске контейнера
CMD ["node", "index.js"]
