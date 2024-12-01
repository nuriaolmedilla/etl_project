# Proyecto ETL: Master en Ciencia de Datos

## Descripción
Este proyecto implementa un proceso ETL completo (Extracción, Transformación y Carga) para integrar datos de plataformas de redes sociales, como Threads e Instagram.

## Instrucciones de uso
### Requisitos
- Docker y Docker Compose instalados.
- Python 3.9 (si no se utiliza Docker).

### Configuración
1. Clonar el repositorio:
   ```
   git clone https://github.com/nuriaolmedilla/etl_project.git
   cd etl_project
   ```
2. Construir el contenedor Docker:
   ```
   docker-compose up --build
   ```
3. Ejecutar el proceso ETL:
   ```
   docker exec -it etl_container python run_etl.py
   ```

## Estructura del proyecto
El repositorio contiene:
- **/scripts**: Código SQL para las fases ETL.
- **Dockerfile** y **docker-compose.yml**: Archivos para contenedorización.
- **README.md**: Este archivo.

## Licencia
MIT License

## Data Lakehouse: Es la mejor opción, ya que los datos tienen una mezcla de estructura:
•	Datos estructurados (dim_account.csv y fact_social_metrics.csv).
•	Datos parcialmente estructurados con formatos inconsistentes (THREADS.csv, INSTAGRAM.csv).
