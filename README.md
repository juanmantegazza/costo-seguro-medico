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
A todos los modelos los evalué usando RMSE (root mean square error). Usé el set de validación para tunear los hiperparámetros y quedarme con la mejor opción de cada modelo.
Finalmente, evalué a los modelos usando el set de test, los comparé y di mis conclusiones. 

Gracias por haber llegado hasta aca!

Saludos, Juan.


# Medical Insurance Cost

Welcome!

In this project, what I did was use the "Medical Cost Personal" dataset, which you can see at https://www.kaggle.com/mirichoi0218/insurance, to create models that allow predicting the cost of medical insurance to be charged to a person.

All the code, the detailed explanation and the conclusions are in the Colab notebook.

In short, what I did was:

### Import Dataset
Directly from Kaggle using Kaggle's own API. For more details see https://www.kaggle.com/docs/api#getting-started-installation-&-authentication

### EDA
Exploratory Data Analysis or Exploratory Data Analysis where I did:
- A description of the dataset itself and its features
- A descriptive statistical analysis
- A review of null values
- Histograms of the attributes to see their composition

### Pre-Processing
Transformation of the data to bring them to the necessary structure to feed the models. It consisted of:
- Convert categorical variables to numerical values.
- Generate design matrix X_df (dataset without the target variable) and matrix with only the target variable (y_df).
- Generate Numpy Structures

### Quantitative and Numerical Data Analysis
At this stage I did:
- A heat map correlation matrix to better understand the relationship between attributes.
- Histograms using Scatter Matrix
- A visualization taking the dataset to two dimensions using PCA

### Learning Models
Before the creation of the learning models themselves, I performed:
- Partition of the dataset in Training, Validation and Test.
- Histogram to see the distribution of each partition (check that they were stratified)
- Normalization of the data to bring them to the interval [0,1] using MinMaxScaler.
Then, with respect to the models I trained:
- PURE LINEAR REGRESSOR
- RIDGE REGRESSOR
- LASSO REGRESSOR
- RANDOM FOREST REGRESSOR 
I evaluated all the models using RMSE (root mean square error). I used the validation set to tune the hyperparameters and get the best option from each model. Finally, I evaluated the models using the test set, compared them and gave my conclusions.
Thank you for coming this far!

Greetings, John.
