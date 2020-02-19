# Se inicia con la descarga de la imagen node con el tag 10, se descarga de Docker Hub
FROM node:10

# Se establece el directorio donde se ejecutará todos los comandos
WORKDIR /usr/src/app

# Se copia los archivos package JSON al directorio /usr/src/app
COPY package*.json ./

# Se procede con la instalación de las dependencias
RUN npm install

# Se copia el resto de los archivos locales al contenedor, excepto node_modules (ver .dockerignore)
COPY . .

# Dentro del contenedor se ejecuta el comando "npm start" para iniciar el servidor de node
CMD [ "npm", "start" ]
