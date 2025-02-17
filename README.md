
# Pasos para levantar Apache Airflow con Docker

### 1. Levantar los contenedores
En la carpeta donde se encuentran los archivos `docker-compose.yaml` y `.env`, ejecuta:

```bash
docker-compose up
```

### 2. Crear el usuario admin
Después de que los contenedores estén en funcionamiento, ejecuta el siguiente comando para crear el usuario administrador:

```bash
docker-compose run airflow-worker airflow users create   --role Admin   --username admin   --email admin   --firstname admin   --lastname admin   --password admin
```

### 3. Acceder a la interfaz web
Abre tu navegador y ve a `http://localhost:8080`. Inicia sesión con las siguientes credenciales:

- **Usuario:** admin
- **Contraseña:** admin
