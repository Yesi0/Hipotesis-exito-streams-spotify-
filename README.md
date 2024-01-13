# Armonía de Datos: Análisis Predictivo del Streaming Musical en Spotify

El repositorio en GitHub presenta un análisis detallado de las tendencias de streaming en Spotify. La metodología incluyó el uso de BigQuery para ejecutar consultas complejas en un dataset extenso, la aplicación de Power BI para crear dashboards interactivos, y la implementación de algoritmos de aprendizaje automático en Python para el análisis predictivo. Las conclusiones se derivaron de pruebas estadísticas y modelado de datos para evaluar hipótesis sobre el éxito en Spotify. 

## Los principales hallazgos son:

Los BPM altos no garantizan un mayor número de streams.
Existe una correlación entre el éxito en Spotify y otras plataformas como Deezer.
La presencia en playlists multiplica significativamente la probabilidad de obtener más streams.
No se encontró una relación directa entre la cantidad de canciones de un artista y su éxito en streams.
Características como la energía y la valencia de la música tienen un impacto significativo en la popularidad.
El código y las visualizaciones están disponibles para su revisión, ofreciendo una visión integral que puede guiar la estrategia de lanzamiento de artistas emergentes.

## Dashboard 

<img width="643" alt="image" src="https://github.com/Yesi0/Hipotesis-exito-streams-spotify-/assets/125078076/daf8a1ab-a077-4c24-88c3-2d428f088fd4">

## REGRESIÓN LINEAL
### Strems vs participación en playlist
<img width="458" alt="image" src="https://github.com/Yesi0/Hipotesis-exito-streams-spotify-/assets/125078076/b8137368-1181-4392-b801-96adf3fb5ace">

El modelo sugiere una relación positiva y significativa entre la participación en listas de reproducción y los 'streams' de una canción, aunque no captura toda la variabilidad y presenta un error considerable en las predicciones. Esto podría ser una indicación de que otros factores adicionales afectan los 'streams' o que la relación no es estrictamente lineal.

 [CLICK AQUI MAS DETALLE](https://colab.research.google.com/drive/1LhAAGk5A7pisNzWOXoW5JGJu5voRrM9S?usp=sharing)
 
## ANALISIS mannwhitney 
Hipotesis 0 = El promedio de streams entre las caracteristicas de la musica alto y bajo es la misma. 

Hipotesis 1 = EL promedio de streams entre las caracteristicas de la musica alto y bajo es distinta.

Alfa = 0.05

<img width="202" alt="image" src="https://github.com/Yesi0/Hipotesis-exito-streams-spotify-/assets/125078076/7e92a18a-9ea4-4c7c-b524-3c8ed1fe5e8f">

si alfa 0.05 > p-value: SI existe diferencie significativa en los promedios de streams entre los grupos

si alfa 0.05 < p-value: NO existe diferencie significativa en los promedios de streams entre los grupos


interpretacion: No Existe una diferencia significativa en los promedios de streams entre los grupos, excepto en la caracteristica Speech, que si refleja una diferencia.

Esto podría implicar que la característica speechiness ( la cantidad de palabras habladas en una canción) tiene un impacto en cuántas veces se reproduce una canción, mientras que las otras características no parecen tener un efecto significativo.

[CLICK AQUI MAS DETALLE](https://colab.research.google.com/drive/1msSzUEYk69ueBKfSbiWz8oZC70ZnbyG3?usp=sharing)

