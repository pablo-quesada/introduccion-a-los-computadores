# Representación de instrucciones

### Repertorio de instrucciones
El **repertorio de instrucciones** es el vocabulario de comandos entendidos por una arquitectura concreta.

### Palabra
Una **palabra** es la unidad natural de acceso en un computador; normalmente un grupo de 32 bits; corresponde al tamaño de un registro en la arquitectura MIPS.

### Registros
Los **registros** son las posiciones especiales construídas en hardware. Son limitados, en la arquitectura MIPS son de 32 bits.

### Instrucciones aritméticas
Las **instrucciones aritméticas** son comandos encargados de realizar operaciones aritméticas entre dos registros operandos.

### Instrucciones de transferencia de datos
Las **instrucciones de datos** son comandos que mueven datos entre memoria y registros.

### Dirección
La **dirección** es valor usado para señalar la posición de un elemento de datos específico dentro de una memoria.

### Restricción de alineamiento
La **restricción de alineamiento** es el requisito de que los datos se alineen en memoria en límites naturales. En la arquitectura MIPS las direcciones deben ser múltiplos de 4.

### Array
Los **arrays** son estructuras de datos más complejas que las variables simples. (Similares a las listas en python, pero cuando se llama a una posición de memoria en un array se debe recordar que por la restricción de alineamiento son múltiplos de 4, siendo la primera el 0 y la segunda 4).

### Big Endian
Opción en la numeración de una palabra en la que el byte más a la derecha es el primero en la palabra.

### Little Endian
Opción en la numeración de una palabra en la que el byte más a la izquierda es el primero en la palabra.

### Formato de instrucción
El **formato de instrucción** es una forma de representación de una instrucción compuesta por campos de números binarios.

### Lenguaje máquina
El **lenguaje máquina** es la  representación binaria de las instrucciones usada para la comunicación dentro de un sistema informático.

### add
Instrucción de suma entre dos registros que indica el operando destino.

### subtract
Instrucción de resta entre dos registros que indica el operando destino.

### load word
Instrucción que carga una palabra de la memoria a un registro. Instrucción de transferencia de datos.

### store word
Instrucción que guarda una palabra del registro en la memoria.Instrucción de transferencia de datos.

### li
Instrucción que carga en un registro una constante. También sirve para preparar llamadas al systema. Instrucción de transferencia de datos.

### la 
Instrucción que carga el contenido de las posiciones de memoria de una palabra. Instrucción de transferencia de datos.

### syscall
Instrucción encargada de llamar al sistema. Se trata de una interrupción. Las interrupciones son un mecanismo para recuperar el control de la CPU y atender otras solicitudes (procesos).

### beq
Instrucción que realiza un salto condicionado a un operando destino o etiqueta si dos operandos son iguales.

### bne
Instrucción que realiza un salto condicionado a un operando destino o etiqueta si dos operandos no son iguales.

### j
Instrucción de salto incondicional a un operando destino o etiqueta.

### sll
Instrucción encargada de desplazar un cierto número de bits un operando a la izquierda. Se puede emplear como instrucción para multiplicar. (Recordar que el número que pongamos se multiplicará por 4, y ese será el desplazamiento)

### Campo
Los **campos** son segmentos de instrucción.

#### opcode
El **opcode** es el campo que indica la operación y el formato de una instrucción.

#### rs
El **rs** es el registro del primer operando fuente.

#### rt
El **rt** es el registro del segundo operando fuente.

#### rd
El **rd** es el registro del operando destino, donde se almacena el resultado de la
operación.

#### shamt
El **shamt** es la cantidad de desplazamientos (shift amount). 

#### func
La **func** (función) Sselecciona la variante específica de la operación en el campo op y a veces es llamado código de función.

### Instrucciones tipo R
Las **instrucciones tipo R** son las operaciones aritmético y lógicas. En ellas se reservan seis bits al opcode, 5 al rs, 5 al rt, 5 al rd, 5 al shamt y 6 a funct.

### Instrucciones tipo I
Las **instrucciones tipo I** son las operaciones de transferencia de datos. En ellas se reservan seis bits al opcode, 5 al rs, 5 al rt y 16 a la dirección.

### Instrucciones tipo J
Las **Instrucciones tipo J** son las operaciones de salto. En las de salto incondicional se reservan 6 bits para el opcode y 26 para la dirección o etiqueta.
En las de salto condicional se reservan seis bits al opcode, 5 al rs, 5 al rt y 16 a la dirección.

### Contador de Programas
El **contador de programas** (PC) es el registro que contiene la dirección de la instrucción que está siendo ejecutada en el programa.

### Modos de direccionamiento

#### Direccionamiento inmediato
El **direccionamiento inmediato** se produce cuando el operando es una constante que aparece en la misma instrucción. (Tipo R con constante).

#### Direccionamiento a registro
El **direccionamiento a registro** se produce cuando el operando está en un registro. (Tipo R con variables).

#### Direccionamiento base o desplazamiento
El **direccionamiento base o desplazamiento** se produce cuando el operando está en la posición de memoria cuya dirección es la suma de un registro y de una constante en la instrucción. (Tipo I).

#### Direccionamiento relativo al PC
El **direccionamiento relativo al PC** se produce cuando la dirección es la suma del PC y de una constante en la instrucción. (Tipo J condicional).

#### Direccionamiento pseudodirecto
El **direccionamiento pseudodirecto** se produce cuando la dirección de salto es los 26 bits de la instrucción concatenados con los bits de mayor peso del PC. (Tipo J incondicional).

### Text-segment
El **text-segment** (segmento de texto) contiene el código máquina de un programa.

### Data-segment
El **data-segment** (segmento de datos) contiene la representación binaria de los datos inicializados en el programa.

### Stack-segment
El **stack-segment** (segmento de pila) es el espacio para manejar procedimientos.
