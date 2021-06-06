# Costo de Seguro Médico

Bienvenidos!

En este proyecto lo que hice fue usar el dataset "Medical Cost Personal", el cual pueden ver en https://www.kaggle.com/mirichoi0218/insurance, para crear modelos que permitan predecir el costo de seguro médico a cobrarle a una persona.

Todo el código, la explicación detallada y las conclusiones estan en la notebook de Colab. 

En resumen, lo que hice fue:

### Importar Dataset
Directamente de Kaggle usando la API propia de Kaggle. Para mas detalle ver https://www.kaggle.com/docs/api#getting-started-installation-&-authentication

### EDA
Exploratory Data Analysis o Análisis Exploratorio de Datos en donde hice:
- Una descripción del dataset propiamente dicho y de sus features
- Un análisis estadístico descriptivo
- Una revisión de valores nulos
- Histogramas de los atributos para ver su composición

### Pre-Procesado
Transformación de los datos para llevarlos a la estructura necesaria para alimentar los modelos. Consistió en:
- Llevar a valores numéricos las variables categóricas.
- Generar matriz de diseño X_df (dataset sin la variable objetivo) y matriz unicamente con la variable objetivo (y_df).
- Generar estructuras Numpy

### Anáisis Cuantitativo y Numérico de los Datos
En esta etapa realicé:
- Una matriz de correlación con mapa de calor para entender mejor la relación entre los atributos.
- Histogramas usando Scatter Matrix
- Una visualización llevando el dataset a dos dimensiones utilizando PCA

### Modelos de Aprendizaje
Antes de la creación de los modelos de aprendizaje en sí, realicé:
- Partición del dataset en Training, Validation y Test.
- Histograma para ver la distribución de cada partición (comprobar que estaban estratificadas)
- Normalización de los datos para llevarlos al intervalo [0,1] usando MinMaxScaler
Luego, con respecto a los modelos entrené:
- REGRESOR LINEAL PURO
- REGRESOR RIDGE
- REGRESOR LASSO
- REGRESOR RANDOM FOREST
A todos los modelos los evalué usando RMSE (root mean square error) 
