# Trabajo_Practico_OpenData
Trabajo Practico de Open Data Componente 2. Por Axel Mathias Petta.

Primeramente se deben importar una serie de librerias para poder realizar el scrapping. Luego de subir el csv "super_seis_ofertas2.csv", procedemos a definir los headers.
Luego con la libreria de r request insrtamos la url de la pagina a realizar el scrapping.
Posteriormente visualizamos el contenido y utilizamos la libreria "soup = BeautifulSoup(content)".
Se define una funcion para obtener los datos de la pagina web, definiendo el tag principal a utilizar (esto se hace manualmente inspeccionando el codigo html de la pagina de Super 6). Una vez definido el tag principal "('div', attrs={'class':'item-box'}" procedemos a buscar los tags y sentenciar los datos que deseamos obtener, que en este caso son el nombre del producto, el precio y la marca del mismo. 
Una vez obtenido los resultados, creamos un data frame con la libreria de Pandas, y guaramos el data frame en un csv.
Con "df" visualizamos los datos del data frame y visualizamos que las columnas contienen errores. Una vez limpiado los datos procedemos a visualizar nuevamente el data frame y guardamos los datos limpios en un csv nuevo.
Finalmente, una vez obtenidos todos los datos de las ofertas en las columnas deseadas en un data frame y en un csv, visualizamos los valores de forma ascendente para ver de una manera mas interactiva las ofertas.
