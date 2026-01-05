Análisis End-to-End: La Paradoja del Mundial de Hockey 2023

Objetivo del Proyecto
El objetivo principal fue determinar la estrategia clave para ganar el Mundial de Hockey 2023:
1. Ofensiva Pura:¿El equipo con mejor rendimiento estadístico y mayor volumen de goles (Países Bajos) fue el campeón?
2. Resiliencia:¿El éxito fue determinado por la capacidad de ganar partidos de eliminación directa, especialmente en situaciones de máxima presión como los penales (Alemania)?


Stack Tecnológico
Este proyecto se desarrolló siguiendo un flujo de trabajo completo (End-to-End) de Análisis de Datos:

ETL (Extracción, Transformación y Carga):MySQL
     Se utilizó para la creación de la base de datos, la gestión de esquemas, la limpieza de datos (ej. estandarización de nombres de equipos y manejo de valores `NULL` en los resultados de penales), y la creación de consultas de análisis complejas.
Visualización y Modelado de Datos:Power BI
 Se utilizó para establecer el Modelo de Estrella (conectando Clasificación, Jugadores, Goleadores y Resultados) y crear un Dashboard interactivo con KPIs y visualizaciones dinámicas.

 Hallazgos Clave (Insights)

El análisis demostró una clara diferencia entre la fase de grupos y la fase eliminatoria:

1. Dominio Estadístico de Países Bajos: El equipo finalizó la fase de grupos con la mejor ofensiva (130 Goles en la métrica total del torneo) y la mayor eficiencia (mayor `GF` vs. menor `GC`).Esto se visualiza en el Gráfico de Dispersión.
2. La Resiliencia de Alemania fue la clave: El campeón, Alemania, ganó un total de 4 partidos en la fase final. Dos de estas victorias cruciales fueron decididas por tanda de penales.
   Conclusión: El factor determinante para el campeonato no fue la potencia ofensiva, sino la capacidad de ganar en situaciones de alta presión, como se demuestra en el Gráfico de Resiliencia.

Dashboard Final en Power BI
 
Visualización del Dashboard

A continuación, se presenta el Dashboard interactivo que resume los hallazgos clave del torneo:

![Dashboard del Mundial de Hockey](./Dashboard_Mundial_Hockey.PNG)

Estructura del Repositorio
 `SQL_Queries.sql`: Contiene todo el código SQL para la creación de la base de datos, la limpieza de datos y las consultas analíticas que extrajeron los insights.
 `Mundial_Hockey_Dashboard.pbix`: El archivo fuente de Power BI con el modelo de datos, las relaciones y todas las visualizaciones del Dashboard.