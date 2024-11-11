# Representación de datos

### Dígitos binarios
Los **dígitos binarios** son los números en base 2, que pueden mantenerse como señales electrónicas altas (unos) o señales electrónicas bajas (ceros). Se representan en colecciones que reciben el nombre de bits en arquitecturas de 8, 16, 32 o 64 bits, que vienen limitadas por el hardware.

### Bit menos significativo o LSB (Least Significant Bit)
El **bit menos significativo** es el bit de más a la derecha en una palabra MIPS.

### Bit más significativo (Most Significant Bit)
El **bit más significativo** es el bit de más a la izquierda en una palabra MIPS.

### Número sin signo
En esta notación se emplea toda la palabra como mantisa.

### Número con signo
En esta notación se emplea el MSB para indicar si el número es negativo (1) o positivo (0).

### Número en complemento a 1
Notación que representa el valor más negativo con (10...000)dos y el valor positivo con (01...11)dos con igual número de valores positivos y negativos pero con dos ceros, uno positivo (00...00)dos y otro negativo (11...11)dos. Este término se utiliza también para la inversión de los bits de una secuencia de bits: cambiar 0 por 1 y 1 por 0.

### Número en complemento a 2
Notación que representa el valor más negativo con (10...000)dos y el valor positivo con (01...11)dos con igual número de valores positivos y negativos pero con dos ceros, uno positivo (00...00)dos y otro negativo (11...11)dos. Este término se utiliza también para la inversión de los bits de una secuencia de bits: cambiar 0 por 1 y 1 por 0, y sumar 1 al bit menos significativo. Actualmente se usa esta representación para la mayoría de los sistemas.

### Operación de suma
En la **operación de suma** la aritmética se realiza bit a bit con un posible acarreo del cálculo de bits adyacentes menos significativos.
