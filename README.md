
# Dashboard de Análisis de Ventas de Electrónicos (2021-2023)

##  Resumen del Proyecto
Este proyecto desarrolla un ecosistema de Business Intelligence para analizar el rendimiento comercial de una empresa de electrónicos durante un periodo de tres años. El enfoque principal fue la **consolidación de datos** provenientes de múltiples hojas de Excel y la normalización de registros para una visualización precisa.

## Stack Técnico
* **Data Source:** Microsoft Excel diferentes datasets de 2021, 2022, 2023.
* **ETL & Data Cleaning:** Power Query (Lenguaje M).
* **Modelado de Datos:** Esquema en Estrella (Star Schema).
* **Visualización:** Power BI Desktop con medidas DAX avanzadas.

##  Desafíos Técnicos y Soluciones (ETL) ⚙️
* **Consolidación de Datos:** Se anexaron dinámicamente tablas de diferentes periodos anuales, asegurando la consistencia de tipos de datos.
* **Integridad Referencial:** Implementación de lógica en Lenguaje M como inyección de registros "comodín" (ID 99 - Online). Esto resolvió el problema de registros huérfanos en Sucursal ID , eliminando los valores "(En blanco)" en los reportes. Tambien para caracteres especiales en registros de Clientes.
* **Normalización:** Tratamiento de nulos y limpieza de strings para dimensiones de Sucursales y Clientes. Separacion de columnas para valores monovalentes y atomicos. Uso de Calendario. Y generacion de ID.

##  Análisis Destacados 📊
* **Análisis de Vendedores:** Ranking de performance y segmentación por sucursal.
* **Comportamiento del Cliente:** Clasificación por nivel de cuenta (Plata, Oro, Platino) y tipo (Normal, Corporativa, Revendedor).
* **Venta por Temporalidad:** Análisis comparativo de tickets por día de la semana y mes.

## Vista del Proyecto  📸 
![alt text](ModeloEstrella.png)
![alt text](Inicio.png)
![alt text](Personas.png)
![alt text](Ventas.png)

##  Uso de IA y Eficiencia 🤖
En este proyecto, utilicé herramientas de IA generativa para optimizar el ciclo de desarrollo:
* **Copilot/Geminis:** Soporte de scripts de limpieza en Lenguaje M y funciones DAX complejas.
* **Documentación:** Automatización de la documentación técnica y comentarios de código.
* **Optimización:** Refactorización de consultas SQL para mejorar el rendimiento de la carga de datos.


*En este proyecto se comprende el ciclo completo de datos, desde la extracción y limpieza hasta la entrega de valor mediante dashboards estratégicos.*
