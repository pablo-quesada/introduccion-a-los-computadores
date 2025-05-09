# TIPOS DE POCESADORES

### 1.CPU
La **CPU (Central Processing Unit)** es el cerebro de la computadora, responsable de ejecutar instrucciones y procesar datos. Un ejemplo de CPU es el Intel Core i7, que se utiliza en computadoras personales y estaciones de trabajo para tareas como la edición de video, juegos y aplicaciones de productividad.

### 2.GPU
La **GPU (graphics processing unit/Unidad de procesamiento gráfico)** es un tipo de procesador mucho más potente y específico que se encarga del procesamiento gráfico con el fin de mejorar el rendimiento y aliviar la carga de la CPU. Un ejemplo de GPU es la NVIDIA GeForce RTX 3080, que se utiliza en computadoras personales para juegos y aplicaciones de gráficos intensivos. Además, las GPUs también se utilizan para GPGPU (General-Purpose computing on Graphics Processing Units), donde se aprovechan sus capacidades de procesamiento paralelo para tareas como el aprendizaje automático, simulaciones científicas y procesamiento de datos masivos.

### 3. SoC
El **SoC (system on chip/Sistema en un chip)** alberga distintos componentes dentro de un mismo chip, ya sea CPU, GPU, etc., con el fin de agrupar y realizar todas las funciones de un sistema completo en un mismo chip, comúnmente usado en móviles y dispositivos de tamaño reducido. Un ejemplo de SoC es el Apple A14 Bionic, que se utiliza en dispositivos como el iPhone 12 y el iPad Air (4ª generación). Ver también [Tema-1 SoC: System on a Chip](Tema-1-Introducción-a-los-computadores)

### 4. FPGA
El **FPGA (Field Programmable Gate Array/Matriz de Puertas Lógicas Programables en Campo)** es un circuito integrado que contiene bloques lógicos configurables y una red de interconexión programable, lo que permite su reconfiguración incluso después de haber sido fabricado. Esta flexibilidad lo hace ideal para una amplia gama de aplicaciones, desde prototipos de hardware hasta sistemas de producción. Un ejemplo destacado de FPGA es el Xilinx Virtex-7, utilizado en áreas como el procesamiento de señales digitales, telecomunicaciones, sistemas de control industrial y aceleración de algoritmos en inteligencia artificial. Los FPGAs son especialmente valiosos en entornos donde se requiere alta personalización y rendimiento en tiempo real.

### 5. ASIC
El **ASIC (Application-Specific Integrated Circuit/Circuito Integrado de Aplicación Específica)** es un tipo de circuito integrado diseñado específicamente para realizar una tarea concreta, lo que lo diferencia de los FPGA, que son reprogramables. Al estar optimizado exclusivamente para su propósito, los ASICs ofrecen un rendimiento y eficiencia superiores en comparación con otros tipos de procesadores. Un ejemplo destacado de ASIC es el procesador de minería de Bitcoin, diseñado exclusivamente para realizar los cálculos intensivos necesarios en la minería de criptomonedas, logrando una eficiencia energética y un rendimiento significativamente mayores que los procesadores de propósito general.

### 6. DSP
El **DSP (Digital Signal Processor/Procesador de Señales Digitales)** es un tipo de procesador especializado en el procesamiento eficiente de señales digitales, como audio, video y datos provenientes de sensores. Estos procesadores están diseñados para realizar cálculos matemáticos complejos a alta velocidad, lo que los hace ideales para aplicaciones que requieren procesamiento en tiempo real. Un ejemplo destacado de DSP es el Texas Instruments TMS320C6000, ampliamente utilizado en áreas como procesamiento de audio en tiempo real, comunicaciones digitales, sistemas de radar, y dispositivos médicos. Los DSPs también son fundamentales en tecnologías modernas como la cancelación de ruido activa, la compresión de datos multimedia y el análisis de señales en sistemas de monitoreo industrial.

### 7. ACAP
EL **ACAP (Adaptative Computing Accelerator Platform/ )** Unidad de procesamiento adaptable creada para tareas de alta exigencia y flexibilidad. Esta formado por: __FPGA + DSP + CPU multicore + cores para Inteligencia Artificial__
 Un ejemplo de ACAP es el Xilinx Versal, que se utiliza en aplicaciones como redes 5G, centros de datos y procesamiento de inteligencia artificial.

# Conjuntos de Instrucciones

