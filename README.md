# Proyecto-IMT-2200
En este proyecto utilizaremos datos, provenientes de un DataSet de Kaggle en formato CSV, sobre 800 futbolistas universitarios activos en sus respectivas ligas. Elegimos trabajar con esta temática por la afinidad existente en el grupo con el deporte, especialmente fútbol, además del interés por la parte científica detrás del entrenamiento y cómo podemos entregar una recomendación para evitar lesiones. Por esto, el proyecto estará destinado a los equipos deportivos para así puedan evaluar sus métodos de entrenamiento y renovarlos de ser necesario. También para que los futbolistas tengan la posibilidad de rendir lo mejor posible. La razón detrás de este trabajo surge por el aumento de lesiones en el fútbol actual, sin la posibilidad de continuar por un tiempo la temporada, por esto decidimos este proyecto para entender mejor las causas de las lesiones.
Para la realización del proyecto usamos como guía la pregunta “¿Es posible predecir el riesgo de lesiones en deportistas según sus rasgos físicos y rutinas?”. Con ella, buscamos ayudar a los deportistas y equipos deportivos dando a conocer las principales causas de lesiones y cómo prevenirlas. Cumpliendo con este objetivo, esperamos una mejora en el deporte disminuyendo la cantidad de lesiones gracias al análisis de estos datos y los jugadores logren una condición más favorable. Por esto, la audiencia objetivo del proyecto son aquellos que buscan iniciar como deportistas, quienes ya practican el deporte y renovar su rutina, y el equipo deportivo para mantener a sus jugadores en buen estado

Derivado a la pregunta guía, decidimos avanzar con el trabajo en base a cinco preguntas:
1.	¿Cómo influye la sobrecarga de partidos y entrenamiento en una posible lesión?
2.	¿Cómo afectan al futbolista sus niveles de estrés, nutrición y falta de sueño en una posible lesión?
3.	¿Haber sufrido una lesión previa aumenta las probabilidades de padecer una siguiente?
4.	¿Existen posiciones en las que es más probable sufrir una lesión?
5.	¿Los jugadores con mejores resultados en test físicos son más propensos a lesionarse?

Luego del análisis exploratorio de datos, el cuál posee anotaciones para comprender el procedimiento llevado a cabo y se encuentra disponible en la carpeta "EDA" junto los datos disponibles y la propuesta inicial del proyecto, decidimos agregar una pregunta más y hacer algunas modificaciones para mejorar el desarrollo del proyecto:
1.	¿Cómo afectan al futbolista sus niveles de estrés, en una posible lesión?
2.	¿Haber sufrido una lesión previa aumenta las probabilidades de padecer una siguiente?
3.	¿Existen posiciones en las que es más probable sufrir una lesión?
4.	¿Los jugadores con mejores resultados en test físicos son más propensos a lesionarse?
5.	¿Existe una vecindad en la que el nivel de estrés haga que la posibilidad de lesionarse se disparé?
6.	¿Existe un valor numérico de cuantas lesiones previas hace que el jugador sea mucho más propenso a lesionarse a futuro?
Cada pregunta es respondida en un archivo único ubicados en la carpeta "PREGUNTAS" acompañado de comentarios que facilitan la comprensión del proceso realizado.

Para el análisis y respuestas a las preguntas de investigación, escribimos códigos que requieren las siguientes librerías y funciones específicas:
-	pandas
-	os
-	seaborn
-	matplotlib.pyplot
-	numpy
-	sklearn.model_selection: train_test_split, KFold, GridSearchCV, cross_val_score, RandomizedSearchCV
-	sklearn.preprocessing: StandardScaler
-	sklearn.linear_model: LogisticRegression, LinearRegression
-	sklearn.metrics: classification_report, roc_auc_score, confusion_matrix
-	sklearn.pipeline: make_pipeline
-	sklearn.ensemble: RandomForestClassifier
-	sklearn.neighbors: KNeighborsClassifier
-	sklearn.tree: DecisionTreeClassifier, plot_tree


El procedimiento del proyecto fue llevado a cabo de la siguiente manera:
1. La propuesta y realización de preguntas fue definida en conjunto por todo el grupo.
2. "EDA" dividido en partes donde Cristobal Hernández se encargo de la limpieza de datos y verificar su calidad, Fernando Pavéz del proceso relacionado a la distribución de datos y estadísticas de estos, y Sebastian Blanco de la correlación entre datos y análisis multivariado.
3. En la realización de preguntas, Fernando Pavéz se encargo de responder las número 1, 2 y 3, mientras que Sebastian Blanco respondió las número 4, 5 y 6.
4. Para finalizar, Cristobal Hernández llevó a cabo el README junto la documentación del proyecto.
El proyecto esta organizado en carpetas :
- En EDA esta el notebook con el proceso de limpieza y exploracion de datos junto con un csv que es la base de datos.
- En la carpeta preguntas se encuentran los notebooks separados por cada pregunta que fue planteada en el EDA ,ademas se encuentra el archivo con los datos limpios.
- En la carpeta de propuesta de proyecto hay un pdf con la organizacion de nuestro proyecto ,donde estan las motivaciones y objetivos de este mismo.
EJECUCION Y REPRODUCTIBILIDAD :
Como fue mencionado anteriormente cada carpeta se encuentra con una base de datos,ya sea la original o con los datos ya limpios,por lo que si el usuario quiere interactuar con algun notebook no tendria problema,solo tiene que clonar el repositorio en su computador y ejecutarlo,siempre y cuando tenga instaladas las librerias que fueron mencionadas anteriormente en su computador.
