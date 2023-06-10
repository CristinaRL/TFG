El código está organizado en dos carpetas, con un notebook cada una, donde encontramos el código realizado.
Los notebooks que contienen el código son Creacion.ipynb y Procesamiento.ipynb.

En Procesamiento de datos encontramos todo el procesamiento de los datos y la obtención de otros mediante el uso de la API de Last.fm.
En Creación del grafo encontramos lo relativo a la creación del grafo, la implementación de la adaptación del algoritmo de Axelrod y las pruebas realizadas.

Los ficheros originales usados, que se encuentran en el archivo hetrec2011-lastfm-2k.zip, son los siguientes:

* artists.dat: Contiene la información sobre los artistas musicales escuchados.

* user_artists.dat: Contiene los artistas escuchados por cada usuario. También provee la cantidad de reproducciones para cada par [usuario, artista].

El formato de los datos es el siguiente:

* artists.dat
   
        id \t name \t url \t pictureURL

        Ejemplo:
        707	Metallica	http://www.last.fm/music/Metallica	http://userserve-ak.last.fm/serve/252/7560709.jpg

* user_artists.dat
	
	userID \t artistID \t weight

	Ejemplo:
	2	51	13883

Los ficheros principales creados son:

* artists-v2.dat: Contiene la información sobre los artistas actualizada. Además se han eliminado los artistas incorrectos o de los que no disponemos suficiente información.

* tags-v3.dat: Contiene los 213 tags que hemos seleccionado como válidos.
* tags-sorted.dat: Contiene los 213 tags que hemos seleccionado como válidos ordenados según los géneros a los que pertenecen y su origen musical.
* tags_to_delete.dat: Contiene los tags a eliminar.
* tags_to_delete-v2.dat: Contiene los tags a eliminar y/o reemplazar.
* tags_to_replace.dat: Contiene los tags a eliminar.
* tags_freq.dat: Contiene todos los tags que habíamos recopilado inicialmente junto con el número de apariciones de cada uno de ellos.

* artist_tags.dat: Contiene los artistas con sus 10 tags (como máximo) más frecuentes.
* artist_tags-v2.dat: Contiene los artistas con sus 10 tags (como máximo) más frecuentes. Los tags son solo los que hemos seleccionado como válidos.

* matrix.txt: Matriz de adyacencia del grafo.
* matrix_percentage.txt: Matriz de adyacencia del grafo en porcentajes.

* final_matrix.txt: Matriz de adyacencia agrupada en géneros musicales. En porcentajes y normalizada.



