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