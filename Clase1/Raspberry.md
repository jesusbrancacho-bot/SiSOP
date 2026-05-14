# Raspberry Pi

## 🧠 IDEA CLAVE 1: ¿Qué es una Raspberry Pi?

❓ ¿Qué es?
Una Raspberry Pi es una **microcomputadora** del tamaño de una tarjeta de crédito.
Es una computadora completa, pero pequeña y de bajo costo.
Según el material, ha tenido un crecimiento enorme en ventas, superando los 46 millones de unidades en 2022 .

❓ ¿Por qué existe?
Fue creada para:
- Enseñar programación
- Democratizar el acceso a la computación
- Permitir proyectos electrónicos y educativos a bajo costo.

En 2017 ganó el premio MacRobert por redefinir cómo las personas interactúan con la computación .

## 🧠 IDEA CLAVE 2: ¿Cómo es físicamente?

❓ ¿Qué componentes tiene?

En la diapositiva de hardware (pág. 13) se muestra su estructura básica :
- CPU / GPU
- RAM
- Puertos USB
- Ethernet
- I/O (entrada/salida)

En otras palabras: Es una PC miniatura.

❓ ¿Cómo funciona?
Funciona como cualquier computadora:
1. La CPU ejecuta instrucciones
2. La RAM guarda datos temporales
3. El almacenamiento (microSD) guarda el sistema operativo
4. Los dispositivos USB permiten conectar teclado, mouse, etc.

Ejemplo sencillo:
Si instalas Linux y conectas un teclado y monitor, puedes usala como una PC normal.

🧠 IDEA CLAVE 3: ¿Cuáles son sus modelos principales?

🔹 Raspberry Pi 1 Model B
    CPU: ARM 700 MHz
    RAM: 512 MB
    Ethernet 10/100
    USB 2.0
    Básica, pensada para educación.

🔹 Raspberry Pi 2 Model B
    CPU: Cortex-A7, quad-core
    RAM: 1 GB
    Ya permitía multitarea más fluida.

🔹 Raspberry Pi 3 Model B
    CPU: Cortex-A53, 64-bit
    Incluye WiFi y Bluetooth
    Aquí empieza a parecerse más a una PC moderna.

🔹 Raspberry Pi 4
    CPU: Cortex-A72, 64-bit
    Hasta 8 GB RAM
    USB 3.0
    2 HDMI
    Ya puede usarse como computadora de escritorio básica.

🔹 Raspberry Pi 5
    CPU: Cortex-A76, 2.4 GHz
    Hasta 8 GB RAM
    Ethernet Gigabit
    Mucho más potente.


🔹 Raspberry Pi Pico
    Aquí cambia el concepto.
    No es una computadora completa.
    Es un microcontrolador para computación física .
    
    Sirve para:
    - Sensores
    - Actuadores
    - Robótica
    
    Ejemplo:
    Encender luces automáticamente cuando detecta movimiento.


## 🧠 IDEA CLAVE 4: ¿Qué sistema operativo usa?

Principalmente usa:
- Raspberry Pi OS (basado en Debian Linux)

Pero puede usar muchos otros sistemas:

Linux-based:
- Ubuntu
- Fedora
- Gentoo
- Kali Linux

No Linux-based:
- FreeBSD
- Windows 10 IoT Core
- RISC OS


❓ ¿Por qué es importante esto en Sistemas Operativos?

Porque demuestra:
- Arquitectura ARM
- Compatibilidad multiplataforma
- Adaptación de kernels
- Gestión de recursos en hardware limitado


#### 🧠 IDEA CLAVE 5: ¿Para qué se usa?

❓ ¿Dónde se usa?
Ejemplos del documento:
- Impresión 3D con AstroPrint
- Acceso remoto con RealVNC
- Minecraft educativo
- Rover de la NASA
- Clusters para probar programas de supercomputadoras

❓ ¿Cómo puede usarse en Sistemas Operativos?

Ejemplos académicos:
- Laboratorio de kernel Linux
- Experimentos de planificación de procesos
- Sistemas embebidos
- Servidor web casero
- Firewall
- Nodo de red

#### 🧠 IDEA CLAVE 6: ¿Cuál es su importancia real?
❓ ¿Por qué es tan relevante?
Porque combina:
- Bajo costo
- Bajo consumo energético
- Arquitectura ARM
- Ecosistema Linux

Permite experimentar sin riesgo.



--- 

# 🧠 Arquitectura ARM

## ❓ ¿Qué es ARM?

ARM es un tipo de **arquitectura de procesador**.

Es decir, es la forma en que está diseñado el CPU internamente.

No todos los procesadores son iguales. Existen principalmente:

- **x86** (Intel, AMD – PCs tradicionales)
- **ARM** (Raspberry Pi, celulares, tablets)

---

## ❓ ¿Cómo es ARM?

ARM está basado en el modelo:

> RISC (Reduced Instruction Set Computer)

