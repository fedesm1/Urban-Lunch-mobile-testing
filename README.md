# Linea de comandos y Bases de datos
# Descripción

En este proyecto, se realiza una practica de linea de comandos (CLI) donde se consulta ciertos registros especificos dentro de una base de datos y se manipulan dentro del servidor remoto, también se realizan consultas SQL a través de psql y PostgreSQL.

# Practica 1 Linea de comandos

<strong> ( Ejercicio 1 ) </strong>

El equipo de desarrollo ha enviado una tarea: debes averiguar qué solicitudes han venido de una dirección IP. Una dirección IP consta de cuatro números separados por un punto. Necesitas direcciones que comiencen con "233.201".

Los logs están en un servidor remoto en logs/2019/12. No sabes qué día ocurrió el error.

Tu tarea es averiguar qué solicitudes fueron enviadas.

Esto es lo que debes adjuntar en la respuesta:

El comando que usaste para obtener los logs necesarios.
Los strings adecuados, por ejemplo: 184.79.247.161 - - [30/12/2019:21:38:13 +0000] "PUT /alerts HTTP/1.1" 400 3557

<strong> ( Ejercicio 2 ) </strong>

Se ha detectado un error en el sistema. Estaba activo el 12.30.2019. En ese momento, había errores 400 y 500. Tu tarea consiste en guardar los logs que se registraron durante este periodo en un archivo independiente.  

Después, debes poner estos logs en archivos por separado con base en los errores. A continuación te explicamos cómo hacerlo:

En el directorio de inicio del servidor remoto, crea un directorio llamado bug1.
Pon todas las solicitudes que ocurrieron en el archivo main.txt en el directorio bug1.
Dentro del directorio bug1 , crea un directorio events.
Dentro del directorio events, crea archivos de error 400 y 500. Llama a estos archivos 400.txt y 500.txt, respectivamente. Identifica en ellos los logs utilizando el error correspondiente del archivo main.txt.
Esto es lo que debes adjuntar en la respuesta:

Los comandos que crean los directorios bug1 y events.
Los comandos que utilizaste para seleccionar los registros especificados para el archivo main.txt.
Los comandos que usas para colocar los logs en los archivos 400.txt y 500.txt de main.txt.
Los archivos de texto 400.txt y 500.txt.

# Practica 2 Bases de datos

<strong> ( Ejercicio 1 ) </strong>

Tienes una base de datos con los viajes en taxi. El plan era tener 10 550 vehículos disponibles, lo que cubre la demanda del usuario; sin embargo, el equipo recibió muchas quejas de que no había vehículos suficientes. ¿Cuántos taxis hay actualmente en las calles? La información sobre todos los automóviles suficientes está en la tabla cabs.

Ve al servidor remoto.
Conéctate a la base de datos chicago_taxi.
Cuenta el número total de automóviles en la tabla cabs. Recuerda que un automóvil podría pertenecer a distintas compañías.
Esto es lo que debes adjuntar en la respuesta:

Número de automóviles.
La solicitud que usaste para resolver el problema.

<strong> ( Ejercicio 2 ) </strong>

En la tabla cabs, cuenta el número de automóviles de cada compañía. Ordena los valores en orden descendente. El equipo piensa que algunas compañías no tuvieron suficientes automóviles disponibles.

Devuelve las compañías con menos de 100 automóviles. Llama cnt (contados) al campo con el número de automóviles, y company_name al campo con el nombre de la compañía.

Para resolver el problema, utiliza el operador HAVING, una analogía de WHERE para las funciones agregadas.

Esto es lo que debes adjuntar en la respuesta:

Una lista de compañías con menos de 100 automóviles.
La solicitud que usaste para resolver el problema.

<strong> ( Ejercicio 3 ) </strong>

Obtén una descripción de las condiciones meteorológicas de la tabla weather_records para cada hora.
Divide todas las horas en dos grupos a través del operador CASE: Está Bad ("mal") si el campo description contiene las palabras "rain" (lluvia) o "storm" (tormenta); Good ("bien"), para todas las demás horas.
Pon el nombre weather_conditions al campo resultante.
La tabla resultante debe tener dos campos: fecha y hora (ts) y weather_conditions.

Haz una selección para el periodo entre 11-05-2017 12:00 a. m. a 11-06-2017 12:00 a. m.

Esto es lo que debes adjuntar en la respuesta:

La tabla resultante con los datos para el periodo especificado.
La solicitud que ayudó a resolver el problema.

<strong> ( Ejercicio 4 ) </strong>

Tras actualizar el software, la compañía de taxis comienza a reportar que la ganancia que reciben no coincide con los datos que proporciona la aplicación. El equipo de desarrollo sugiere que el problema puede estar en los datos sobre el número de viajes.

Para determinar si hay un bug, debes obtener la selección del número de viajes de cada compañía de taxi para los días 15 y 16 de noviembre de 2017.

Devuelve el campo company_name. Nombra trips_amount (cantidad de viajes) al campo con el número de viajes y devuélvelo.
Organiza en orden descendente los resultados obtenidos en el campo trips_amount.
Pista: para resolver el problema, conecta las tablas de taxis y viajes.
Aplica funciones de agregación con agrupamiento. No olvides escribir la construcción con una condición.

Esto es lo que debes adjuntar en la respuesta:

La tabla resultante con los datos para el periodo especificado.
La solicitud que ayudó a resolver el problema.

# Técnicas

- Bases de datos
- SQL
- ProstgreSQL
- Linea de comandos
- Logs
- SSH protocol

# Estructura
<strong>Archivos:</strong>

1.	Consultas y respuestas: [Answers](https://docs.google.com/document/d/14rdVwx81fy0f-sgJOjzh1brqo9_gDq2d/edit?usp=sharing&ouid=105660489015748579866&rtpof=true&sd=true)
