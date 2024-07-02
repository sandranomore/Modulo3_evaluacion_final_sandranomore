EVALUACIÓN MÓDULO 3
SANDRA MORENO
Descripción
En esta evaluación del módulo 3 analizamos los datos de fidelización de clientes y actividad de vuelos para identificar patrones y tendencias que pueden influir en la estrategia de negocio.
Se divide en tres fases: exploración y limpieza de datos, visualización de datos y evaluación de diferencias.
Herramientas utilizadas en Visual Studio Code
•	Python: Para análisis y procesamiento de datos.
•	Pandas: Manipulación y análisis de estructuras de datos.
•	Matplotlib y Seaborn: Visualización de datos.
•	Scipy: Pruebas estadísticas.
•	Jupyter Notebook: Entorno de desarrollo interactivo.
Datos Utilizados
customer_loyalty_history
•	Información de fidelización de clientes.
•	Columnas clave: Salary, Cancellation Year, Cancellation Month, Country.
customer_flight_activity
•	Actividad de vuelos de clientes.
•	Columnas clave: Flights Booked, Distance, Points Accumulated, Points Redeemed, Education.
Contenido
Fase 1: Exploración y Limpieza
Dataframe customer_loyalty_history:
•	Valores atípicos en Salary
•	Datos faltantes en Salary
•	Datos faltantes en Cancellation Year y Cancellation Month
Dataframe customer_flight_activity:
•	Datos duplicados
•	Alta proporción de ceros en Distance
•	Relación entre Points Accumulated y Points Redeemed
•	Columnas eliminadas: Cancellation Year y Cancellation Month por alta proporción de valores nulos.
Fase 2: Visualización
2.1 Barplot / Lineplot
•	Interpretación: Muestra la cantidad de vuelos reservados por mes en 2017 y 2018.
•	Conclusión: Los picos más altos se observan en marzo y agosto, con una tendencia general ascendente en 2018.
2.2 Scatterplot
•	Interpretación: Relación entre la distancia de vuelos y puntos acumulados.
•	Conclusión: Tendencia positiva entre la distancia y los puntos acumulados.
2.3 Countplot
•	Interpretación: Distribución de clientes por provincia o estado.
•	Conclusión: Mayor concentración en Ontario, British Columbia y Quebec.
2.4 Countplot
•	Interpretación: Comparación del salario promedio según el nivel educativo.
•	Conclusión: Salarios más altos para niveles educativos "Doctor" y "Master".
2.5 Pieplot
•	Interpretación: Proporción de clientes por tipo de tarjeta de fidelidad.
•	Conclusión: Mayor número de clientes en el programa "Star".
2.6 Gráfico de Barras apiladas
•	Interpretación: Distribución de clientes según estado civil y género.
•	Conclusión: Mayor número de clientes casados, con una distribución de género similar.
Fase 3: Evaluación de diferencias
3.1 Preparación de Datos
•	Filtrado para incluir columnas relevantes: Flights Booked y Education.
3.2 Análisis Descriptivo
•	Promedio de vuelos: Similar entre niveles educativos (~4 vuelos).
•	Desviación estándar: Consistente entre niveles educativos.
•	Mediana: 1 vuelo reservado en todos los grupos.
3.3 Prueba Estadística: A/B Testing
Formulación de Hipótesis
•	H0: No hay diferencias significativas entre niveles educativos.
•	H1: Existen diferencias significativas entre niveles educativos.
Prueba de Normalidad (Shapiro-Wilk)
•	Resultados: Datos no siguen una distribución normal (p < 0.05).
Prueba Mann-Whitney U
•	Resultado: p-value = 0.0005, indicando diferencias significativas.
Conclusión
El proyecto proporciona insights sobre la relación entre características de los clientes y su comportamiento en reservas de vuelos, apoyando la toma de decisiones estratégicas.
El análisis de A/B testing revela diferencias significativas en el número de vuelos reservados entre niveles educativos superiores y básicos. Se rechaza la hipótesis nula, sugiriendo que el nivel educativo impacta en la frecuencia de reserva de vuelos.

