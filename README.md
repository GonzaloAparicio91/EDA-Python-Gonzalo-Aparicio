1. Proceso de trabajo.

Lo primero que he hecho ha sido importar las bibliotecas de Python necesarias para la realización de este trabajo, así como emplear la función necesaria para que se puedan ver las gráficas completas, independientemente del tamaño de las mismas.

Nada mas abrir los dos archivos Excel, uno en formato .xslx y otro en formato .csv, he comprobado que no había ninguna forma de poder unir ambas tablas, dado que no había ningún elemento común con el que poder trabajar para compilar ambas tablas en una, por lo tanto, 
trabajé con cada tabla por separado. Intenté crear una tabla conjunta cuyo resultado fue que otra en la que aparece el nombre de cada una de las columnas de las dos tablas, pero el resto está vacío, dado que no hay ningún dato en común en las dos tablas que permita la 
conexión de la una con la otra.

Para todo el proceso, he empleado el programa Visual Studio Code, y el código Python para realizar las modificaciones y búsquedas dentro de lso archivos.

El proceso de limpieza de la tabla en formato .xslx ha sido muy sencillo por varias razones: el formato de la misma permite abrir el archivo sin tener que importarlo; aunque tanto el número de páginas como el número de filas del archivo es superior que el otro, 
este ha sido más sencillo de limpiar, dado que las variables a cambiar están determinadas por las columnas que, en este caso, son en menor cuantía que las del otro archivo. 

En este archivo las únicas modificaciones que he tenido que hacer han sido: la eliminación de la primera columna, dado que al ser una enumeración de las filas, no es relevante para llevar a cabo el estudio,; la modificación del formato de la segunda columna, 
llamada “Income”, a la que he añadido entre paréntesis la aclaración de que el valor está en euros, ya que al ser un valor monetario, he decidido añadirle los dos decimales, correspondientes a los céntimos de euro, pero como en todos los casos no hay decimales, estos no 
aparecen y, por último, he decidido modificar la columna Dt_Customer, correspondiente a la fecha de alta como cliente de cada uno de ellos. En este caso, he eliminado el valor de la hora, ya que, al ser cero, no es relevante, así como la modificación del orden de la fecha, 
del establecido yyyy-mm-dd a dd-mm-aaaa, correspondiente al uso en España.

En lo que respecta al segundo archivo, el que tiene formato .csv, he tenido más dificultades a la hora de hacer la limpieza. También he eliminado la primera columna de enumeración, ya que tampoco es relevante para el estudio; también eliminé las columnas de Latitud y 
Longitud, que corresponde a los valores numéricos que representan la geolocalización de cada uno de los clientes. Como no aparecía en los requisitos del proyecto y tampoco le veía ninguna forma para poder trabajar con ellos, decidí eliminar ambas columnas. A continuación, 
modifiqué los valores nulos de la tabla por Not Specified, como forma de mostrar que no disponíamos de ese valor a la hora de hacer el estudio y que fuera una de las variables a tener en cuenta en el análisis- Después, modifiqué los valores de las columnas en las que 
aparecen los valores 0 y 1 como forma de afirmación o negación por las palabras Sí o No, ya que son más visuales a la hora de realizar el estudio.

Como lo que se pretende en este ejercicio es demostrar las competencias adquiridas, una vez limpias y preparadas ambas tablas, lo primero que he hecho ha sido comprobar las dimensiones de ambas tablas usando la fórmula shape; también he querido investigar un poco sobre la 
información general que nos proporcionan las dos tablas: a través de la función info, que nos muestra el numero de valores nulos y no nulos de cada una de las columnas del archivo, asi como el tipo de dato que maneja cada una de las columnas de las dos tablas.

A continuación ya he entrado en el análisis estadístico de las tablas. Primero, he usado la función describe para conocer cierta información general de las estadísticas de la tabla clientes, como son el número de datos, la media, la desviación estandar, los valores mínimos
y maximos, así como los cuartiles de los datos, es decir, los datos que representan la cuarta parte, la mediana y las tres cuartas partes de la tabla; luego he calculado por separado cada una de estas mismas variables, pero esta vez solo tneiendo en cuenta la columna de 
Edad de los trabajadores de la tabla datos-banco.

Por último, he decidido añadir tres representaciones gráficas de la tabla datos-banco, que creo que son interesantes que sean añadidas en el estudio: el primer gráfico, un diagrama lineal, representa la distribución de los trabajadores según su edad, el segundo es un 
gráfico de barras que pretende mostrar la distribución del a plantilla según su función dentro del banco y por último, un gráfico circular que representa la distribución de la plantilla según su estado civil.

2. Análisis de las dos tablas.
