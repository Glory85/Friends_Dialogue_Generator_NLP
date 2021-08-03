
<h1> <b>CLASIFICADOR DE "QUOTES", GENERADOR DE DIÁLOGO Y VISUALIZACIONES VARIAS - SERIE FRIENDS:</b></h1>

Siempre he sido una fan de la serie friends, motivo por el cuál decidí hacer mi proyecto sobre la serie, pensando también en los fans que hay en todo el mundo. También encontré muy interesante la clase de NLP, así que quise profundizar un poco más en el tema. 

<h2> <b>OBJETIVO DEL PROYECTO</b></h2> Crear un clasificador de "quotes", un generador de diálogo y visualizaciones varias para publicarlos en alguna web de friends en honor a la reunión que ha tenido lugar este año. 

<h2> <b>DATASETS</b></h2>

Los datasets utilizados son: 

* **"friends_quotes"** : dataset de Kaggle https://www.kaggle.com/ryanstonebraker/friends-transcript: este dataset incluye los guiones de casi todos los capítulos de la serie. El dataset contiene las siguientes columnas: 
  * author
  * episode_number
  * episode_title
  * quote
  * quote_order
  * season 

* **"Guest_Stars_DF"** : dataset creado a partir del friends_quotes dataset y modificado manualmente. Este contiene las líneas que han tenido diferentes actores/actrices invitados/as a la serie durante las 10 temporadas: Este dataset lo completé manualmente con información encontrada en varios artículos por internet. 
  * https://www.radiotimes.com/tv/comedy/best-friends-guest-stars/
  * https://www.bustle.com/entertainment/23313-73-famous-friends-guest-stars-you-totally-forgot-were-ever-on-the-show
  
* **"season1_df_modified"** : dataset creado a partir del friends_quotes dataset y modificado manualmente. Este contiene las conversaciones por parejas (no contiene las conversaciones grupales), de los 9 personajes que más frases tienen en la primera temporada

* **"script_ross"** : dataset creado a partir del friends_quotes dataset y modificado manualmente. Este contiene los diálogos entre Ross y otras personas de la serie en la primera temporada --> escogi a Ross ya que era el personaje con más diálogo en la primera temporada por parejas. 

<h2> <b> PREGUNTAS </b></h2>

<h3> <b> PREGUNTA 1: ¿Cuáles son los 9 personajes con más líneas de texto en cada temporada? </b> </h3>

Para responder esta pregunta he visualizado un countplot con seaborn y he filtrado las diferentes temporadas con ipywidgets.

<h3> <b> PREGUNTA 2: ¿Cuáles de estos personajes hablan más entre ellos en la primera temporada? </b> </h3>

Con la información del count plot podemos ver que los 9 personajes que más líneas de texto tienen en la primera temporada son: Ross,Monica, Rachel, Chandler, Joey, Phoebe, Carol, Susan, Janice. He representado las conversaciones entre ellos mediante un nx.Graph(). 


<h3> <b> PREGUNTA 3: ¿Qué actores/actrices invitados aparecieron durante las 10 temporadas?¿Incrementó el número de actores/actrices invitados/as a lo largo de las 10 temporadas? </b> </h3>

He visualizado la evolución de la  lMediante plotly.express 

<h3> <b> PREGUNTA 4: ¿Quién de los 6 personajes principales es más positivo/negativo? </b> </h3>

<h3> <b> PREGUNTA 5: Clasificador de "quotes": ¿Quién ha dicho qué? </b> </h3>

<h3> <b> PREGUNTA 6: Generador de diálogo: ¿qué diría Ross? </b> </h3>