### ISA
La **ISA (Instruction Set Architecture)** es una interfaz abstracta que define cómo el software interactúa con el hardware. Incluye un conjunto de instrucciones, registros, modos de direccionamiento, acceso a la memoria, entrada/salida (E/S) y otros aspectos esenciales para que un programa en lenguaje máquina se ejecute correctamente en un procesador específico. La ISA actúa como un puente entre el diseño del hardware y el desarrollo de software, proporcionando una base común que permite la compatibilidad y optimización entre ambos. Ejemplos de arquitecturas de conjunto de instrucciones incluyen x86, ARM, RISC-V y MIPS, cada una con características y aplicaciones específicas.

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

# Tipos de sistemas operativos

## En base al número de usuarios

### Sistemas operativos de un solo usuario (monousuarios)
Ejecutan programas de un solo usuario, y solo uno a la vez a través de una máquina virtual conceptual la que los programas son ejecutados como si fuesen los únicos aprovechando los recursos del hardware. Este es el caso de MS-DOS. Algunos sistemas monousuarios como Microsoft Windows(95 a 10) y sistemas operativos integrados más pequeños (embebidos) como uCos y VxWorks permiten ejecutar múltiples programas del mismo usuario (multitarea).

### Sistemas operativos multiusuario
Permiten que varios usuarios accedan simultáneamente a los recursos de un sistema, cada uno dentro de un entorno seguro e independieente (máquina virtual). Una ventaja clave de los sistemas multiusuarios es la gestión avanzada de permisos, lo que garantiza que los usuarios solo puedan acceder a los archivos y recursos que se les han asignado. Además, los sistemas multiusuario, como los basados en Linux o MacOS, facilitan el desarrollo colaborativo en plataformas de programación y servidores de aplicaciones, permitiendo que varios desarrolladores trabajen en parelelo en proyectos sin riesgo de conflicto entre procesos. Un caso actual es del Amazon Web Services (AWS) o Google Cloud Platform (GCP), donde múltiples usuarios y empresas utilizan los mismos servidores físicos de manera concurrente, aislados entre sí mediante máquinas virtuales o contenedores, lo que garantiza la seguridad y escalabilidad de los servicios.

## En base al sistema que tienen que gestionar

### Sistemas operativos de mainframe
Están diseñados para proporcionar servicios a múltiples usuarios remotos de manera concurrente. Estos sistemas gestionan los recursos de red y facilitan la comunicación entre las aplicaciones de usuario, llamadas clientes, y los servicios que ofrecen los servidores, garantizando un flujo eficiente de datos y solicitudes. Los sistemas operativos de servidor están optimizados para manejar peticiones de diversos
clientes, ofreciendo servicios esenciales como almacenamiento de archivos, alojamiento web y soporte de aplicaciones. La arquitectura de estos sistemas permite la compartición efectiva de recursos hardware y software; por ejemplo, un único servidor puede alojar múltiples sitios web, permitiendo que diferentes organizaciones utilicen el mismo hardware físico. Además, los sistemas operativos de servidor implementan robustos mecanismos de seguridad y gestión de acceso, asegurando que solo usuarios autorizados puedan interactuar con los recursos, lo que es esencial en escenarios empresariales donde la integridad y la confidencialidad de los datos son primordiales.

### Sistemas operativos de servidor
Están diseñados para proporcionar servicios a múltiples usuarios remotos de manera concurrente. Estos sistemas gestionan los recursos de red y facilitan la comunicación entre las aplicaciones de usuario, llamadas clientes, y los servicios que ofrecen los servidores, garantizando un flujo eficiente de datos y solicitudes. Los sistemas operativos de servidor están optimizados para manejar peticiones de diversos clientes, ofreciendo servicios esenciales como almacenamiento de archivos, alojamiento web y soporte de aplicaciones. La arquitectura de estos sistemas permite la compartición efectiva de recursos hardware y software; por ejemplo, un único servidor puede alojar múltiples sitios web, permitiendo que diferentes organizaciones utilicen el mismo hardware físico. Además, los sistemas operativos de servidor implementan robustos mecanismos de seguridad y gestión de acceso, asegurando que solo usuarios autorizados puedan interactuar con los recursos, lo que es esencial en escenarios empresariales donde la integridad y la
confidencialidad de los datos son primordiales.

### Sistemas operativos de ordenadores personales
Están diseñados para respaldar a los usuarios individuales mediante la gestión eficiente de múltiples aplicaciones de forma simultánea, un concepto conocido como multitarea. Estos sistemas se centran en proporcionar un entorno receptivo y amigable, permitiendo a los usuarios ejecutar varias aplicaciones a la vez, como procesadores de texto, navegadores web y videojuegos. Además, estos sistemas operativos suelen incluir interfaces gráficas (GUI) intuitivas y herramientas de personalización que mejoran aún más la interactividad y la accesibilidad, permitiendo a los usuarios adaptar sus entornos de trabajo según sus preferencias y necesidades específicas.

