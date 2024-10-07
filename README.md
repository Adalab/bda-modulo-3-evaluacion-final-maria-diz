# Módulo 3: Ejercicio de evaluación final

## Los Datos
Los datos que se proporciona consisten en dos conjuntos de archivos que, en conjunto, describen el comportamiento de los clientes dentro de un programa de lealtad de una aerolínea.
Customer Flight Analysis.csv

Este archivo contiene información sobre la actividad de vuelo de los clientes, incluyendo el número de vuelos reservados, la distancia volada, puntos acumulados y redimidos, y costos asociados a los puntos redimidos.

•	Loyalty Number: Este atributo representa un identificador único para cada cliente dentro del programa de lealtad de la aerolínea. Cada número de lealtad corresponde a un cliente específico.
•	Year: Indica el año en el cual se registraron las actividades de vuelo para el cliente.
•	Month: Representa el mes del año (de 1 a 12) en el cual ocurrieron las actividades de vuelo.
•	Flights Booked: Número total de vuelos reservados por el cliente en ese mes específico.
•	Flights with Companions: Número de vuelos reservados en los cuales el cliente viajó con acompañantes.
•	Total Flights: El número total de vuelos que el cliente ha realizado, que puede incluir vuelos reservados en meses anteriores.
•	Distance: La distancia total (presumiblemente en millas o kilómetros) que el cliente ha volado durante el mes.
•	Points Accumulated: Puntos acumulados por el cliente en el programa de lealtad durante el mes, con base en la distancia volada u otros factores.
•	Points Redeemed: Puntos que el cliente ha redimido en el mes, posiblemente para obtener beneficios como vuelos gratis, mejoras, etc.
•	Dollar Cost Points Redeemed: El valor en dólares de los puntos que el cliente ha redimido durante el mes.
Customer Loyalty History.csv
 
Este archivo proporciona un perfil detallado de los clientes, incluyendo su ubicación, nivel educativo, ingresos, estado civil, y detalles sobre su membresía en el programa de lealtad (como el tipo de tarjeta, valor de vida del cliente, y fechas de inscripción y cancelación).

•	Loyalty Number: Identificador único del cliente dentro del programa de lealtad. Este número permite correlacionar la información de este archivo con el archivo de actividad de vuelos.
•	Country: País de residencia del cliente.
•	Province: Provincia o estado de residencia del cliente (aplicable a países con divisiones provinciales estatales, como Canadá).
•	City: Ciudad de residencia del cliente.
•	Postal Code: Código postal del cliente.
•	Gender: Género del cliente (ej. Male para masculino y Female para femenino).
•	Education: Nivel educativo alcanzado por el cliente (ej. Bachelor para licenciatura, College para estudios universitarios o técnicos, etc.).
•	Salary: Ingreso anual estimado del cliente.
•	Marital Status: Estado civil del cliente (ej. Single para soltero, Married para casado, Divorced para divorciado, etc.).
•	Loyalty Card: Tipo de tarjeta de lealtad que posee el cliente. Esto podría indicar distintos niveles o categorías dentro del programa de lealtad.
•	CLV (Customer Lifetime Value): Valor total estimado que el cliente aporta a la empresa durante toda la relación que mantiene con ella.
•	Enrollment Type: Tipo de inscripción del cliente en el programa de lealtad (ej. Standard).
•	Enrollment Year: Año en que el cliente se inscribió en el programa de lealtad.
•	Enrollment Month: Mes en que el cliente se inscribió en el programa de lealtad.
•	Cancellation Year: Año en que el cliente canceló su membresía en el programa de lealtad, si aplica.
•	Cancellation Month: Mes en que el cliente canceló su membresía en el programa de lealtad, si aplica.



## Ejercicio
### Fase 1: Exploración y Limpieza
1.	Exploración Inicial:
•	Realiza una exploración inicial de los datos para identificar posibles problemas, como valores nulos, atípicos o datos faltantes en las columnas relevantes.
•	Utiliza funciones de Pandas para obtener información sobre la estructura de los datos, la presencia de valores nulos y estadísticas básicas de las columnas involucradas.
 
•	Une los dos conjuntos de datos de la forma más eficiente.
2.	Limpieza de Datos:
•	Elimina o trata los valores nulos, si los hay, en las columnas clave para asegurar que los datos estén completos.
•	Verifica la consistencia y corrección de los datos para asegurarte de que los datos se presenten de forma coherente.
•	Realiza cualquier ajuste o conversión necesaria en las columnas (por ejemplo, cambiar tipos de datos) para garantizar la adecuación de los datos para el análisis estadístico.
### Fase 2: Visualización
Usando las herramientas de visualización que has aprendido durante este módulo, contesta a las siguientes preguntas usando el tipo de gráfica que consideres más adecuado (podéis ponerle fantasía a las gráficas ;-) ):
1.	¿Cómo se distribuye la cantidad de vuelos reservados por mes durante el año?
2.	¿Existe una relación entre la distancia de los vuelos y los puntos acumulados por los clientes?
3.	¿Cuál es la distribución de los clientes por provincia o estado?
4.	¿Cómo se compara el salario promedio entre los diferentes niveles educativos de los clientes?
5.	¿Cuál es la proporción de clientes con diferentes tipos de tarjetas de fidelidad?
6.	¿Cómo se distribuyen los clientes según su estado civil y género?


### Fase 3: Evaluación de Diferencias en Reservas de Vuelos por Nivel Educativo
Utilizando un conjunto de datos que hemos compartido, se busca evaluar si existen diferencias significativas en el número de vuelos reservados según el nivel educativo de los clientes. Para ello, los pasos a seguir son:

1.	Preparación de Datos: Filtra el conjunto de datos para incluir únicamente las columnas relevantes: 'Flights Booked' y 'Education'.
2.	Análisis Descriptivo: Agrupa los datos por nivel educativo y calcula estadísticas descriptivas básicas (como el promedio, la desviación estándar, los percentiles…) del número de vuelos reservados para cada grupo.
3.	Prueba Estadística: Realiza una prueba A/B Testing para determinar si existe una diferencia significativa en el número de vuelos reservados entre los diferentes niveles educativos.
