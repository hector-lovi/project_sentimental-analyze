# Procesamiento de lenguaje natural
Este repositorio tiene como objetivo la creación de un sistema de análisis focalizado al contenido audiovisual (principalmente series).  

Mediante una API construida en Python con Flask el usuario podrá almacenar contenido audiovisual (mediante un estilo similar al de un guión), pudiendo consultar dicho contenido, analizar su positividad / negatividad e incluso generar una recomendación.

# Documentación  

**Ayuda**  
`@get("/help")`

**Crear usuario partícipes en episodios**  
`@post('/user/create')`  

**Crear un episodio**  
`@post('/episode/create')`

**Sustraer el sentimiento de un capítulo concreto**  
`@get("/episode/<episode_id>/get_sentiment")`

**Recomendador de episodios**  
El usuario deberá de generar una breve descripción, se analizará y se le devolverá una recomendación acorde con la descripción.  
`
docs = {
    'description':'bitch, dildo, big black, aliens, Mr. Hat'
}  

@get('/episode/recommend', params=docs).text`