### Sistemas operativos de ordenadores personales móviles
Están diseñados específicamente para gestionar el hardware y las funcionalidades únicas de dispositivos móviles, como teléfonos móviles y tablets. Estos sistemas operativos son responsables de llevar a cabo diversas tareas, que incluyen llamadas telefónicas, navegación por GPS, gestión de sensores y protocolos de comunicación. Además, permiten la instalación de aplicaciones de terceros, lo que capacita a los usuarios para personalizar sus dispositivos con una amplia
gama de opciones de software que mejoran tanto la funcionalidad como la experiencia del usuario. Asimismo, los sistemas operativos móviles deben optimizar el uso de recursos limitados, garantizando un rendimiento eficiente y una gestión eficaz de la batería.

### Sistemas operativos para nodos-sensores
Están diseñados para gestionar redes de dispositivos con pocos recursos hardware, comúnmente utilizados en aplicaciones de Internet de las Cosas (IoT). Estos sistemas se centran en la recopilación, el envío y el almacenamiento de información procedente de diversos sensores desplegados en distintos
entornos. Su funcionamiento debe ser altamente eficiente, dado que operan bajo las limitaciones de un procesamiento restringido, escasa memoria y disponibilidad limitada de energía. En un contexto de ciudad inteligente, estos sistemas pueden integrar datos de
sensores de tráfico, calidad del aire y consumo de energía, proporcionando información valiosa para la planificación urbana y la sostenibilidad.

### Sistemas operativos en tiempo real
Están diseñados para gestionar tareas críticas que requieren procesamiento y respuestas inmediatas. Estos sistemas se clasifican en dos
tipos: sistemas de tiempo real duro (hard real-time) y sistemas de tiempo real suave (soft real-time). Los sistemas de tiempo real duros se utilizan en aplicaciones de misión crítica donde el tiempo es fundamental, y cualquier retraso podría tener consecuencias catastróficas, como en dispositivos médicos, sistemas aeroespaciales y automatización industrial. Estos sistemas garantizan que las tareas críticas se completen dentro de estrictas limitaciones temporales. Por otro lado, los sistemas de tiempo real suaves manejan tareas en las que los plazos son importantes, pero no se aplican de manera tan estricta. En estos entornos, las tareas pueden experimentar retrasos ocasionales sin repercusiones significativas, lo que los hace adecuados para aplicaciones como el procesamiento multimedia y las telecomunicaciones, donde las respuestas oportunas mejoran elrendimiento sin comprometer la seguridad.

### Sistemas operativos embebidos
Están diseñados para gestionar dispositivos concretos,como televisores, cámaras, drones y una variedad de otros electrodomésticos inteligentes optimizando el uso del hardware en el que se ejecutan y proporcionando un entorno de computación ligero y eficiente. Una característica significativa de los sistemas operativos embebidos es que, por lo general, no ejecutan software de terceros, lo que aumenta su seguridad y fiabilidad, convirtiéndolos en opciones ideales para aplicaciones críticas en electrónica de consumo y dispositivos industriales. Además, los sistemas operativos embebidos suelen incorporar un diseño de tiempo real (RTOS, por sus siglas en inglés), que permite responder a eventos o condiciones externas en un plazo estricto. Esta capacidad es fundamental en sistemas de control de vehículos autónomos o en dispositivos médicos que requieren monitorización y respuesta inmediata. A medida que la Internet de las Cosas (IoT)continúa creciendo, la importancia de los sistemas operativos embebidos se incrementa.

### Sistemas operativos diseñados para tarjetas inteligentes
Gestionan operaciones específicas, a menudo centrándose en un conjunto limitado de funcionalidades. Estos sistemas facilitan operaciones como el procesamiento seguro de pagos, la verificación de identidad y el control de acceso, normalmente asociados con tarjetas de crédito y tarjetas de identificación. Los sistemas operativos de tarjetas inteligentes están diseñados para manejar protocolos de seguridad y cifrado, asegurando que la información sensible esté protegida durante las transacciones. Al optimizar las operaciones para casos de uso particulares, estos sistemas operativos proporcionan funcionalidad segura y confiable, al tiempo que mantienen la simplicidad y eficiencia necesarias para su uso efectivo en aplicaciones cotidianas.