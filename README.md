1. Proceso de trabajo.

Lo primero que he hecho ha sido importar las bibliotecas de Python necesarias para la realización de este trabajo, así como emplear la función necesaria para que se puedan ver las gráficas completas, independientemente del tamaño de las mismas.

Nada mas abrir los dos archivos Excel, uno en formato .xslx y otro en formato .csv, he comprobado que no había ninguna forma de poder unir ambas tablas, dado que no había ningún elemento común con el que poder trabajar para compilar ambas tablas en una, por lo tanto, trabajé con cada tabla por separado. Intenté crear una tabla conjunta cuyo resultado fue que otra en la que aparece el nombre de cada una de las columnas de las dos tablas, pero el resto está vacío, dado que no hay ningún dato en común en las dos tablas que permita la conexión de la una con la otra.

Para todo el proceso, he empleado el programa Visual Studio Code, y el código Python para realizar las modificaciones y búsquedas dentro de lso archivos.

El proceso de limpieza de la tabla en formato .xslx ha sido muy sencillo por varias razones: el formato de la misma permite abrir el archivo sin tener que importarlo; aunque tanto el número de páginas como el número de filas del archivo es superior que el otro, este ha sido más sencillo de limpiar, dado que las variables a cambiar están determinadas por las columnas que, en este caso, son en menor cuantía que las del otro archivo. 

En este archivo las únicas modificaciones que he tenido que hacer han sido: la eliminación de la primera columna, dado que al ser una enumeración de las filas, no es relevante para llevar a cabo el estudio,; la modificación del formato de la segunda columna, llamada “Income”, a la que he añadido entre paréntesis la aclaración de que el valor está en euros, ya que al ser un valor monetario, he decidido añadirle los dos decimales, correspondientes a los céntimos de euro, pero como en todos los casos no hay decimales, estos no aparecen, la creación de una nueva columna, llamada Total children, que muestrael número total de hijos, resultante de sumar las columnas Kidhome y Teenhome y, por último, he decidido modificar la columna Dt_Customer, correspondiente a la fecha de alta como cliente de cada uno de ellos. En este caso, he eliminado el valor de la hora, ya que, al ser cero, no es relevante, así como la modificación del orden de la fecha, 
del establecido yyyy-mm-dd a dd-mm-aaaa, correspondiente al uso en España.

En lo que respecta al segundo archivo, el que tiene formato .csv, he tenido más dificultades a la hora de hacer la limpieza. También he eliminado la primera columna de enumeración, ya que tampoco es relevante para el estudio; también eliminé las columnas de Latitud y Longitud, que corresponde a los valores numéricos que representan la geolocalización de cada uno de los clientes. Como no aparecía en los requisitos del proyecto y tampoco le veía ninguna forma para poder trabajar con ellos, decidí eliminar ambas columnas. A continuación, 
he modificado los valores nulos de la tabla por Not Specified, como forma de mostrar que no disponemos de ese valor a la hora de hacer el estudio y que fuera una de las variables a tener en cuenta en el análisis. Después, he modificado los valores de las columnas en las que aparecen los valores 0 y 1 como forma de afirmación o negación por las palabras Sí o No, ya que son más visuales a la hora de realizar el estudio.

Como lo que se pretende en este ejercicio es demostrar las competencias adquiridas, una vez limpias y preparadas ambas tablas, lo primero que he hecho ha sido comprobar las dimensiones de ambas tablas usando la fórmula shape; también he querido investigar un poco sobre la información general que nos proporcionan las dos tablas: a través de la función info, que nos muestra el numero de valores nulos y no nulos de cada una de las columnas del archivo, asi como el tipo de dato que maneja cada una de las columnas de las dos tablas.

A continuación ya he entrado en el análisis estadístico de las tablas. Primero, he usado la función describe para conocer cierta información general de las estadísticas de la tabla clientes, como son el número de datos, la media, la desviación estandar, los valores mínimos y maximos, así como los cuartiles de los datos, es decir, los datos que representan la cuarta parte, la mediana y las tres cuartas partes de la tabla; luego he calculado por separado cada una de estas mismas variables, pero esta vez solo tneiendo en cuenta la columna de Edad de los trabajadores de la tabla datos-banco.

