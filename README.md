#### Navega por los siguientes links para acceder a los files de cada proyecto
##### Browse the following links to access the files for each project


> ## [Supply Chain HIV & Malaria Project](https://github.com/PriscilagsData/files_projects/tree/4a8590818c0df87efe50426fb646b6c1a391ee49/Supply%20Chain%20Medicine%20HIV%20%26%20Malaria)
>
> ###### Cadena de suministro global de productos de la salud. Estudio de geomercado - HIV & Malaria. Este database proporciona específicamente datos sobre presupuesto, envío y costo de productos sanitarios. Detallan composición, dosis, marcas, costos, entre otras características de los insumos, información referida a la logística de los envíos y su administración, países involucrados en las transacciones y fechas de realización. Los registros corresponden a un rango temporal de 10 años, entre 2006 y 2015. Originalmente en formato csv, cuenta con 33 columnas o atributos y 10324 registros. Se realiza un arduo proceso de ETL para comenzar con el análisis efectivo.
> ###### La logística de envíos asociada al abastecimiento de este tipo de insumos por parte del SCMS se encuentra dividida en proyectos asignados a cada país y pueden analizarse desde diversas ramas. Principalmente se destacan las vías de transporte utilizadas en cada envío, los tipos de contratos de compraventa internacional de mercancías consumados, e incluso las oficinas desde donde se administra cada movimiento. Para la organización de los datos se procede al proceso de normalización del DB mediante un diagrama de entidad-relación o DER, acompañado de un diagrama relacional, definiendo características como PK y FK o tipos de campo.
> ###### Desde Power BI Desktop se importan las tablas del archivo Excel producto de la normalización previa y se procede a la etapa de Transformación de datos. Se controlan las relaciones de tablas autodetectadas y se editan en base al modelo relacional como parte de las buenas prácticas. Se crea la tabla Calendario y Medidas. Se crean nuevas columnas mediante funciones DAX, como así medidas de interés. Las dos principales segmentaciones utilizadas en el estudio son las de “Afección” y “Efecto”, ya que son el punto de partida para realizar una categorización genérica de los datos, pudiendo orientar el estudio a cada “tipo de mercado” por separado (HIV o Malaria).
> ###### El SCMS, en el período comprendido entre los años 2006 y 2015, ha contado con 142 proyectos asociados a 43 diferentes países destino, y un total de 7030 envíos. La demora de entrega del envío ha sido de 141 días promedio. La vía de envío principal es Air, seguida por Truck, casi cubriendo el 90% del total. El INCOTERM EXW es el más utilizado en este tipo de envíos para insumos médicos y la principal oficina encargada de la administración de los movimientos del sistema es aquella ubicada en USA. Por otro lado, vemos que Nigeria es el país con mayor cantidad de envíos, con un total de 927, con amplia diferencia frente al país del segundo puesto. Con respecto a las ventas, podemos observar que los países demandantes de insumos están ubicados exclusivamente en el hemisferio sur. Específicamente el HIV con fuerte presencia en el continente africano, mientras que la malaria se ubica en zonas de Centroamérica y algunos países puntuales de áfrica como Nigeria y la República Democrática del Congo. Esta información se correlaciona con el dato de alta cantidad de envíos a Nigeria en el período.
> ###### Pasando a los fabricantes, filtrando por afección malaria, se puede observar claramente que en USA la cantidad de insumos producidos es notoriamente menor a la proporción monetaria ganada con respecto a otros países fabricantes. Lo opuesto se representa para la India. Diviendo ganancias por cantidad de fabricantes, llegamos a ver reflejado en la tabla los valores de promedio de ganancias por fabricante y concluimos que USA es pionera, seguida de China y luego India. Algo diverso se observa al filtrar por HIV, siendo ahora India quien toma el primer puesto y USA queda fuera incluso del top 10.
> ###### La India arrasa el primer puesto con respecto a la diversificación de su producción, contando 83 productos diversos. Amplia diferencia con el segundo puesto de USA, con una diversificación de solo 22 productos. Otro dato interesante es que solo 7 países son fabricantes de insumos para la malaria (con ventas de 167 millones de dólares anuales), mientras que para el HIV más de 20.
> Fuente DB: https://catalog.data.gov/dataset/supply-chain-shipment-pricing-data-07d29
---

