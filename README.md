# ML_musica_urbana
Buscamos desarrollar un modelo de regresión que prediga la popularidad actual (abril de 2025) de canciones previamente relevantes, todas dentro del marco del género urbano, mediante el análisis de:
- Características técnicas del audio (tempo, RMS, flatness, etc.)
- Métricas de engagement del artista (seguidores, popularidad histórica)
- Metadatos del track (duración, año de publicación, colaboraciones, formato, etc.)

El target es el dato de popularidad (popularity) según Spotify a abril 2025, un valor numérico entre 0 y 100 que indica el nivel de interés actual de un tema según Spotify. Se pretende capturar su comportamiento como indicador de vigencia o éxito sostenido en el tiempo.

Para conformar el dataset, vamos a buscar los lanzamientos dentro del género urbano, en el contexto español, es decir, que tuvieron cierta relevancia en nuestro país, fuera cual fuera el origen del track. 
Aunque los lanzamientos abarcan un amplio intervalo de tiempo, el 65% aprox. son desde el 2020 en adelante, y cerca del 90% del 2015 en adelante.

El modelo final se guarda en la carpeta src/models/ como un archivo .pkl, lo que permite reutilizarlo o integrarlo en pipelines futuros sin necesidad de reentrenamiento.

------------------------------------------------------------------------------------
We aim to develop a regression model that predicts the current popularity (as of April 2025) of previously relevant songs, all within the urban music genre, by analyzing:
- Technical audio features (tempo, RMS, flatness, etc.)
- Artist engagement metrics (followers, historical popularity)
- Track metadata (duration, release year, collaborations, format, etc.)

The target variable is the popularity score provided by Spotify in April 2025 — a numerical value ranging from 0 to 100, indicating a song’s current level of public interest. The goal is to capture this value as a proxy for ongoing relevance or sustained success over time.

To build the dataset, we selected songs that belong to the urban music genre and had some degree of relevance within the Spanish market, regardless of the artist's country of origin.
Although the dataset spans a wide range of years, approximately 65% of the tracks were released after 2020, and nearly 90% after 2015.

The final model is saved in the folder src/models/ as a .pkl file, which makes it easily reusable or integrable in future pipelines without the need for retraining.

