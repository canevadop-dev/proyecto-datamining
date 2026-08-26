# proyecto-datamining
# Análisis e Integración de Datos: Deserción y Trayectoria Educativa en el Perú (2023–2024)

## Descripción del Proyecto
Este proyecto integra cuatro fuentes públicas oficiales del Ministerio de Educación del Perú (MINEDU) para analizar la deserción escolar a nivel distrital y evaluar su agravamiento durante la transición de Educación Primaria a Educación Secundaria en el periodo 2023–2024.

El flujo realiza una integración multinivel en cascada:
1. **Nivel Escuela:** Empareja la matrícula y trayectoria 2023 con el catálogo del Padrón de IIEE para obtener la localización distrital (UBIGEO).
2. **Nivel Distrito:** Agrega los indicadores de matrícula y los cruza con los registros oficiales de deserción de cohorte (Primaria y Secundaria).

---

## Fuentes de Datos
Los datos provienen de repositorios públicos oficiales del Ministerio de Educación del Perú (MINEDU) y la Plataforma Nacional de Datos Abiertos:

* **Padrón de Instituciones Educativas (Censo Escolar):** [ESCALE - MINEDU](https://escale.minedu.gob.pe/censo-escolar/-/document_library_display/oJ44/view/8520583/65449?_110_INSTANCE_oJ44_redirect=https%3A%2F%2Fescale.minedu.gob.pe%2Fcenso-escolar%2F-%2Fdocument_library_display%2FoJ44%2Fview%2F8520583)
* **Matriculación y Trayectoria Estudiantil (2021–2024):** [Datos Abiertos Gob.pe](https://www.datosabiertos.gob.pe/dataset/matriculaci%C3%B3n-y-trayectoria-estudiantil-2021-2024)
* **Tasa y Número de Desertores en Educación Primaria y Secundaria (2023–2024):** [Datos Abiertos Gob.pe](https://www.datosabiertos.gob.pe/dataset/tasa-y-n%C3%BAmero-de-desertores-eneducaci%C3%B3n-primaria-y-secundaria-20232024)

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
   git clone https://github.com/canevadop-dev/proyecto-datamining.git
cd proyecto-datamining
