# Diseño del camino de datos

### Elemento del camino de datos
Un **elemento del camino de datos** es una unidad funcional utilizada para operar o mantener un dato dentro de un procesador.En la implementación MIPS, los elementos del camino de datos incluyen las memorias de instrucciones y datos, el banco de registros, la unidad aritmético-lógica (ALU), y sumadores.

### Banco de registros
El **banco de registros** es un elemento de estado que consiste en un conjunto de registros que pueden ser leídos y escritos proporcionando el identificador del registro al que se desea acceder. Se necesita una ALU para poder operar con los valores leídos de los registros.

### Sumador
El **sumador de registros** es un elemento encargado de incrementar el PC (descrito en el tema 5) para que apunte a la dirección de la siguiente instrucción,.Se representa como una ALU con la etiqueta de sumador.

### Extensión de signo
La **extensión de signo** consiste en incrementar el tamaño de un dato mediante la replicación del bit de signo del dato original en los bits de orden alto del dato destino más largo.

### Multiplexor
Un **multiplexor** es un dispositivo encargado de seleccionar entre las múltiples líneas de datos.

### Memoria de instrucciones
La **memoria de instrucciones** almacena las instrucciones del programa que está siendo ejecutado.

### ALU
La **ALU** se encarga de realizar las operaciones aritméticas (suma, resta, multiplicación, etc) y lógicas (AND, OR, NOT, etc).

### Shift left 2
EL **Shift left 2** es un tipo de operación de desplazamiento de bits en la que los bits se mueven dos posiciones a la izquierda, lo que es equivalente a multiplicar el número por 4.

### Memoria de datos
La **memoria de datos** es la parte de la memoria que almacena los datos mientras se ejecuta. A diferencia de la memoria de instrucciones, que solo contiene las instrucciones del programa, la memoria de datos contiene las variables y otros datos que el programa manipula durante su ejecución.


# Jerarquía de memoria

### Jerarquía de memoria
Estructura que utiliza múltiples niveles de memorias. A medida que aumenta la distancia desde el procesador, aumenta el tamaño de las memorias y el tiempo de acceso.

### Localidad temporal
Principio que establece que si se accede a la dirección de memoria de un dato, pronto se accederá de nuevo a esa dirección.

### Localidad espacial
Principio de localidad que establece que si se accede a la dirección de memoria de un dato es accedida, pronto se accederá a las direcciones de memoria que se encuentren próximas a ella.

### Jerarquía de memoria
Estructura que utiliza varios niveles de memoria, a medida que aumenta la distancia desde la CPU, el tamaño de las memorias y el tiempo aumentan.

### Bloque
Unidad mínima de información que puede estar o no presente en una jerarquía de dos niveles.

### Frecuencia de aciertos
Fracción de accesos a memoria que se encontraron en un nivel determinado de la jerarquía de memoria.

### Frecuencia de fallos
Fracción de accesos a memoria que no se encontraron en un determinado nivel de la jerarquía de memoria.

### Tiempo de acierto
Tiepo necesario para cceder a un determinado nivel de la jerarquía de memoria, incluido el tiempo necesario para determinar si el acceso corresponde a un acierto o a un fallo.

### Penalización por fallo
Tiempo necesario para ir a buscar un bloque a un determinado nivel de la jerarquía de memoria partiendo desde otro nivel inferior, incluido el tiempo necesario para acceder al bloque, transmitirilo de un nivel al otro y guardarlo en el nivel que experimentó el fallo.

### Caché con correspondencia directa
Organización de caché en la que cada posición de memoria principal se corresponde con una única posición en la caché.

### Caché completamente asociativa
Estructura de caché en la cual un bloque puede ser emplazado en cualquier posición de la caché.

### Caché asociativa por conjuntos
Caché que tiene un número establecido de posiciones (al menos dos) donde cada bloque puede ser emplazado.

### Etiqueta
Campo de cada una de las entradas de la tabla utilizada por la jerarquía de memoria que contiene información de la dirección que es necesaria para identificar si el bloque de información asociado se corresponde con la palabra solicitada.

### Bit de validez
Campo de cada una de las entradas de la tabla utilizada por la jerarquía de memoria que indica que el bloque asociado en la jerarquía contiene datos válidos.

### Menos recientemente utilizado (Least Recently Used, LRU)
Política de reemplazamientos en la cual el bloque reemplazado corresponde al que no ha sido usado por el periodo de tiempo más largo. Es el más utilizado.

### Menos frecuentemente usado (Least Frequently Used, LFU)
Política de reemplazamiento en la cual el bloque reemplazado corresponde al que no ha sido usado un mayor número de veces.

### Memoria virtual
Técnica que permite a un sistema operativo ejecutar programas que requieren más memoria de la que están físicamente disponible en la RAM (memoria principal). Esto se logra al usar una combinación de memoria RAM y almacenamiento secundario (disco duro o SSD) para simular una memoria más grande. Está organizada en páginas, que son bloques de memoria de tamaño fijo. Estos tamaños pueden ser 1 KiB, 4 KiB, 16 KiB, o más. Si un programa intenta acceder a una página que no está en la RAM, ocurre un fallo de página, en este caso, se busca la página en el disco y se copia a la RAM. Las páginas no necesitan ser consecutivas.