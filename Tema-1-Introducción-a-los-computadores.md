# Componentes hardware de un computador

### CPU: Unidad Central de Proceso
La **CPU (Central Processing Unit)** es el cerebro de la computadora, responsable de ejecutar instrucciones y procesar datos. 

### RAM: Random Access Memory
La **RAM (Memoria de Acceso Aleatorio)** es una memoria volátil de alta velocidad que almacena temporalmente los datos y programas que la CPU necesita acceder rápidamente. Cuanta más RAM tenga un sistema, mejor será su capacidad para manejar múltiples tareas.

### HDD: Hard Disk Drive
El **HDD (Disco Duro)** es un dispositivo de almacenamiento magnético que utiliza discos giratorios y un cabezal lector/escritor para almacenar datos. Aunque es más lento y menos resistente que los SSD, los HDD suelen ofrecer mayor capacidad de almacenamiento a un costo más bajo.

### SSD: Solid State Disk
El **SSD (Disco de Estado Sólido)** es un dispositivo de almacenamiento que utiliza memoria flash en lugar de discos giratorios, como los discos duros tradicionales. Es más rápido, silencioso y resistente a golpes, mejorando significativamente el rendimiento del sistema.

### Chip
Un **chip** es una pequeña pieza de material semiconductor (generalmente silicio) que contiene circuitos electrónicos. Los chips son la base de todos los dispositivos electrónicos modernos, desde computadoras hasta teléfonos móviles.

### Circuito Integrado
Un **circuito integrado** es un conjunto de componentes electrónicos, como transistores y resistencias, miniaturizados en una pequeña placa de material semiconductor. Se utilizan en una amplia variedad de dispositivos, desde computadoras hasta electrodomésticos, y son fundamentales en la electrónica moderna.

### SoC: System on a Chip
El **SoC (System on a Chip)** es un circuito integrado que combina en un solo chip múltiples componentes esenciales de un sistema, como la CPU, GPU, memoria, y controladores de entrada/salida. Los SoC son comunes en dispositivos móviles, tablets y otros sistemas embebidos, proporcionando eficiencia energética y ahorro de espacio.

# Tecnología para construir computadores

### Válvula de vacío
La **válvula de vacío** es un tubo de vidrio hueco entre 5 y 10 cm de longitud en el cual se ha eliminado la mayor cantidad de aire posible, que usa un haz de electrones para transferir datos.

### Transistores
Los **transistores** son dispositivos electrónicos semiconductores que actúan como interruptores o amplificadores de señales eléctricas. Son los componentes fundamentales en la construcción de circuitos integrados y procesadores, permitiendo el control del flujo de corriente en los chips.

### Obleas (Blank Wafers y Pattern Wafers)
La **oblea (wafer)** es una fina lámina circular de material semiconductor, generalmente silicio, de grosor no mayor que 0,25cm, utilizadas como base para la fabricación de chips. 
- **Blank wafers** son obleas sin ningún patrón, listas para el proceso de fabricación.
- **Pattern wafers** son obleas que ya han pasado por procesos de fotolitografía y tienen los patrones de circuitos necesarios para crear chips.

### Dies
Los **dies** son pequeñas piezas individuales que se cortan de una oblea procesada. Cada die contiene un circuito funcional, como una CPU o un módulo de memoria, y es esencialmente el chip sin empaquetar listo para ser probado y encapsulado.

### Chip Empaquetado
Un **chip empaquetado** es un die que ha sido encapsulado en un paquete protector, que incluye conectores para la comunicación con otros componentes. El empaquetado protege el die de daños físicos y ambientales y facilita su integración en sistemas electrónicos.

# Lenguaje de alto nivel y lenguaje máquina

### Código binario
El **código binario** es un lenguaje de programación fornado por unos y ceros. Estos unos y ceros representan también las señales eléctricas de "on" y "off" respectivamente 

### Palabras
Una **palabra** es una unidad natural de acceso en un computador, normalmente un grupo de 32 bits, que se corresponde al tamaño de un registro en la arquitectura MIPS, que es una arquitectura de conjunto de instrucciones ISA.

### Repertorio de instrucciones
El **repertorio de instrucciones** es el conjunto de palabras que contienen las instrucciones en forma de bits.

# Almacenamiento de datos e instrucciones

### Registros de procesador
Los **registros** son un número limitado de posiciones especiales en las que se sitúan las instrucciones aritméticas.

### Memoria caché
La **memoria caché** es una memoria rápida y pequeña que actúa como un *búfer*(espacio de memoria en el que se almacenan datos de manera temporal) para otra memoria mayor y más lenta.