Por último, he decidido añadir tres representaciones gráficas de la tabla datos-banco, que creo que son interesantes que sean añadidas en el estudio: el primer gráfico, un diagrama lineal, representa la distribución de los trabajadores según su edad, el segundo es un gráfico de barras que pretende mostrar la distribución del a plantilla según su función dentro del banco y por último, un gráfico circular que representa la distribución de la plantilla según su estado civil.

2. Análisis.

Lo primero que he investigado ha sido el número de columnas y filas que tienen cada una de las tablas. En este caso, la tabla correspondiente a los datos de los clientes tiene un total de 43170 filas y 7 columnas; estas últimas corresponden a los datos de que disponemos de los clientes. Por otro lado, la tabla datos-banco, que corresponde a los datos de que disponemos de los empleados del banco consta de 43000 filas y 21 columnas que, en este caso, son los datos de que disponemos de los empleados.

Lo siguiente qye he analizado es el tipo de dato que podemos ver en cada una de las tablas. En el caso de la tabla de clientes, vemos que la mayoría de datos son numéricos, dado que solo las columnas Dt_Customer, que corresponde a la fecha de alta de los clientes y el ID o número de identificación del cliente se consideran como datos alfanuméricos y no numéricos únicamente; por otro lado, podemos ver que en la tabla datos-banco, todos los datos son alfabéticos, dado que los que eran numéricos los hemos modificado para una mejor comprensión.

Después hemos analizado las variables estadísticas de las dos tablas. En la tabla resultante de la fórmula describe podemos ver que el total de datos de la tabla clientes es de 43170 datos, que la media, por ejemplo de ingresos es de 93227.39€, siendo el valor mínimo 5841 € y el máxmo, 180802 €. también podemos ver, por ejemplo, que la desviación estandar del número total de hijos es de 1.15, lo que indica que al no ser un número muy elevado ni muy cercano a cero, esta desviación es moderada, no muy pronunciada, por lo que no hay mucha diferencia de unos trabajadores a otros en lo que respecta al número total de hijos.

A continuación hemos calculado las mismas variables, pero con la tabla datos-banco. En este caso, hemos calculado cada variable por separado. Asimismo, vemos que la media de edad de los trabajadores del banco es de 40 años. También podemos ver que la desviación estandar es de 10.44, que es muy pronunciada. Esto lo podemos comprobar también viendo las edades mínima y máxima de los trabajadores, que son de 17 y 98 años, lo que explica que la desviación estandar sea tan pronunciada.

Por último, hemos realizado 3 gráficas para estudiar la distribución por edad, por trabajo y por estado civil de los trabajadores del banco.

En la primera gráfica, una gráfica lineal, vemos que la moayoría de los trabajadores tienen entre 30 y 40 años, que la cifra de trabajadores va descendiendo desde los 40 años de forma progresiva hasta los 60. No encontramos casi trabajadores cuya edad sobrepase los 60 años. Lo mismo ocurreen las edades comprendidas entre los 17 y los 23 20 años que, aunque forman parte de la muestra, su presencia es casi resdual.

En la segunda gráfica, una gráfica de barras, vemos que las tres profesiones más comunes dentro del banco son administración, operarios (blue-collar) y técnicos. mientras que las tres con menor presencia en el banco son las de amas de casa, desempleados y estudiantes; también podemos ver que aunque sea el menor de los valores de la gráfica, una importante parte de la muestra no ha facilitado su labor dentro del banco. Aunque esta última cifra es importante, tampoco es lo suficientemente importante como para suponer un cambio en el orden de los valores dentro de la gráfica, por lo que no es relevante.

Por último, en la tercera gráfica, un diagrama circular, vemos que más de la mitad de los empleados del banco están casados, algo más de la cuarta parte de la muestra son solteros y algo más de la décima parte de los trabajadores están divorciados; solo el 0.2 % de los empleados no ha facilitado su estado civil. De nuevo, al ser un porcentaje muy poco elevado, no supone un impedimento para saber la distribución de los trabajadores según su estado civil. 
















