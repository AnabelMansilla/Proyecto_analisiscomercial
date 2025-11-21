# Proyecto de análisis comercial para Data Analytics - ÍCARO 

Como parte del curso de Data Analytics dictado por ÍCARO y avalado por la Universidad Nacional de Córdoba y para su aprobación final se realizó un análisis de evolución de indicadores en una cadena de insumos informáticos con recomendaciones finales. La base de datos fue brindada por la misma institución en formato Excel y se procesó de la siguiente manera:

- Aplicación completa de ETL (Extract, Transform, Load). Con una limpieza de datos realizada en Power Query.
- Se determinaron métricas y KPIs relevantes para el área comercial en base a experiencias en el rubro de comercio.
- De acuerdo a los datos disponibles se procedió a realizar un análisis exploratorio en tres áreas relevantes:
  - Un resumen del estado de ventas para el año 2019,
  - Un análisis detallado en cuánto a la participación de cada categoría de productos sobre el total de ventas,
  - Distribución geográfica de las sucursales vs la ubicación de los clientes.
- Se presentaron observaciones sobre los principales insights y acciones recomendadas. 

## CONSIGNAS DEL TRABAJO FINAL 



- Expondrán ante la Dirección General, una presentación ejecutiva de un tablero analítico. Uds son los analistas de datos de una prestigiosa cadena de comercialización de insumos tecnológicos.

- El tablero contendrá todos los aspectos desarrollados en clases, cumpliendo con:
  - Al menos 3 Indicadores y/o Métricas
  - Al menos un KPI
- Gráficos que den cuenta del comportamiento de negocio, atendiendo a los criterios de las visualización efectivas
- Mapa a elección, implementado en Power Bi  
 
- Como analistas de datos, se les pide que hagan recomendaciones:
  - Operativas y Comerciales (del negocio y sus resultados, logística, ventas, reubicación de sucursales, etc), 
  - Del Estado de Arte de los datos (DataQuality, mejora de sistemas recomendadas, prospección, etc)
        
---

## RECOMENDACIONES OPERATIVAS Y COMERCIALES

### Ventas, Ticket medio y Piezas por Ticket.

