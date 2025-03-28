📌 Flujo de Autenticación
Los usuarios pueden registrarse o iniciar sesión a través de los formularios correspondientes.

Los datos ingresados en los formularios se validan utilizando esquemas de Zod.

Si la autenticación es exitosa:

El servidor genera un token JWT.

El token se almacena en una cookie HTTP-only para mayor seguridad.

Los datos del usuario se guardan en el contexto de autenticación.

Las rutas protegidas verifican el estado de autenticación antes de permitir el acceso.

Al cargar la aplicación, el token se verifica automáticamente.

Los usuarios pueden actualizar su perfil o cerrar sesión en cualquier momento.

🛠️ Tecnologías Utilizadas
JWT (JSON Web Tokens) → Autenticación sin estado.

Cookies HTTP-only → Almacenamiento seguro del token.

Zod → Validación de datos en formularios.

React Context → Gestión del estado global de autenticación.

React Router → Protección de rutas y control de acceso.


### MERN Stack CRUD with JWT

This is a web application project using React, with a Nodejs Backend using Express and Mongodb as Database (MERN Stack)

### Installation with docker-compose (Recommended)

```sh
docker-compose up -d
npm run dev
```

### Deployment

```sh
git clone 
cd mern-tasks-auth
npm i
npm run build
npm start
```

> You need to have a Mongodb database running