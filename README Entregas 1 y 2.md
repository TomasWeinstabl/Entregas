# Entregas

Entrega 1

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

Entrega 2

Para la segunda entrega me hubiese gustado hacer un algoritmo de regresión para poder asignarle un precio de venta a los productos en función  de su fecha de venta. Esto sería útil:
1. Para extrapolar, estimando los precios futuros de venta en fechas posteriores a las analizadas.
2. Para interpolar, estimando el precio de venta de algún lote de productos, entre las fechas analizadas, del cual no se haya registrado su precio de venta por el vendedor.

El algoritmo de regresión no fue viable ya que la correlación entre la variable temporal y el precio era baja.

Por lo tanto, opté por hacer un algoritmo de clasificación que logre determinar a qué tipo de avocado (convencional u orgánico) corresponde un lote vendido de avocados en función de su fecha de venta y de su precio. Esto podría ser útil para aquellas ventas en donde el distribuidor no haya registrado a qué tipo de avocado correspondía determinado lote vendido.

Utilicé el algoritmo KNeighborsClassifier. Configuramos como variable "X" a una matriz de dos columnas, siendo éstas el campo Timestamp (es decir, el campo original Date pero tranformado a valores enteros Unix) y el campo AveragePrice (es decir, el precio). Además, configuramos como variables "y" al output del algoritmo, siendo éste 0 si se trata de avocados convencionales o 1 si se trata de avocados orgánicos.

Posteriormente, dibujé una gráfica, siendo el eje X el tiempo y el eje Y el precio unitario del avocado. En el mismo, se puede visualizar las fronteras de decisión del algoritmo.

Por último, imputé 4 putos distintos hayados en la gráfica para comprobar que efectivamente, el output del algoritmo coincidiese con lo que se visualiza en la gráfica, y efectivamente, así fue.

