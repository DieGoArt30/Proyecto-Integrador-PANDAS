# Proyecto Integrador Dataset - PROTALENTO.
El proyecto de este curso consiste en analizar el conjunto de datos introducido en esta sección, procesarlo, limpiarlo y finalmente ajustar modelos de machine learning para realizar predicciones sobre estos datos.

## Fases de las entregas del proyecto.
El desarrollo de este proyecto está planeado en 5 fases de entrega, teniendo en cuenta las indicaciones del mentor de Protalento.

### Proyecto Dataset - Parte No. 1 (Introducción al análisis de datos):
Se va a trabajar con un dataset sobre fallo cardíaco El dataset contiene registros médicos de 299 pacientes que padecieron insuficiencia cardíaca durante un período de seguimiento. Las 13 características clínicas incluidas en el conjunto de datos son:

Edad: edad del paciente (años)
Anemia: disminución de glóbulos rojos o hemoglobina (booleano)
Presión arterial alta: si el paciente tiene hipertensión (booleano)
Creatinina fosfoquinasa (CPK): nivel de la enzima CPK en la sangre (mcg/L)
Diabetes: si el paciente tiene diabetes (booleano)
Fracción de eyección: porcentaje de sangre que sale del corazón en cada contracción (porcentaje)
Plaquetas: plaquetas en la sangre (kiloplaquetas/mL)
Sexo: mujer u hombre (binario)
Creatinina sérica: nivel de creatinina sérica en la sangre (mg/dL)
Sodio sérico: nivel de sodio sérico en la sangre (mEq/L)
Fumar: si el paciente fuma o no (booleano)
Tiempo: período de seguimiento (días)
[Objetivo] Evento de fallecimiento: si el paciente falleció durante el período de seguimiento (booleano)
El objetivo en esta etapa del proyecto integrador es convertir la lista de edades a un arreglo de NumPy y calcular el promedio de edad de las personas participantes en el estudio.
Archivos de la Entrega No. 1:
PD_parte1_promedioEdad.py
Readme.md
heart_failure_clinical_records_dataset.csv
Proyecto Dataset - Parte No. 2 (Carga de datos):
Continuando con la anterior sección del proyecto integrador, se debe realizar lo siguiente:

Convertir la estructura Dataset en un DataFrame de Pandas usando pd.DataFrame.
Separar el dataframe en dos diferentes, uno conteniendo las filas con personas que perecieron (is_dead=1) y otro con el complemento.
Calcular los promedios de las edades de cada dataset e imprimir.
Archivos de la Entrega No. 2:
PD_parte2_cargaDatos.py
Proyecto Dataset - Parte No. 3 (Calculando analíticas simples):
Continuando con el DataFrame con todos los datos de la anterior subsección, ahora se debe hacer lo siguiente:

Verificar que los tipos de datos son correctos en cada colúmna (por ejemplo que no existan colúmnas numéricas en formato de cadena).
Calcular la cantidad de hombres fumadores vs mujeres fumadoras (usando agregaciones en Pandas).
Archivos de la Entrega No. 3:
PD_parte3_analiticaSimple.py
Proyecto Dataset - Parte No. 4 (Procesando información en bruto):
Imagina que no tuvieramos el acceso fácil de estos datos a través de la librería y tuvieramos que descargar los datos usando requests. Los datos son accesibles en esta dirección https://huggingface.co/datasets/mstz/heart_failure/raw/main/heart_failure_clinical_records_dataset.csv

Realizar un GET request para descargarlos y escribir la respuesta como un archivo de texto plano con extensión csv (no se necesita pandas para esto, sólo manipulación de archivos nativa de Python).
Agrupar el código para esto en una función reutilizable que reciba como argumento la url.
Archivos de la Entrega No. 4:
PD_parte4_procesandoInfoEnBruto.py
ResultadoConsulta.csv
