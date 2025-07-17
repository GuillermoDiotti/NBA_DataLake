# NBA_DataLake

Construcción de un DataLake con distintas herramientas y tecnologías para el análisis de registros de la NBA

## Repositorio con los dataframes seleccionados

[Repositorio](https://github.com/GuillermoDiotti/NBA_DATA)

## Stack Tecnológico

- Hive (Ingesta de datos hacia HDFS)
- HDFS (Sistema de almacenamiento organizado por zonas)
- Spark (Framework que permite el procesamiento sobre los dataframes)
- Hive (Herramienta utilizada para la ejecución de consultas sobre los datos)
- SuperSet (Encargada de la creación de dashboards para visualizaciones)

## Zonas

Para un almacenamiento organizado, estructurado y limpio se definen las siguientes zonas dentro de HDDFS

- lnd (landing) -- zona que aloja los datos raw de la fuente de datos
- rfn (refined) -- zona que aloja los datos refinados, luego de limpiezas de duplicados, nulos, etc
- mld (modeled) -- zona que aloja los datos modelados luego del refinamiento, sobre esta zona se realizan las consultas en hive
- anl (analytics) -- zona que aloja los datos preparados para la analítica y visualizacion