![Reporte de ventas año 2019](https://github.com/AnabelMansilla/Proyecto_analisiscomercial/blob/main/Anabel_Mansilla_page-0001.jpg?raw=true)

##### Observación: 
El Ticket medio es igual al total de ventas sobre la cantidad de tickets emitidos, representa el promedio abonado por cada compra y refleja los hábitos de compra del cliente. 
Por otra parte, a lo largo del año 2019 el valor de las PPT oscila entre 1,12 y 1,13; lo cual indica que la mayoría de ventas es de sólo un producto por ticket, lo que lleva a su vez a un impacto directo de la rotación de los productos y al riesgo de llegar a un sobrestock.
##### Acciones:
- Ofrecer planes de financiación atractivos.
- Reforzar la atención al cliente. Escuchar, entender sus necesidades, ofrecer artículos acordes y comunicar medios de pago.
- Ubicar productos de mayor valor en puntos focales para incrementar su visibilidad.
- Reforzar la venta cruzada (ofrecer productos complementos a aquellos que el cliente desea comprar).
- Promociones en compras de varias unidades.
- Evaluar el componente de estacionalidad en los meses con menos ventas: enero (verano), julio y junio (meses de invierno). Incorporar productos que tienen alta demanda en esos meses del año.

### Categorías y productos

![](https://github.com/AnabelMansilla/Proyecto_analisiscomercial/blob/main/Anabel_Mansilla_page-0002.jpg?raw=true)


##### Observación: 
Las categorías menos rentables son también las que ofrecen menos variedad de productos.
##### Acciones:
- Diversificar los productos en las categorías grabación, bases, gaming y limpieza.
- Evaluar la continuidad del rubro de limpieza por su baja participación.
- Comprobar si los precios de la categoría impresión se encuentran actualizados.
- Asegurar la reposición de los productos de acuerdo a la demanda y capacidad de los mobiliarios donde se exhiben.
- Planificar acciones periódicas de Visual Merchandising y hacer un seguimiento semanal de su impacto en los indicadores y top de ventas.

### Distribución geográfica de clientes.

![](https://github.com/AnabelMansilla/Proyecto_analisiscomercial/blob/main/Anabel_Mansilla_page-0003.jpg?raw=true)

##### Observación:
La provincia que menor monto de venta ha tenido en el año 2019 es Río Negro, con un total por $3.568.454,53 y una participación del 0,95% sobre el ingreso total en el país. Río Negro posee solo una sucursal en el país.  Los clientes más cercanos a esa sucursal se concentran en la provincia de Neuquén, donde no hay sucursales abiertas.
##### Acciones:
- Evaluar la posibilidad de la apertura de una sucursal en Neuquén.
- Planear alguna estrategia de Marketing para atraer a más clientes de la zona y un programa de fidelización.
- Evaluar la posibilidad de establecer un sistema logístico que facilite la entrega de productos desde Rio Negro a Neuquén para retener esos clientes.

---
## RECOMENDACIONES EN CUANTO A LA CALIDAD DE LOS DATOS

- Contar con una base de datos sobre el stock de productos tanto en área de ventas como en depósito para generar un indicador de rotación de productos y analizar la posible existencia de sobre-stock y quiebres.
- En la base de proveedores agregar la división por rubro.
- Almacenar los datos de clientes: ID, nombre, apellido, domicilio, localidad, provincia y locación geográficas (latitud y longitud) en una única base de datos.
- Agregar la opción de elegir de una lista la provincia para evitar confusiones al cargar nuevos datos. Se ha observado la carga Ciudad Autónoma de Buenos Aires (CABA) como una provincia en diferentes tablas.
- Agregar la opción de elegir a partir de una lista la categoría al momento de cargar los productos. En la tabla de productos existía un único producto cargado como "opción 1" pero correspondiente a la categoría gabinetes.
- Para aquellos productos que no puedan encasillarse en alguna de las categorías pueden cargarse como pertenecientes a una categoría llamada "Varios" u "Otros", para evitar así la existencia de valores nulos en este campo.
- Analizando la tabla "Productos" se observa que existen dos productos duplicados, es decir, que responden al mismo concepto, con diferente ID y Precio.
- Revisar la existencia de productos cargados con precio "0".

---
## DEVOLUCIÓN FINAL

Excelente trabajo. El proyecto refleja un análisis muy completo y estratégico de las ventas a nivel país, combinando métricas clave, análisis de productos, categorías y clientes con visualizaciones altamente efectivas en Power BI. La presentación de los datos es clara y profesional, y la paleta de colores utilizada facilita la interpretación de la información, destacando tendencias, comparaciones y áreas críticas de forma inmediata.

Aspectos destacados:

- Ticket medio y piezas por ticket: La evolución a lo largo del año y la identificación de los meses de menor venta (enero, junio y julio) permite comprender la estacionalidad y planificar acciones específicas para esos períodos.

- Ventas por categoría y productos: La visualización de Pareto y los top 5 de productos más y menos vendidos facilitan priorizar productos estrella, reforzar ventas cruzadas y tomar decisiones de stock.

- Distribución geográfica: La ubicación de clientes y sucursales permite identificar oportunidades de expansión (como Neuquén) y diseñar estrategias logísticas y comerciales para zonas con baja cobertura.

- Recomendaciones operativas: Se proponen acciones claras sobre stock, promociones, fidelización de clientes, diversificación de productos, actualización de precios y visual merchandising, todas respaldadas por los datos analizados.

- Calidad de datos: Se destacan las observaciones sobre estandarización, eliminación de duplicados, nulos y carga correcta de categorías y provincias, lo que asegura confiabilidad en el análisis.

- Visualización y presentación: La combinación de gráficos de barras, líneas, mapas y tablas, junto con la paleta de colores, genera un dashboard intuitivo y agradable a la vista, haciendo que los insights sean fácilmente comprensibles y accionables por la gerencia.

Conclusión:
Este reporte demuestra un manejo profesional de Power BI, un análisis profundo de los datos y recomendaciones concretas y estratégicas. La visualización de los datos no solo comunica la información de manera efectiva, sino que también convierte el dashboard en una herramienta de apoyo para la toma de decisiones a nivel gerencial. Realmente un trabajo sobresaliente, tengo que decir que me encanto tu visualización! Felicitaciones!


