# Representación de instrucciones

### Repertorio de instrucciones
El **repertorio de instrucciones** es el vocabulario de comandos entendidos por una arquitectura concreta.

### Palabra
Una **palabra** es la unidad natural de acceso en un computador; normalmente un grupo de 32 bits, equivalente a 4 bytes. En la arquitectura MIPS, una palabra corresponde al tamaño de un registro, y cada byte representa 8 bits.

### Registros
Los **registros** son las posiciones especiales construídas en hardware. Son limitados, en la arquitectura MIPS son de 32 bits.

### Instrucciones aritméticas
Las **instrucciones aritméticas** son comandos encargados de realizar operaciones aritméticas entre dos registros operandos.

### Instrucciones de transferencia de datos
Las **instrucciones de datos** son comandos que mueven datos entre memoria y registros.

### Dirección
La **dirección** es un valor que identifica la ubicación específica de un dato dentro de la memoria. Es esencial para acceder y manipular información almacenada en un sistema informático.

### Restricción de alineamiento
La **restricción de alineamiento** es una regla que exige que los datos se almacenen en direcciones de memoria que sean múltiplos de su tamaño natural. En la arquitectura MIPS, por ejemplo, las direcciones deben ser múltiplos de 4 para garantizar un acceso eficiente y correcto.

### Big Endian
Opción en la numeración de una palabra en la que el byte más a la derecha es el primero en la palabra.

### Little Endian
Opción en la numeración de una palabra en la que el byte más a la izquierda es el primero en la palabra.

### Formato de instrucción
El **formato de instrucción** es una forma de representación de una instrucción compuesta por campos de números binarios.

### Lenguaje máquina
El **lenguaje máquina** es la  representación binaria de las instrucciones usada para la comunicación dentro de un sistema informático.

## Algunas instrucciones en ensamblador

- `add`: Instrucción de suma entre dos registros que indica el operando destino.
- `subtract`: Instrucción de resta entre dos registros que indica el operando destino.
- `load word`: Instrucción que carga una palabra de la memoria a un registro. Instrucción de transferencia de datos.
- `store word`: Instrucción que guarda una palabra del registro en la memoria. Instrucción de transferencia de datos.
- `li`: Instrucción que carga en un registro una constante. También sirve para preparar llamadas al sistema. Instrucción de transferencia de datos.
- `la`: Instrucción que carga el contenido de las posiciones de memoria de una palabra. Instrucción de transferencia de datos.
- `syscall`: Instrucción encargada de llamar al sistema. Se trata de una interrupción. Las interrupciones son un mecanismo para recuperar el control de la CPU y atender otras solicitudes (procesos).
- `beq`: Instrucción que realiza un salto condicionado a un operando destino o etiqueta si dos operandos son iguales.
- `bne`: Instrucción que realiza un salto condicionado a un operando destino o etiqueta si dos operandos no son iguales.
- `j`: Instrucción de salto incondicional a un operando destino o etiqueta.
- `sll`: Instrucción encargada de desplazar un cierto número de bits un operando a la izquierda. Se puede emplear como instrucción para multiplicar. (Recordar que el número que pongamos se multiplicará por 4, y ese será el desplazamiento).


## Campos de una instrucción
Los **campos** de una instrucción son las partes individuales en las que se divide una instrucción en lenguaje máquina. Cada campo tiene un propósito específico y contiene información necesaria para que el procesador interprete y ejecute la instrucción correctamente. Estos campos incluyen datos como el tipo de operación a realizar, los registros involucrados, las direcciones de memoria, o valores constantes. La estructura y el tamaño de los campos varían según el formato de la instrucción y la arquitectura del procesador.

- `opcode`: El campo que indica la operación y el formato de una instrucción.
- `rs`: El registro del primer operando fuente.
- `rt`: El registro del segundo operando fuente.
- `rd`: El registro del operando destino, donde se almacena el resultado de la operación.
- `shamt`: La cantidad de desplazamientos (shift amount).
- `func`: Selecciona la variante específica de la operación en el campo `op` y a veces es llamado código de función.

### Instrucciones tipo R
Las **instrucciones tipo R** son aquellas que realizan operaciones aritméticas y lógicas. Estas instrucciones están compuestas por varios campos, cada uno con un propósito específico:

- `opcode`: 6 bits que indican la operación a realizar.
- `rs`: 5 bits que especifican el primer registro fuente.
- `rt`: 5 bits que especifican el segundo registro fuente.
- `rd`: 5 bits que indican el registro destino donde se almacenará el resultado.
- `shamt`: 5 bits que representan la cantidad de desplazamientos (shift amount).
- `funct`: 6 bits que seleccionan la variante específica de la operación definida por el `opcode`.

### Instrucciones tipo I

Las **instrucciones tipo I** son aquellas que se utilizan principalmente para operaciones de transferencia de datos y algunas operaciones aritméticas con constantes. Estas instrucciones están estructuradas en varios campos, cada uno con un propósito específico:

- `opcode`: 6 bits que indican la operación a realizar.
- `rs`: 5 bits que especifican el registro fuente.
- `rt`: 5 bits que especifican el registro destino.
- `inmediate`: 16 bits que contienen un valor constante o una dirección de memoria.

Este formato permite realizar operaciones como cargar o almacenar datos entre registros y memoria, así como realizar cálculos con valores inmediatos.

### Instrucciones tipo J

Las **instrucciones tipo J** son aquellas utilizadas para operaciones de salto sin condiciones. Se reservan 6 bits para el `opcode` y 26 bits para la dirección o etiqueta de destino.

### Contador de Programas
El **contador de programas** (PC) es el registro que contiene la dirección de la instrucción que está siendo ejecutada en el programa.

## Modos de direccionamiento

#### Direccionamiento inmediato
El **direccionamiento inmediato** se produce cuando el operando es una constante que aparece en la misma instrucción.

#### Direccionamiento a registro
El **direccionamiento a registro** se produce cuando el operando está en un registro.

#### Direccionamiento base o desplazamiento
El **direccionamiento base o desplazamiento** se produce cuando el operando está en la posición de memoria cuya dirección es la suma de un registro y de una constante en la instrucción.

#### Direccionamiento relativo al PC
El **direccionamiento relativo al PC** se produce cuando la dirección es la suma del PC y de una constante en la instrucción.

#### Direccionamiento pseudodirecto
El **direccionamiento pseudodirecto** se produce cuando la dirección de salto es los 26 bits de la instrucción concatenados con los bits de mayor peso del PC.

## Segmentos de memoria
El **segmento de memoria** es una división lógica de la memoria de un programa en diferentes áreas, cada una con un propósito específico. Estas divisiones permiten organizar y gestionar eficientemente el código, los datos y las estructuras necesarias para la ejecución del programa. Los segmentos principales incluyen:

- `Text-segment`: (segmento de texto) contiene el código máquina de un programa.
- `Data-segment`: (segmento de datos) contiene la representación binaria de los datos inicializados en el programa. 
- `Stack-segment`: (segmento de pila) es el espacio para manejar procedimientos. Maneja las llamadas a procedimientos y el almacenamiento temporal de datos.