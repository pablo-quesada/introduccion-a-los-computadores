# TIPOS DE POCESADORES

### 1.CPU
La **CPU (Central Processing Unit)** es el cerebro de la computadora, responsable de ejecutar instrucciones y procesar datos. Un ejemplo de CPU es el Intel Core i7, que se utiliza en computadoras personales y estaciones de trabajo para tareas como la edición de video, juegos y aplicaciones de productividad.

### 2.GPU
La **GPU (graphics processing unit/Unidad de procesamiento gráfico)** es un tipo de procesador mucho más potente y específico que se encarga del procesamiento gráfico con el fin de mejorar el rendimiento y aliviar la carga de la CPU. Un ejemplo de GPU es la NVIDIA GeForce RTX 3080, que se utiliza en computadoras personales para juegos y aplicaciones de gráficos intensivos. Además, las GPUs también se utilizan para GPGPU (General-Purpose computing on Graphics Processing Units), donde se aprovechan sus capacidades de procesamiento paralelo para tareas como el aprendizaje automático, simulaciones científicas y procesamiento de datos masivos.

### 3. SoC
El **SoC (system on chip/Sistema en un chip)** alberga distintos componentes dentro de un mismo chip, ya sea CPU, GPU, etc., con el fin de agrupar y realizar todas las funciones de un sistema completo en un mismo chip, comúnmente usado en móviles y dispositivos de tamaño reducido. Un ejemplo de SoC es el Apple A14 Bionic, que se utiliza en dispositivos como el iPhone 12 y el iPad Air (4ª generación). Ver también [Tema-1 SoC: System on a Chip](Tema-1-Introducción-a-los-computadores)

### 4. FPGA
El **FPGA (Field Programmable Gate Array/ Matriz de puertas lógicas programables en campo)** es un circuito integrado equipado con bloques lógicos configurables que se puede reprogramar después de haber sido fabricado. Un ejemplo de FPGA es el Xilinx Virtex-7, que se utiliza en aplicaciones como procesamiento de señales, telecomunicaciones y sistemas de control industrial.

### 5.ASIC
El **ASIC (Circuito Integrado de Aplicación Específica)** es un circuito integrado como el FPGA pero a diferencia de este no se puede reprogramar y fue creado para una tarea en específico; consiguiendo así un mayor rendimiento y eficiencia en dicha tarea. Un ejemplo de ASIC es el procesador de minería de Bitcoin, que se utiliza específicamente para realizar los cálculos necesarios en la minería de criptomonedas, logrando un rendimiento y eficiencia superiores en comparación con otros tipos de procesadores.

### 6.DSP
### 6. DSP
El **DSP (Digital Signal Processor/ Procesador de señales digitales)** es una CPU diseñada para procesar señales de audio y video principalmente, se utiliza para aplicaciones que requieran un procesamiento de las señales de alta velocidad. Un ejemplo de DSP es el Texas Instruments TMS320C6000, que se utiliza en aplicaciones como procesamiento de audio en tiempo real, comunicaciones digitales y sistemas de radar.

### 7. ACAP
EL **ACAP (Adaptative Computing Accelerator Platform/ )** Unidad de procesamiento adaptable creada para tareas de alta exigencia y flexibilidad. Esta formado por: __FPGA + DSP + CPU multicore + cores para Inteligencia Artificial__
 Un ejemplo de ACAP es el Xilinx Versal, que se utiliza en aplicaciones como redes 5G, centros de datos y procesamiento de inteligencia artificial.

# Conjuntos de Instrucciones

### ISA
La **ISA (Instruction Set Architecture)** es una interfaz abstracta entre el hardware y el nivel más bajo del software que incluye toda la información necesaria para escribir un programa en lenguake máquina que se ejecutará correctamente, e incluye las instrucciones, los registros, el acceso a la memoria, la E/S, etc.

### CISC
EL **CISC (Complex Instruction Set Computer)** se trata de una ISA con muchas instrucciones de distinto tamaño y formato, se puede acceder a la memoria desde cualquiera instrucción.

### RISC
El **RISC (Reduced Instruction Set Computer)*** es un tipo de ISA muy optimizado y pequeño que cuenta con instrucciones uniformes y del mismo tamaño, además solo se puede acceder a la memoria sólo con operaciones de carga y almacenamiento.

# Redimiento

### Tiempo de respuesta/ en ejecución/ de latencia
Es el tiempo transcurrido desde el comienzo y el final de un evento, se mide en segundos.

### Productividad/ throughput/ ancho de banda
Es la cantidad total de trabajo realizada en un tiempo determinado, medido en transacciones o tareas por hora.

### Tiempo transcurrido/ elapsed time/ response time/ wall clock time
Es el tiempo total de la ejecución de un programa, determina el rendimiento del sistema.

### Tiempo de CPU
Es el tiempo que una CPU emplea en una tarea determinada, se divide entre el tiempo de usuario y el tiempo del sistema.

### Periodo del reloj/ tiempo del ciclo
Es el tiempo que tarda en realizarse el ciclo de ese reloj; se mide en segundos o mas bien en fracciones de segundos, durante un ciclo la CPU puede realizar mas de una tarea básica y define la rapidez a la que la CPU puede procesasr instrucciones.

### Frecuencia de reloj
Es el número de ciclos que puede completar la CPU en un segundo y se mide en hercios (Hz). La frecuencia de reloj está directamente relacionada con el tiempo del ciclo, ya que el tiempo del ciclo es el inverso de la frecuencia de reloj. Por ejemplo, si una CPU tiene una frecuencia de reloj de 2 GHz (gigahercios), el tiempo del ciclo sería 0.5 nanosegundos (1 / 2 GHz).

### SPEC CPU BENCHMARKS
Los **Benchmarks o tests de rendimiento** son un conjunto de programas que ejecutan tareas para medir el rendimiento de un computador, dispositivo o sistema. Un ejemplo común de benchmarks es SPEC (Standard Performance Evaluation Corporation), una organización que desarrolla y mantiene un conjunto de benchmarks estandarizados para evaluar el rendimiento de sistemas informáticos. Los benchmarks de SPEC son ampliamente utilizados en la industria para comparar el rendimiento de diferentes sistemas y arquitecturas.

### Ley de Amdahl
Esta ley nos dice que la posible mejora del rendimiento está limitada por la porción en que se utilice la prestación mejorada. En otras palabras, si solo una parte del sistema se mejora, el impacto total en el rendimiento global estará limitado por la fracción del tiempo que esa parte mejorada es utilizada.
