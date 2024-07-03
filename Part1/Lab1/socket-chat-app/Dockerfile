# Usa una imagen base de Node.js
FROM node:14

# Establece el directorio de trabajo en /app
WORKDIR /app

# Copia package.json y package-lock.json
COPY package*.json ./

# Instala las dependencias
RUN npm install

# Copia el resto del código de la aplicación
COPY . .

# Exponer el puerto que usa la aplicación (ajusta si tu aplicación usa otro puerto)
EXPOSE 3000

# Comando para ejecutar la aplicación
CMD ["node", "index.js"]
