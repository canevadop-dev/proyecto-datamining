# proyecto-datamining
# Análisis e Integración de Datos: Deserción y Trayectoria Educativa en el Perú (2023–2024)

## Descripción del Proyecto
Este proyecto integra cuatro fuentes públicas oficiales del Ministerio de Educación del Perú (MINEDU) para analizar la deserción escolar a nivel distrital y evaluar su agravamiento durante la transición de Educación Primaria a Educación Secundaria en el periodo 2023–2024.

El flujo realiza una integración multinivel en cascada:
1. **Nivel Escuela:** Empareja la matrícula y trayectoria 2023 con el catálogo del Padrón de IIEE para obtener la localización distrital (UBIGEO).
2. **Nivel Distrito:** Agrega los indicadores de matrícula y los cruza con los registros oficiales de deserción de cohorte (Primaria y Secundaria).

---

## Fuentes de Datos
Debido al límite de tamaño de archivos en GitHub (>25 MB), los datasets completos se encuentran alojados en el siguiente enlace de acceso público:

🔗 **[Descargar datasets completos desde Google Drive](https://drive.google.com/drive/folders/1jkxgIUl6A-DmUvLk2mRkgOxk4cTCXd9x?usp=sharing)**

### Detalle de archivos:
* `Padron.dbf`: Catálogo oficial de IIEE (descargar desde el enlace de Drive).
* `Matriculación y Trayectoria Estudiantil 2023.csv`: Microdatos de matrícula (descargar desde el enlace de Drive).
* `Tasa y número de desertores en Educación Primaria 2023-2024.csv`: Incluido en este repositorio.
* `Tasa y número de desertores en Educación Secundaria 2023-2024.csv`: Incluido en este repositorio.

## Instrucciones de Ejecución

### Opción 1: Ejecutar en Google Colab
1. Subir el archivo `notebooks/Primera_entrega_nueva_fuente.ipynb` a Google Colab.
2. Cargar los 4 archivos de datos en el entorno `/content/`.
3. Ejecutar las celdas en orden secuencial (`Entorno de ejecución` > `Ejecutar todo`).

### Opción 2: Ejecutar en Local / Jupyter Notebook
1. Clonar el repositorio:
   ```bash
   git clone [https://github.com/TU_USUARIO/TU_REPOSITORIO.git](https://github.com/TU_USUARIO/TU_REPOSITORIO.git)
   cd TU_REPOSITORIO
