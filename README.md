# Análisis Bibliográfico Automatizado con Python
Este repositorio contiene las herramientas necesarias para realizar un análisis bibliográfico (cienciometría/bibliometría) utilizando datos exportados de Scopus. El flujo de trabajo permite procesar grandes volúmenes de metadatos académicos para identificar tendencias, autores clave y redes de colaboración.

## Requisitos Previos
Antes de ejecutar el análisis, asegúrate de contar con lo siguiente:

1. Obtención de Datos (Scopus)
Es necesario haber descargado previamente la base de datos bibliográfica:

Realiza tu búsqueda en Scopus.

Selecciona los documentos de interés.

Haz clic en Export.

Elige el formato CSV (se recomienda CSV para facilitar la manipulación con Pandas).

Asegúrate de incluir todos los campos: Información de cita, Resumen, Palabras clave y Detalles de bibliografía.

2. Entorno de Desarrollo
Puedes trabajar en cualquiera de los siguientes entornos:

Jupyter Notebook: Ideal para un análisis exploratorio visual paso a paso.

Visual Studio Code: Recomendado si prefieres un entorno de desarrollo integrado con la extensión de Jupyter instalada.

## Instrucciones de Configuración
Sigue estos pasos para poner en marcha el proyecto:

1. Clonar el Repositorio
Bash
git clone https://github.com/tu-usuario/nombre-del-repo.git
cd nombre-del-repo
2. Instalación de Dependencias
Asegúrate de tener Python instalado y ejecuta:

Bash
pip install pandas numpy matplotlib seaborn wordcloud
(Opcional) Si vas a realizar análisis de redes:

Bash
pip install networkx pyvis
3. Ejecución del Análisis
Coloca tu archivo descargado de Scopus (ej. scopus.csv) en la carpeta data/.

Abre tu entorno (VS Code o Jupyter).

Inicia el archivo analisis_bibliografico.ipynb.

Cambia la ruta del archivo en la celda de carga de datos:

Python
df = pd.read_csv('data/scopus.csv')
