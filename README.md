# API NLP - Servicio de análisis de sentimientos
Ejemplo de API alojada en Heroky, proyecto Data&Analytics Feb 2020 bootcamp FT.

# Overview
La API se encuentra alojada en Heroku, sirve datos extraidos de la base de datos de MongoDB Atlas y procesados usando la libreria nltk de NLP.

# Documentación
Ofrece un servicio de análisis de series, pudiendo extraer el sentimiento capítulo a capítulo de cualquier tipo de producto audiovisual, con el objetivo de recomendar las series en base a su similaridad.

*** Index: @get("/help")

*** User endpoints:
Create a new user: @post('/user/create')
Recommend a user to another user (based on nlp words similarity): @get("/user/<user_id>/recommend")

*** Chat endpoints:
Create a new chat document: @post('/chat/create')
Extract sentiment from a certain chat: @get("/chat/<chat_id>/get_sentiment")