## Memoria principal
La **memoria principal** es la memoria volátil (que solo guarda los datos cuando está recibiendo señal eléctrica) que se usa para almacenar los programas cuando se están ejecutando; típicamente se compone de DRAM (memoria construida como un circuito integrado, que provee acceso aleatorio a cualquier posición) en los computadores actuales

### Memoria secundaria
La **memoria secundaria** es una memoria no volátil (forma de memoria que guarda los datos incluso en ausencia de alimentación eléctrica y que se usa para almacenar los programas entre ejecuciones) usada para almacenar los programas y datos entre ejecuciones; típicamente se compone de disicos magnéticos en los computadores actuales.

# Sistemas operativos

### Sistema operativo
El **sistema operativo** es el programa principal que se ejecuta en una computadora. Es responsable de administrar los recursos del sistema, como la memoria, el procesador y los dispositivos de entrada/salida. Además, proporciona una interfaz para que los usuarios interactúen con la computadora y ejecuten aplicaciones.

### Rol del sistema operativo 
Algunos de los **roles del sistema operativo** son la gestión de recursos externos e internos, la gestión de la memoria principal y del almacenamiento secundario, así como del tiempo de CPU en la multitarea, la ejecución de las máquinas virtuales y la protección y gestión de errores.

# Comunicación entre computadores

### Columna de la era PostPC

### Redes de área local (LAN) y de área ancha (WAN)
La **Red de ára local** es una red diseñada para transportar datos en un área confinada geográficamente, típicamente dentro de un mismo edificio. La **Red de área extensa** es una red que se extiende a lo largo de cientos de kilómetros y que puede abarcar un continente.

### Redes con cable e inalámbricas

### Computación en la nube

### Comunicación y conexión entre procesadores

# Arquitectura de computadores

### Ley de Moore
La **Ley de Moore** es una observación empírica que indica que el número de transistores en un circuito integrado tiende a duplicarse aproximadamente cada dos años. Esta tendencia ha impulsado el avance tecnológico en la industria de los computadores durante décadas.

### Paralelismo
El **paralelismo** es una técnica que consiste en diseñar una aplicación para que realice diferentes tareas en paralelo, utilizando múltiples procesadores o nodos. Esto permite acelerar el proceso y mejorar la eficiencia del sistema.

### Pipelining
El **pipelining** es una técnica de implementación que consiste en solapar la ejecución de múltiples instrucciones. Esta técnica divide el proceso de ejecución de una instrucción en varias etapas, permitiendo que múltiples instrucciones se ejecuten simultáneamente en diferentes etapas del pipeline. Esto mejora el rendimiento del procesador al aprovechar mejor los recursos y reducir el tiempo de ejecución de las instrucciones.

### Predicción
La **predicción** consiste en suponer un resultado para un salto antes de que se establezca el resultado real. Este enfoque permite proceder a partir de esa suposición en lugar de esperar a que se establezca el resultado real. 

### Jerarquía de memoria
La **jerarquía de memoria** es una estructura que utiliza varios niveles de memoria. A medida que nos alejamos de la CPU, el tamaño de las memorias y el tiempo de acceso aumentan. En la parte superior de la jerarquía se encuentra la memoria caché, que es pequeña pero muy rápida. A continuación, se encuentra la memoria principal (RAM), que es más grande pero más lenta. Por último, en la parte inferior de la jerarquía, se encuentra la memoria secundaria (como los discos duros), que tiene una capacidad mucho mayor pero es aún más lenta. Esta jerarquía permite optimizar el rendimiento del sistema al almacenar los datos más utilizados en las memorias más rápidas y acceder a los datos menos utilizados en las memorias más lentas.

### Hacer el caso común más rápido
Dado que la ley de Andahl nos dice que la oportunidad para conseguir una mejora se ve afectada por el tiempo que este suceso consume, es más beneficioso enfocarse en hacer más rápido el caso más frecuente. Al optimizar el rendimiento del caso más común, se logra una mejora más significativa y eficiente en comparación con mejorar un proceso poco frecuente.

### Usar abstracción para simplificar el diseño
La **abstracción** es un modelo que oculta temporalmente los detalles de menor nivel de los sistenas de computadores para facilitar el diseño de sistemas sofisticados.

### Confiabilidad a través de la redundancia
La **redundancia** consiste en la implementación de un número muy elevado de componentes pequeños en lugar de un número menor de los mismos de mayor tamaño para disminuir las posibilidades de que estos tengan errores. Al tener múltiples componentes realizando la misma función, si uno de ellos falla, los demás pueden tomar su lugar y mantener el funcionamiento del sistema. Esto aumenta la confiabilidad y la disponibilidad del sistema, aunque también puede aumentar los costos y la complejidad del diseño.