> ## [Seattle Energy Report](https://github.com/PriscilagsData/files_projects/tree/4a8590818c0df87efe50426fb646b6c1a391ee49/Seattle%20Energy%20Report%20-%20Tableau)
>
> ###### Evaluación energética edilicia de la ciudad de Seattle en 2016. El DB extraido de Kaggle incluye campos detallados de cada propiedad: nombre, dirección, tax ID number, año de construcción, nº de edificios, nº de pisos, GFA (parking y edificio). Además categoriza las propiedades según su barrio, uso primario y uso principal. Dentro de los datos energéticos, detalla gastos eléctricos y de gas natural (en kBtu) y emisiones de gases de efecto invernadero (GHG Emissions). En este reporte se busca analizar el consumo energético de las propiedades de la ciudad de Seattle a presentar a su Secretaría de Ambiente y Energía, registrado durante el año 2016. Más particularmente, se busca detectar relaciones o tendencias entre dicho consumo energético y las diferentes características asociadas a las propiedades como ubicación o barrio, tipo de uso y superficie total (GFA).
> ###### Se realizan tres reportes: GHG EMISSIONS, ENERGY CONSUMPTION, STRUCTURAL ANALYSIS. Algunas de las conclusiones obtenidas del proceso de análisis de datos fueron: Los barrios con mayor emisión de gases de efecto invernadero en 2016 (EAST y DOWNTOWN); top 10 propiedades de mayor emisión y caracterización del puesto número 1 ("Plant 2 Site"); tendencia detectada que sugiere que a menor antiguedad de la propiedad, mayor es el consumo energético asociado; propiedad con mayor consumo eléctrico (Universidad de Washington), y la de mayor consumo de gas natual (Plant 2 Site); tipos de propiedades con mayor aporte al total de consumo energético (aproximadamente 50%) (Oficinas, Residencias y Escuelas/Universidades); el área (GFA) de las propiedades de la ciudad se divide en un muy pequeño porcentaje de parking con respecto a una amplia superficie edificada.

---

> ## [Data jobs Analysis](https://github.com/PriscilagsData/files_projects/tree/4a8590818c0df87efe50426fb646b6c1a391ee49/Data%20jobs%20Project)
> 
> ###### Base de datos formato original .csv de 9355 entrevistados con puestos de trabajo en Data a nivel mundial en el período 2020 - 2023. Se registran nombre y categoría del puesto, modalidad de trabajo y esquema laboral, además incluye datos referentes a los trabajadores como lugar de residencia, nivel de experiencia, edad y otros como referencias salariales en sus monedas efectivas y su equivalente en USD. El DB es importado y trabajado en Excel. Luego de la limpieza, eliminación de duplicados, corrección, organización y ETL general del DB se aplican listas de validación y filtros útiles para el práctico manejo de los datos. Se realizan cálculos auxiliares recurriendo a las funciones avanzadas de Excel, minigráficos y formatos condicionales de barras, set de ícomos y escala de colores que facilitan la lectura de valores obtenidos.
> ###### Algunas de las líneas de análisis fueron: categorización de salarios en USD basado en rangos, promedio de salario según nivel de experiencia, recaudación total en dólares de los trabajadores dentro de la categoría "Data Analysis" en el año 2023, cotización del USD para cada moneda al momento del registro, definición de tipos de trabajadores entre "Nómade Digital" o "Trabajador Establecido" con funciones condicionales y diagrama de Pareto de distribución de trabajadores respecto del área de trabajo. Utilizando Segmentadores conectados o relacionados a tablas y gráficos dinámicos, se vincula toda la información obtenida y se expone en pantalla las visualizaciones en un Dashboard interactivo. 
---
