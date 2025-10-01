🐳 Cómo crear Imágenes y Contenedores en Docker

para levantar un proyecto con Docker usando dos opciones: comandos manuales o docker-compose.yml

Usando Comandos Manuales

1️⃣ Crear la red
docker network create rednodejs

2️⃣ Crear la imagen
docker build -t nodejs:1 .

3️⃣ Crear el contenedor con puerto y red
docker create -p3000:3000 --name nodejs --network rednodejs nodejs:1

Usando docker-compose.yml

Levantar el contenedor
docker compose up

Detener y borrar el contenedor
docker compose down
