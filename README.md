<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

#Ejecutar en desarrollo

1. Clonar el repositorio
2. Ejecutar

```
yarn install
```

3. Tener Nest CLI instalado

```
npm i -g @nestjs/cli
```

4. levantar la base de datos

```
docker-compose up -d
```

5. Clonar el archivo **.env.template** y renombrar a **.env**

6. Llenar las variables de entorno definidas **.env**

7. Ejecutar el proyecto en modo desarrollo con el comando:

```
yarn start:dev
```

8. Poblar la base de datos con la semilla

```
http://localhost:3000/api/v2/seed
```

## Stack usado

- MongoDB
- Nest

# Production Build


1. Crear el archivo __.env.prod__
2. llenar las variables de entorno de producción 
3. Crear la nueva imagen 

```
docker-compose -f docker-compose.prod.yaml --env-file .env.prod up --build
```

