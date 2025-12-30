# TELECOMX_CHALLENGE_ALURALATAM
Analisis de datos de un Json para comprender los factores que llevan a la pérdida de clientes.

**Análisis de Evasión de Clientes (Churn) - TelecomX**

Este proyecto realiza un análisis exhaustivo de los factores que impulsan la evasión de clientes en una compañía de telecomunicaciones TELECOMX. Utilizando técnicas de ciencia de datos, identificamos perfiles de riesgo y cuantificamos el impacto económico de la pérdida de usuarios para proponer estrategias de retención efectivas.
Estructura del Proyecto: El análisis se divide en las siguientes etapas:
Limpieza de Datos: Tratamiento de valores nulos y estandarización de variables numéricas como charges.total.
Análisis Exploratorio (EDA): Identificación de patrones mediante visualizaciones (Boxplots, KDE Plots, Gráficos de Torta).
Impacto Económico: Cálculo del valor perdido mensual y del ticket promedio de los clientes en fuga.
Conclusiones Estratégicas: Recomendaciones basadas en hallazgos sobre tipos de contrato, servicios de internet y métodos de pago.

**Instalación y Dependencias**

Para ejecutar este proyecto localmente, asegúrate de tener instalado Python 3.x1. Se recomienda utilizar un entorno virtual.

**Dependencias Principales**

El proyecto utiliza las siguientes bibliotecas de Python:
-Pandas: Para la manipulación y limpieza de datos
-NumPy: Para operaciones numéricas
-Matplotlib y Seaborn: Para la generación de gráficos y visualizaciones

Puedes instalarlas ejecutando:

pip install pandas numpy matplotlib seaborn

**Cómo Ejecutar el Proyecto**

1. Clona este repositorio: git clone https://github.com/tu-usuario/nombre-del-repo.git
2. Asegúrate de que el archivo de datos esté en la ruta correcta definida en el notebook.
3. Abre el archivo principal del análisis (por ejemplo, TELECONCHALLENGE.ipynb) en Jupyter Notebook o Google Colab.
4. Ejecuta las celdas de forma secuencial.

**Origen de los Datos**

Los datos y notebooks base utilizados para este proyecto provienen de los recursos compartidos en: https://drive.google.com/drive/u/1/folders/1CeFHp4FxUUf3xliGz7-o1NWxt21nmndI especificamente el arcivo: TelecomX_Data.json

**Posibles Problemas y Soluciones**

Error en nombres de columnas: Verifica que las columnas coincidan con el formato (ej: charges.monthly vs charges.total).

Valores no numéricos en cargos: Se aplicó pd.to_numeric(errors='coerce') para manejar espacios en blanco o textos en columnas de moneda.

Error de visualización en Colab: Asegúrate de importar correctamente matplotlib.pyplot y seaborn al inicio del notebook

**Principales Hallazgos**

Pérdida Mensual: El impacto económico asciende a $139,130.85 mensuales.
Perfil Crítico: Los clientes con servicios de Fibra Óptica y contratos mes a mes representan el mayor riesgo de fuga.
Fricción de Pago: El método de Electronic Check presenta una tasa de abandono significativamente superior a los métodos automáticos.

Autor: Javier More
