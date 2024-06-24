<h1>Movie Analysis</h1>

> [!NOTE]
> Este es un proyecto que pretende en base a un análisis de los datos oficiales de peliculas y tvseries generar insight de negocio para una empresa de stremaming que busca entrar al mercado. <br>

<h2>Problema del negocio</h2>

<table><tr><td> 
<p align="justify">Una plataforma de streaming para el hogar, con presencia en todo el mundo, necesita impulsar su rendimiento utilizando datos de tendencias en el sector de manera estratégica. </p>
</td></tr></table>

<h2>Tecnologías Usadas</h2>

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black) 

<h2>Objetivos</h2>
  
  1. <p align="justify"> ¿Cual es la evolución del rating por tipo de contenido? </p>
  2. <p align="justify"> ¿Cual es el rating promedio por género? </p>
  3. <p align="justify"> ¿Cuáles son los géneros que proporcionan mayor ROI? </p>
  4. <p align="justify"> ¿Cuáles son los países con mayor producción de contenido? </p>
  5. <p align="justify"> Series de TV más vistos </p>
  6. <p align="justify"> Sugerencia de películas a traer al catálogo </p>

<h2> Análisis Exploratorio de los Datos(EDA) </h2>

**Tiempo de duración en Minutos**

<p align="center">
  <img src="https://github.com/Marioarellano21/Movie_Analysis/assets/146877817/87e9907a-a511-45c0-9c49-42712f5baa54" alt="Tiempo de duración en Minutos" />
</p>

<p align="justify"> Encontramos valores atípiocos/extremos con cantidad de miles de minutos, por eso observamos una gráfica donde la mayor concentración de datos esta en 0 en teoría, lo que pasa es que tenemos valores extremos tan grandes que parece que esto, pero la realidad es que las peliculas suelen tener duración de entre 1 hora(60 min) a 2 horas(120min) normalmente, algunas otras suelen durar entre las 2 y 3 horas, pero estas son un poco más excepcionales, es decir si establecemos como un maximo(180min) en cuanto a minimo 15min, ya que hay series que sus capitulos rondan los 15-20min de duración, vemos como mejora el boxplot en gran medida, donde ya no observamos datos atípicos.</p>

**Estrenos porcentaje de estrenos por año/Cantidad de estrenos por año**

<p align="center">
  <img src="https://github.com/Marioarellano21/Movie_Analysis/assets/146877817/f331cb0d-923c-4ca9-88ea-f2ff64914def" alt="Tiempo de duración en Minutos" />
</p>

<p align="justify"> Podemos observar que la mayoría de las películas y series han sido producidas y estrenadas en el siglo 21, en estos ultimos 20 años se han lanzado aproximadamente unos 300mil titulos lo que representa un 62% de nuestros datos, dividos la primera decada de los 2000 con un 33% de estos lanzamientos y en la segunda epoca, en este caso incluyendo los ultimos 4 años un 29% de lanzamientos, parece que con el paso de tiemp disminuyo un poco la cantidad de producciones realizadas, como la compañia es de streaming y los tiempos van cambiando constantemente, limitaremos el análisis de las producciones entre el año 1990 hasta el presente año 2024, el resto no las consideraremos porque aunque fueron de gran impacto en su epoca, hoy en día pueden que no tengan el mismo impacto debido a los grandes cambios culturales que hemos tenido en estas dos ultimas decadas.</p>


<h2> Conclusiones y sugerencias</h2>
<p align="justify"> A raíz de los objetivos planteados, hicimos con la hipótesis de determinar si ciertos actores, que aportan mayor ROI , o mayor cantidad de contenidos a su vez son los que tienen mayor cantidad de votos por la audiencia. y/o viceversa. Por ello presentamos unas sugerencias de películas que son prácticamente nuevas y no están en el catálogo de la plataforma de streaming con la que trabajamos filtrandos por los tres géneros más destacados Aventuras, Ciencia Ficción y Acción. Lo presentamos en una carpeta llama `output` que tiene esta estructura.</p>

```
  ├── outpus
      	├── actors_common_title_basics.csv
      	├── genre_actors_tmdb_df.csv
      	├── title_basics_"genre"_actors.csv      <- "genre" es el género en concreto de la lista
        ├── tmdb_"genre"_actors.csv              <- "genre" es el género en concreto de la lista
        └── tmdb_movies_genre_common.csv
```

> [!IMPORTANT]
> Esto fue un proyecto que participamos los miembros del canal del
> 
>[![](https://img.shields.io/youtube/channel/subscribers/UCuerQOTskuNkddcT738357g?style=for-the-badge&logo=youtube&label=Bootcamp%20Xperience)](https://www.youtube.com/@BootcampXperience)
