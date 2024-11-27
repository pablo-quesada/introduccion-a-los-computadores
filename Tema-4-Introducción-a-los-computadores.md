# Representación de datos

### Dígitos binarios
Los **dígitos binarios** son los números en base 2, que pueden mantenerse como señales electrónicas altas (unos) o señales electrónicas bajas (ceros). Se representan en colecciones que reciben el nombre de palabras en arquitecturas de 8, 16, 32 o 64 bits, que vienen limitadas por el hardware.

### Bit menos significativo o LSB (Least Significant Bit)
El **bit menos significativo** es el bit de más a la derecha en una palabra.

### Bit más significativo (Most Significant Bit)
El **bit más significativo** es el bit de más a la izquierda en una palabra.

### Número sin signo
En esta notación se emplea toda la palabra como mantisa.

### Número con signo
En esta notación se emplea el MSB para indicar si el número es negativo (1) o positivo (0).

### Número en complemento a 1

La notación de **complemento a 1** es un sistema de representación de números enteros con signo en binario.

- Representa el valor más negativo como `(11...111)` y el valor más positivo como `(01...111)`.
- Tiene dos ceros: uno positivo `(00...000)` y otro negativo `(11...111)`.
- Hay un número igual de valores positivos y negativos.

Para obtener el complemento a uno de un número binario:

1. Invertir los bits, cambiando `0` por `1` y `1` por `0`.

Esta notación es menos común en sistemas modernos debido a las complicaciones que introduce en operaciones aritméticas, como la necesidad de gestionar los dos ceros distintos.

### Número en complemento a 2

La notación de **complemento a 2** es un sistema de representación de números enteros con signo en sistemas binarios. En esta notación:

- El valor más negativo se representa como `(10...000)` y el valor más positivo como `(01...111)`.
- Se garantiza que hay un único cero, representado como `(00...000)`.
- Hay un número diferente de valores negativos y positivos, ya que el rango de los números negativos incluye uno más que el de los positivos.

Para calcular el complemento a dos de un número binario:

1. Invertir los bits (cambiar `0` por `1` y `1` por `0`).
2. Sumar `1` al bit menos significativo del resultado.

Este sistema es ampliamente utilizado en la mayoría de los sistemas modernos debido a su eficiencia para operaciones aritméticas.

### Operación de suma
En la **operación de suma** la aritmética se realiza bit a bit con un posible acarreo del cálculo de bits adyacentes menos significativos.
