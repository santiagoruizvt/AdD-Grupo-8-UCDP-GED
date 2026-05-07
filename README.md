# AdD-Grupo-8-UCDP-GED

Este repositorio reúne el análisis del dataset "Eventos de violencia organizada (UCDP GED)" para el trabajo del grupo de la asignatura de Análisis de Datos.

## Descripción

El dataset UCDP GED documenta eventos de violencia organizada en el mundo, incluyendo detalles temporales, geográficos y del tipo de conflicto. Este proyecto busca explorar patrones de violencia, tendencias temporales, distribución geográfica y posibles indicadores predictivos.

## Objetivos sugeridos

- Exploración y limpieza de datos
- Análisis descriptivo de tipos de evento y actores involucrados
- Visualización de series temporales de violencia
- Mapas geoespaciales y análisis regional
- Agrupamiento de eventos y detección de hotspots
- Preparación de modelos básicos de clasificación o regresión para analizar factores asociados a la violencia organizada

## Estructura del repositorio

- `dataset/` - datos originales del proyecto
- `README.md` - guía del repositorio
- `pyproject.toml` - dependencias y configuración de Python

## Configuración del entorno con `uv`

`uv` es una herramienta de gestión de entornos para Python que crea y sincroniza un entorno virtual basado en el archivo `pyproject.toml`.

1. Asegúrate de tener Python 3.11 o 3.12 instalado.
2. Actualiza pip:

Windows (PowerShell o CMD):

```powershell
python -m pip install --upgrade pip
```

Linux:

```bash
python3 -m pip install --upgrade pip
```

3. Instala `uv`:

Windows:

```powershell
python -m pip install uv
```

Linux:

```bash
python3 -m pip install uv
```

4. Valida que `uv` esté instalado correctamente:

```bash
uv --version
```

5. Sincroniza y crea el entorno con `uv sync` antes de instalar dependencias:

```bash
uv sync
```

6. Instala las dependencias definidas en `pyproject.toml`:

```bash
uv install
```

7. Activa el entorno:

- PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

- CMD:

```cmd
.\.venv\Scripts\activate.bat
```

- Linux / macOS:

```bash
source .venv/bin/activate
```

> Si `uv install` no funciona, puedes instalar las dependencias manualmente con `python -m pip install -r requirements.txt` si generas un `requirements.txt` o usando `pip` directamente.

## Cómo trabajar con el dataset

1. Carga los datos desde `dataset/GEDEvent_v25_1.csv`.
2. Revisa tipos de variables, valores nulos y registros duplicados.
3. Realiza análisis exploratorio con Pandas, visualizaciones con Matplotlib y Seaborn, y perfiles de datos con ydata-profiling.
4. Genera gráficos que muestren:
   - frecuencia de eventos por año y país
   - distribución de tipos de violencia organizada
   - evolución temporal de los principales actores
   - mapas o análisis geoespaciales básicos
5. Documenta hallazgos en notebooks, informes o presentaciones.

## Buenas prácticas

- No incluyas archivos de entorno virtual en el control de versiones.
- Mantén los datos originales sin modificar y trabaja sobre copias filtradas o derivadas.
- Usa notebooks claros con secciones bien identificadas.
- Guarda resultados y visualizaciones en carpetas de salida específicas si son parte del análisis.
