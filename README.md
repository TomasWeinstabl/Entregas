# Entregas

El trabajo consta de analizar las ventas de palta de la empresa Hass en distintas regiones de Estados Unidos entre los años 2015 y 2018.

El primer paso fue tomar una base de datos que sea útil para practicar análisis de datos. Elegí una base llamada "Avocado Prices" hallada en Kaggle. ((https://www.kaggle.com/datasets/neuromusic/avocado-prices)) La misma fue almacenada en una carpeta de Google Drive como archivo ".csv". 

Algunos de los campos mas relevantes de la base de datos son:
Date: dia/mes/año donde se vendió cierta cantidad de paltas. (en cierta región)
Average Price: precio promedio de la unidad de palta. (en cierto período y región)
Total Volume: cantidad de paltas vendidas. (en cierto período y región)
4046/4225/4770: cantidad de paltas vendidas de 3 genéticas de palta distintas. (en cierto período y región)
Total bags: cantidad de bolsas de palta vendidas. (en cierto período y región)
Small bags: cantidad de bolsas pequeñas de palta vendidas. (en cierto período y región)
Large bags: cantidad de bolsas grandes de palta vendidas. (en cierto período y región)
Xlarge bags: cantidad de bolsas muy grandes de palta vendidas. (en cierto período y región)
Type: el tipo de la palta vendida. Puede ser convencional u orgánica.
Región: región en la que se vendieron las paltas. (en cierto período)


Posteriormente, importé la base de datos a un archivo en formato ".ipynb" dentro de Google Colab  para poder analizar sus datos. Una vez dentro de Google Colab, importé las librerías Pandas, Matplotlib y Seaborn. Gracias a las funciones de estas 3 librerías pude generar 6 gráficas que nos permitirán a nosotros obtener algunos insights útiles sobre las características del negocio de Hass y su evolución en el tiempo.
