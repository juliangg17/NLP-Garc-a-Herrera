Proyecto de Procesamiento de Lenguaje Natural (NLP) - Análisis de Datos Multimodales
Este proyecto implementa técnicas de procesamiento de lenguaje natural (NLP) para analizar datos de diferentes medios (juegos, películas y libros), utilizando Python y bibliotecas avanzadas de NLP. El objetivo es procesar y preparar estos datos para análisis y tareas de clasificación, con la aplicación de técnicas de similitud y modelos de embeddings.

Contenido
Librerías:

Instalación y carga de bibliotecas esenciales para el análisis de texto y procesamiento de datos.
Carga y Procesamiento de Datos:

Juegos: Carga y transformación de datos de juegos desde un archivo CSV, incluyendo la generación de características como allow_kids y Class.
Películas: Carga y transformación de datos de películas desde un archivo CSV, combinando columnas y generando características.
Libros: Uso de web scraping para obtener datos de libros, seguido de procesamiento de los datos en un formato similar.
Modelos de Embeddings y Clasificación:

Aplicación de modelos de embeddings preentrenados (sentence-transformers, BERT) para la creación de vectores semánticos.
Implementación de un modelo de regresión logística para clasificación, con evaluación usando métricas de clasificación.
Técnicas de Similitud:

Cálculo de similitud de coseno entre embeddings para evaluar similitudes textuales.
Requisitos
Este proyecto requiere Python 3.x y las siguientes bibliotecas de Python. Puedes instalarlas usando pip:

bash
Copiar código
pip install pandas numpy scikit-learn torch transformers sentence-transformers spacy bs4 tqdm ipywidgets
Bibliotecas utilizadas:
pandas: Para manipulación y procesamiento de datos.
numpy: Para operaciones numéricas y manejo de matrices.
collections (Counter): Para el conteo eficiente de elementos en estructuras de datos.
re: Expresiones regulares para el preprocesamiento de texto.
spacy: Para procesamiento de lenguaje natural, incluyendo tokenización y modelado básico.
sklearn.metrics.pairwise (cosine_similarity): Para el cálculo de similitudes entre vectores.
transformers: Para modelos de lenguaje preentrenados, como BERT y pipelines de NLP.
AutoTokenizer, AutoModel, BertTokenizer, BertForSequenceClassification, pipeline: Herramientas para trabajar con modelos de lenguaje.
torch: Framework de machine learning necesario para ejecutar modelos de transformers.
sentence-transformers: Para generar embeddings de oraciones, permitiendo evaluar la similitud semántica.
requests y BeautifulSoup: Para web scraping, extrayendo datos de páginas web.
tqdm: Para mostrar una barra de progreso durante la ejecución de bucles largos.
ipywidgets e IPython.display: Para crear y mostrar widgets interactivos en notebooks.
Ejecución
Clonar el Repositorio
Clona el repositorio para acceder a los datos y archivos necesarios:

bash
Copiar código
git clone https://github.com/juliangg17/NLP-TUIA-Garcia-Herrera.git
cd NLP-TUIA-Garcia-Herrera
Instalar Dependencias Si aún no has instalado las bibliotecas necesarias, usa el siguiente comando:

bash
Copiar código
pip install -r requirements.txt
(Asegúrate de tener un archivo requirements.txt con las bibliotecas mencionadas, si decides gestionarlas con un archivo de este tipo).

Ejecutar el Notebook Abre y ejecuta el notebook en un entorno de Jupyter Notebook o JupyterLab, siguiendo el flujo de cada celda de código para cargar, procesar y analizar los datos.

Notas
Este proyecto utiliza modelos de lenguaje preentrenados y técnicas de NLP avanzadas. Se recomienda ejecutar el notebook en una máquina con GPU para procesar los modelos más rápido, especialmente al trabajar con sentence-transformers y BERT.
