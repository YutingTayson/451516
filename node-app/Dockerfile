# Используем базовый образ Node.js
FROM node:latest

# Устанавливаем рабочую директорию внутри контейнера
WORKDIR /app

# Копируем package.json и package-lock.json в контейнер
COPY package*.json ./

# Устанавливаем зависимости
RUN npm install

# Копируем все файлы из локальной директории в контейнер
COPY . .

# Определяем команду для запуска приложения
CMD ["npm", "start"]

