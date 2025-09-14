## Instrucciones adicionales:
1. Crear archivo de configuracion `.env` en la raíz con la siguiente estructura:
  MYSQL_ROOT_PASSWORD=supersecret

  MYSQL_DATABASE=app_db

  MYSQL_USER=app_user

  MYSQL_PASSWORD=app_pass

  DB_HOST=db

  DB_PORT=3306

  DB_USER=app_user

  DB_PASSWORD=app_pass

  DB_NAME=app_db

  DATABASE_URL=mysql://app_user:app_pass@db:3306/app_db

  POSTGRES_HOST=db

  POSTGRES_PORT=3306

  POSTGRES_DB=app_db

  POSTGRES_USER=app_user
  
  POSTGRES_PASSWORD=app_pass

 ** Considerar que se agregan variables postgres, debido a que el codigo de la app insistia en ir a buscar este tipo de variables (prefijo postgres) y como la instruccion era no modificar codigo, se agregó ese tipo de variables, pero con las mismas credenciales de mysql.

2. Levantar los servicios utilizando el comando "docker compose up"