Eso significa:

- Instrucciones más simples  
- Menor consumo energético  
- Mayor eficiencia por watt  

### 🧩 Ejemplo sencillo

Un procesador **x86** es como una navaja suiza con 100 herramientas.  
Un procesador **ARM** es como un kit optimizado con pocas herramientas, pero muy rápidas.

---

## ❓ ¿Por qué Raspberry Pi usa ARM?

Porque:

- Consume poca energía
- Genera menos calor
- Es más barato
- Es ideal para sistemas embebidos

Modelos como Raspberry Pi 3, 4 y 5 usan CPUs ARM Cortex (A53, A72, A76).

---

## ❓ ¿Por qué es importante en Sistemas Operativos?

Porque el sistema operativo debe:

- Compilarse específicamente para ARM
- Manejar su conjunto de instrucciones
- Adaptarse a su gestión de memoria

No puedes instalar un Windows tradicional (x86) en una Raspberry Pi (ARM).

---

# 🌍 Compatibilidad Multiplataforma

## ❓ ¿Qué significa multiplataforma?

Significa que un sistema operativo o software puede funcionar en diferentes arquitecturas.

Ejemplo:

Linux puede correr en:

- x86
- ARM
- RISC-V
- PowerPC

---

## ❓ ¿Cómo logra Raspberry Pi esta compatibilidad?

Porque usa principalmente:

> Linux (Raspberry Pi OS basado en Debian)

Linux es portable.

Eso significa que el kernel puede adaptarse a distintos procesadores.

Además puede ejecutar:

- Ubuntu
- Fedora
- Gentoo
- Kali Linux
- FreeBSD
- Windows IoT

---

## ❓ ¿Por qué es importante?

Demuestra que el sistema operativo no depende de una sola arquitectura.

Eso es **diseño modular**.

Linux separa:

- Código dependiente del hardware
- Código independiente del hardware

---

# ⚙️ Adaptación de Kernels

## ❓ ¿Qué es el kernel?

El kernel es el núcleo del sistema operativo.

Se encarga de:

- Gestionar CPU
- Gestionar memoria
- Controlar dispositivos
- Manejar procesos

---

## ❓ ¿Qué significa adaptar el kernel?

Significa configurarlo para que funcione con un hardware específico.

En Raspberry Pi, el kernel debe:

- Reconocer CPU ARM
- Manejar puertos GPIO
- Controlar USB, Ethernet y WiFi
- Manejar la GPU integrada

No es el mismo kernel que el de una laptop.

---

## ❓ ¿Cómo se adapta?

Mediante:

- Compilación específica para ARM
- Drivers específicos
- Configuración del Device Tree

---

## ❓ ¿Por qué es importante en Sistemas Operativos?

Porque demuestra que el SO:

- No es universal
- Debe comunicarse correctamente con el hardware

Raspberry Pi es ideal para estudiar esto porque es:

- Abierta
- Accesible
- Bien documentada

---

# 🧩 Gestión de Recursos en Hardware Limitado

## ❓ ¿Qué significa hardware limitado?

Comparado con una PC moderna:

- Menos RAM
- Menos potencia CPU
- Menos almacenamiento

Ejemplo:

- Raspberry Pi 1: 512 MB RAM  
- Raspberry Pi 4/5: hasta 8 GB RAM  

---

## ❓ ¿Qué debe hacer el sistema operativo?

Administrar cuidadosamente:

- Memoria
- Procesos
- Prioridades
- Consumo energético

---

## ❓ ¿Cómo lo hace?

1. Planificación eficiente de procesos
2. Uso controlado de memoria virtual
3. Gestión de caché
4. Drivers optimizados
5. Evitando procesos innecesarios

---

## ❓ ¿Por qué es importante?

Porque obliga a diseñar sistemas eficientes.

En una PC potente puedes desperdiciar recursos.  
En Raspberry Pi no.

Por eso es un laboratorio ideal para:

- Estudiar planificación
- Medir uso de CPU
- Analizar swapping
- Optimizar procesos

---

# 🎯 Resumen Integrador

| Concepto | Idea Central |
|----------|--------------|
| Arquitectura ARM | CPU eficiente, bajo consumo, diferente a x86 |
| Compatibilidad Multiplataforma | Linux puede adaptarse a múltiples arquitecturas |
| Adaptación de Kernel | El núcleo del SO debe configurarse para el hardware específico |
| Gestión en Hardware Limitado | El SO debe optimizar recursos escasos |

---

# 🧠 Preguntas para Verificar Comprensión

1. ¿Por qué no puedes instalar cualquier Windows en Raspberry Pi?
2. ¿Qué ventaja tiene ARM frente a x86 en consumo energético?
3. ¿Por qué Linux es considerado portable?
4. ¿Qué problemas aparecen cuando la RAM es limitada?
5. ¿Qué parte del SO interactúa directamente con el hardware?
