Este proyecto consiste en exponer 10 criptomonedas en Power BI, obteniendo datos estando conectados a la API de un exchange. Se pueden observar datos históricos en frecuencia diaria, como el precio de cierre y el volumen negociado en los activos. Adicionalmente, se incluye un pequeño análisis para el BTC/USD, que se basa en estudio de los ciclos de alzas y bajadas del precio de este en el tiempo, además de una predicción del precio a largo plazo.

Los criptoactivos expuestos son los siguientes BTC/USD, BNB/USD, DOGE/USD, MATIC/USD, LUNC/USD, ETH/USD, XRP/USD, SOL/USD, LTC/USD, USDT/USD, elegidos como parte de los más representativos de la industria de criptomonedas, cada uno cuenta con los datos extraídos en conexion en linea con la API publica del exchange FTX, que se almacenan en diferentes tablas, las cuales contienen los siguientes campos:

Fecha: se incluye un dato por día, para cada criptomoneda, desde el día desde que se dispone datos, hasta el día de hoy.

Precio Cierre: corresponde al precio con el cual se cierra el día de transacciones del activo, y se utiliza este debido a que es el más representativo para realizar cualquier tipo de análisis de estos instrumentos.

Volumen: corresponde a la cantidad transada durante 24 horas de cada uno de los activos representados.

También se incluye tabla BTC/USDComp, la cual contiene precios históricos estáticos de más larga data, obtenidos de otra fuente, necesaria para realizar análisis de largo plazo del precio y proyección de este a futuro. Esta tabla contiene los siguientes campos:

Fecha: se incluye un dato por día, para cada criptomoneda, desde el día desde que se dispone datos, hasta el día de hoy.

Close: corresponde al precio con el cual se cierra el día de transacciones del activo, y se utiliza este debido a que es el más representativo para realizar cualquier tipo de análisis de estos instrumentos. pero se encuentra multiplicado por factor 1.000.000.

Precio Cierre: corresponde al precio Close, dividido por 1.000.000, por lo cual es el precio correcto para realizar análisis con este.

Volumen: corresponde a la cantidad transada durante 24 horas de cada uno de los activos representados.

También se incluye tabla Calendario, la cual se requiere para realizar cálculos relacionados con el tiempo para el precio de cada activo, como por ej. media móvil.

Por último, se incluyen dos tablas AnalisisBTC y AnalisisBTCproy, en éstas se obtienen datos peak de precios de BTC/USD tanto para largos ciclos alcistas, como también para largos ciclos bajistas, la diferencia entre ambas, es que la segunda incluye una simple predicción de precio y fechas de cumplimiento, según comportamiento histórico. Las columnas de estas tablas son las siguientes:

Fecha: corresponde al año y mes del evento ocurrido con el precio de BTC/USD.

Precio Bitcoin: corresponde al precio de BTC/USD en cada peak análizado.

Meses transcurridos: tiempo en meses transcurridos, entre cada evento de subida y baja importante de precio.

Variación precio %: corresponde al porcentaje en que el precio varía, entre cada uno de los eventos importantes de movimiento en este.

Pizzas Disponibles: corresponde a un indicador lúdico del precio del BTC/USD, para ser utilizado en Storytelling.
