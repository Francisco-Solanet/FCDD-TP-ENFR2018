# Análisis exploratorio de datos – ENFR 2018

Trabajo práctico de **Fundamentos de Ciencia de Datos**.

Este proyecto consiste en un análisis exploratorio de datos (EDA) sobre la **Encuesta Nacional de Factores de Riesgo (ENFR 2018)**. Se utilizan herramientas de Python para explorar variables sociodemográficas, estudiar valores faltantes, realizar visualizaciones y analizar hipótesis relacionadas con los ingresos, los hábitos y el estado de salud de la población argentina.

## 1. Estructura del proyecto

```text
FCDD-TP-ENFR2018/
│
├── README.md
├── requirements.txt
├── .gitignore
│
│
├── src/
│   └── TPE_FCDD.ipynb
│
├── data/
│   ├── raw/
│   │   └── ENFR2018_baseusuario.zip
│
└── informe/
    ├── TPE_FUNDAMENTOS.docx
    
```

**Descripción de las carpetas:**

- `src/`: contiene los archivos Python desarrollados en Visual Studio Code.
- `data/raw/`: contiene el conjunto de datos original.
- `informe/`: contiene el informe final del trabajo práctico.

## 2. Requisitos previos

Para ejecutar el proyecto se necesita:

- Python 3 instalado.
- pip, el gestor de paquetes de Python.
- Jupyter Notebook o JupyterLab, o Visual Studio Code con soporte para notebooks.
- Los archivos del proyecto, incluyendo el conjunto de datos original.

El archivo `ENFR2018_baseusuario.zip` debe estar ubicado en `data/raw/`. El notebook utiliza una ruta relativa para localizarlo.

## 3. Instalación del entorno

Se recomienda utilizar un entorno virtual para instalar las dependencias sin modificar otros proyectos de Python.

Abrir una terminal en la carpeta raíz del proyecto y ejecutar:

### Windows

Crear el entorno virtual:

```powershell
python -m venv .venv
```

Activarlo:

```powershell
.\.venv\Scripts\Activate.ps1
```

### Linux / macOS

Crear el entorno virtual:

```bash
python3 -m venv .venv
```

Activarlo:

```bash
source .venv/bin/activate
```

Una vez activado el entorno, actualizar pip:

```bash
python -m pip install --upgrade pip
```

Instalar las dependencias del proyecto:

```bash
python -m pip install -r requirements.txt
```

## 4. Dependencias utilizadas

Las principales bibliotecas utilizadas en el proyecto son:

| Biblioteca | Uso |
|---|---|
| Pandas | Lectura, manipulación y análisis de datos. |
| NumPy | Operaciones y cálculos numéricos. |
| Matplotlib | Generación de gráficos. |
| Seaborn | Visualizaciones estadísticas. |
| Scikit-learn | Preprocesamiento, estandarización e imputación de datos. |
| Yellowbrick | Visualización de técnicas de análisis, como PCA. |

Las versiones de las dependencias se encuentran especificadas en `requirements.txt`.

## 5. Ejecución del proyecto

### Opción A: Jupyter Notebook

Con el entorno virtual activado, ejecutar:

```bash
jupyter notebook
```

También se puede utilizar JupyterLab:

```bash
jupyter lab
```


### Visual Studio Code

1. Abrir la carpeta raíz del proyecto en Visual Studio Code.
2. Abrir el archivo `.ipynb` ubicado en `notebooks/`.
3. Seleccionar el intérprete de Python correspondiente al entorno virtual `.venv`.
4. Seleccionar el kernel correspondiente.
5. Ejecutar las celdas en orden.

**Importante:** se recomienda ejecutar las celdas secuencialmente, ya que algunas utilizan variables y resultados generados en celdas anteriores.

## 6. Datos utilizados

El proyecto utiliza la base de datos usuario de la **Encuesta Nacional de Factores de Riesgo 2018**, publicada por el Instituto Nacional de Estadística y Censos (INDEC).

El archivo original se encuentra comprimido en:

```text
data/raw/ENFR2018_baseusuario.zip
```

El notebook contempla la descompresión del archivo para acceder a los datos utilizados durante el análisis.

## 7. Tecnologías utilizadas

- Python
- Jupyter Notebook
- Visual Studio Code
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Yellowbrick

## 8. Informe final

El informe académico contiene el desarrollo del análisis exploratorio, las dimensiones estudiadas, las hipótesis planteadas, las visualizaciones y las conclusiones obtenidas.

Se encuentra disponible en la carpeta `informe/`.
