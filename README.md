# Análisis de Vuelos 🛫

**Tabla de contenido**

- [Temática](#Temática)
- [Objetivos](#Objetivos)
- [Modelado de datos](#Modelado)
- [Dashboard](#Dashboard)
- [Proyecto](#Proyecto)

------------

### Temática
La temática seleccionada es sobre los vuelos del año 2015 de Estados Unidos.
La base de datos contiene datos de vuelos de los Estados Unidos del año 2015. Cuenta con datos sobre los horarios de salida y llegada, tiempo de retraso, cancelaciones y sus motivos.

------------

### Objetivos
Se realizaron análisis para encontrar insights de interés dentro del rubro, como identificar los aeropuertos y las compañías de aerolíneas con mayor cantidad de vuelos. También se estudiaron los tiempos de retrasos y sus motivos y la cantidad de cancelaciones y sus motivos.
Específicamente los objetivos planteados fueron:
- Identificar los aeropuertos y compañías de aerolíneas que tienen mayor cantidad de vuelos.
- Identificar si existe algún periodo de meses en particular donde existe mayor cantidad de vuelos.
- Identificar el tiempo promedio en minutos perdido por vuelo por tipo de demora.
- Identificar los aeropuertos y aerolíneas con mayor demora.
- Identificar si existe algún periodo de meses en particular con mayor tiempo de demora.
- Identificar cuáles son los principales motivos de cancelación de cada aerolínea y de cada aeropuerto.
- Identificar si existe algún periodo de meses en particular donde ocurren mayores cancelaciones.

### Modelado
Para la limpieza y normalización de los datos se utilizó PowerQuery creandosé un modelo de datos tipo estrella.

![DER_bi](https://user-images.githubusercontent.com/86801780/178976760-8121dee8-2229-4191-9f81-795a90ae0f10.jpg)
> Modelo de datos

## Dashboard
El dashboard se confeccionó en PowerBI. 

Para más información sobre las medidas, cálculos y parámetros utilizados ver la [Documentación.](https://github.com/mariaaguirreescalada/dashboard-vuelos/blob/master/Analisis_vuelos2015.pdf "Documentación")

- **Portada**

![Portada](https://user-images.githubusercontent.com/86801780/178976782-7100e2f6-d05f-4526-9d54-41e725384370.jpg)
> Contiene información del proyecto. Se incluyen iconos que redireccionan a cada una de las solapas del dashboard.

------------
- **Glosario**

![Glosario](https://user-images.githubusercontent.com/86801780/178976798-35ca1bc2-845a-45d9-b13b-65a5f931227c.jpg)
> Explica la funcionalidad de los iconos utilizados y la referencia a cada tipo de retraso y cancelación, esto se realizó mediante figuras que despliegan la descripción al posicionarse sobre ellas.

------------

- **Resumen**

![Resumen](https://user-images.githubusercontent.com/86801780/178976808-369ea6f3-84f7-4332-8df2-7ec7ac04805a.jpg)
> Contiene los principales indicadores y el listado Top 3 de aeropuertos y aerolíneas más utilizadas.

------------

- **Análisis de Aeropuertos**

![Aeropuert](https://user-images.githubusercontent.com/86801780/178976820-97531947-41d3-40f8-8722-84b13f5d6e74.jpg)
> Muestra los aeropuertos y aerolíneas más utilizadas. Las tarjetas representan la cantidad de vuelos total y el porcentaje que representan dichos vuelos del total. Se observa la evolución de la cantidad de vuelos por cada mes del año. Posee un  mapa  coroplético, donde se representa la cantidad de vuelos por estado.

------------

- **Análisis de Retrasos [Tiempo Promedio]**

![Retrasos_TP](https://user-images.githubusercontent.com/86801780/178976844-764dae21-0d3d-46a4-9d82-21282f5602c2.jpg)
> Top 5 de aerolíneas con mayor tiempo promedio de retraso. La tarjeta indica los minutos promedio de retraso por vuelo. Se observa la evolución del tiempo perdido según el mes del año. El gráfico treemap muestra el total de minutos de retraso para cada tipo de demora. El mapa coroplético representa el tiempo promedio de retraso por estados.

------------

- **Análisis de Retrasos [Tiempo Total]**

![RetrasosTT](https://user-images.githubusercontent.com/86801780/178976856-a88ca428-43a5-4bbb-ae46-6e3da6aabed0.jpg)
> Esta solapa representa la misma información que la solapa anterior solo que los tiempos son expresados en minutos.

------------

- **Análisis de Cancelaciones**

![Cancelaciones](https://user-images.githubusercontent.com/86801780/178976881-70a04979-b671-423f-b6e4-d94394f07846.jpg)
> Top 5 de aerolíneas con menos cancelaciones. Se observa la evolución de la cantidad de cancelaciones por mes y la cantidad de cancelaciones por motivo de cancelación.
Se visualizan 2 KPI que indican la relación entre la cantidad de vuelos cancelados y la cantidad de cancelaciones permitidas por año. Esta cantidad de cancelaciones puede ser modificada mediante una barra deslizable, los valores permitidos están entre 0 y 90.000 con pasos de 10.000.

------------

### Proyecto 
Para mayor detalle puede explorar el proyecto:
> [Analisis_Vuelos.pbix](https://drive.google.com/file/d/1y5A87iO7lQsnffbGUfF-59AKNvzar8ge/view?usp=sharing)

------------

Puede **descargar la base de datos** utilizada con el siguiente link:
> Airline Flight Delays  https://www.mavenanalytics.io/data-playground
