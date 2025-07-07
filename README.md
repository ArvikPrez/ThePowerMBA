DASHBOARD ANALISIS DE MERCADOS ELECTRICOS

Actualmente, trabajo en una consultoria energética en la cual se ofrecen distintos servicios a comercializadoras electricas. Uno de nuestros pilares fundamentales, desde mi grupo de trabajo, es el de analizar los distintos mercados eléctricos, para intentar aprovechar al maximo las oportunidades de compra y venta de energía en función de la situación real de la peninsula iberica. 

Para ello, la intención de este dashboard, es proporcionar, de manera rápida y visual, como se encuentran los ultimos dias una serie de mercados, en este caso de REE, como son las restricciones técnicas de Fase I y Fase II (RRTT en el Dashboard), y además unas gráficas visuales para que se pueda revisar quienes han sido los agentes de mercado que han vendido y han comprado en las distintas subastas intradiarias del día en curso (DIA D)

La estructura del proyecto es un fichero excel, en el cual se trae mucha informacion desde la web publica de Red Electrica de España, la cual tiene la siguiente ruta https://www.esios.ree.es/es/generacion-y-consumo?date=22-07-2023 
Toda la información que se muestra en el excel ha sido descargada via API, que es propiedad de mi empresa y he tenido que eliminar por normativa interna. Pero se puede descargar desde la web de esios ya que es una informacion pública. 
Además de esto, hay distintas macros de VBA y un codigo de PYTHON para descargar los ficheros de P48, que son los programas de los distintos agentes de mercado en cada una de las horas diarias, esto se usa para ver la trazabilidad de quiénes son los agentes compradores y vendedores en los distintos mercados electricos. 
Dentro del codigo python que utilizo para traer los P48, uso las librerias xlwings, pandas, requests, io y openpyxl

Los resultados son bastante claros, por un lado podemos observar las previsiones de la demanda, solar fotovoltaica, solar termica y eolica terrestre para los proximos cuatro dias, esto nos da una informacion de qué puede ocurrir en los mercados proximos. 
Luego traemos la informacion de los mercados de REE de Restricciones técnicas fase I y fase II, tanto en volumen de energía como en spread de precios. Y por ultimo representamos tres gráficas, cada una perteneciente a cada subasta intradiaria del dia en curso y en ella agrupamos por tecnología el volumen de compra y de venta en cada hora. 

El objetivo de los siguientes modulos es intentar mejorar este dashboard, me gustaria introducir, si fuese posible, mas tablas, y ademas me gustaria que apareciese de alguna forma quiénes son los agentes de mercado que, en cada hora, han comprado o vendido mas volumen. 

AUTORES: Álvaro Pérez Castañeda
