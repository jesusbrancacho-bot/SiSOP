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


Raspberry Pi en Sistemas Operativos
Aplicaciones Académicas y Técnicas

------------------------------------------------------------

1️⃣ Laboratorio de Kernel Linux
❓ ¿Qué es?

Usar la Raspberry Pi para estudiar y experimentar con el núcleo del sistema operativo (kernel).

Recuerda:
El kernel es el que controla:

CPU
Memoria
Procesos
Dispositivos
⚙️ ¿Cómo se usa en la práctica?

En Raspberry Pi puedes:

Compilar tu propio kernel Linux para ARM.
Modificar módulos.
Activar o desactivar drivers.
Probar cambios reales en hardware físico.
🧠 ¿Qué aprendes?
Cómo el kernel detecta hardware.
Cómo se cargan drivers.
Cómo se gestionan interrupciones.
Cómo se programa a bajo nivel.
🧩 Ejemplo

Cambias la política de planificación del kernel.
Recompilas.
Reinicias la Raspberry.
Observas cómo cambian los tiempos de respuesta.

Eso es laboratorio real.

2️⃣ Experimentos de planificación de procesos
❓ ¿Qué es planificación?

Es decidir:

¿Qué proceso usa la CPU y por cuánto tiempo?

⚙️ ¿Cómo lo pruebas en Raspberry Pi?

Puedes:

Crear múltiples procesos.
Medir tiempos de espera.
Analizar uso de CPU con top.
Cambiar prioridades con nice.
🧠 ¿Qué se aprende?
Round Robin
Prioridades
Starvation
Context switch
Uso eficiente de CPU
🧩 Ejemplo

Ejecutas:

yes > /dev/null

Varias veces.

Creas carga artificial.

Observas cómo el scheduler reparte CPU.

Eso es teoría aplicada.

3️⃣ Sistemas Embebidos
❓ ¿Qué es un sistema embebido?

Es un sistema que:

Está dedicado a una tarea específica.
No es una PC general.
Está integrado en un dispositivo.

Ejemplos:

Robot
Control industrial
Sistema domótico
⚙️ ¿Cómo Raspberry Pi se usa aquí?

Porque:

Es pequeña.
Consume poca energía.
Tiene GPIO (pines físicos).
Corre Linux.
🧠 ¿Qué se aprende?
Sistemas en tiempo real.
Interacción hardware–software.
Drivers.
Manejo de sensores.
🧩 Ejemplo

Conectas un sensor de temperatura.
El sistema operativo recibe la señal.
Un proceso decide encender un ventilador.

Eso es SO interactuando con mundo físico.

4️⃣ Servidor Web Casero
❓ ¿Qué es?

Usar Raspberry Pi como servidor:

Apache
Nginx
Node.js
⚙️ ¿Cómo funciona?
Instalas servidor web.
Abres puerto 80.
La Raspberry responde peticiones HTTP.
🧠 ¿Qué se aprende?
Gestión de procesos servidor.
Concurrencia.
Uso de sockets.
Administración de memoria bajo carga.
🧩 Ejemplo

10 personas entran a tu página.

El SO debe:

Crear procesos o hilos.
Administrar memoria.
Gestionar red.

Eso es práctica directa de IPC y planificación.

5️⃣ Firewall
❓ ¿Qué es un firewall?

Es un sistema que:

Filtra tráfico de red.
Decide qué entra y qué sale.
⚙️ ¿Cómo Raspberry Pi actúa como firewall?

Se instala Linux + iptables o nftables.

La Raspberry:

Analiza paquetes.
Aplica reglas.
Bloquea accesos.
🧠 ¿Qué se aprende?
Redes en SO.
Manejo de sockets.
Seguridad.
Gestión de paquetes.
🧩 Ejemplo

Regla:

sudo iptables -A INPUT -p tcp --dport 22 -j DROP

Bloqueas acceso SSH.

Eso es el sistema operativo filtrando tráfico.

6️⃣ Nodo de Red
❓ ¿Qué es un nodo?

Un dispositivo que forma parte de una red.

Puede ser:

Router
Switch
Servidor
Cliente
⚙️ ¿Cómo Raspberry Pi funciona como nodo?

Puede actuar como:

Servidor DNS
Proxy
Router WiFi
Cliente en cluster
🧠 ¿Qué se aprende?
Comunicación entre procesos.
Protocolos de red.
Distribución de carga.
Computación distribuida.
🧩 Ejemplo avanzado

Clusters de cientos de Raspberry Pi se usan para probar programas destinados a supercomputadoras.

Eso significa:

Muchas máquinas pequeñas trabajando juntas.

Aprendes:

Sincronización distribuida.
Comunicación por red.
Gestión remota.
🎯 Integración Final

Raspberry Pi sirve en Sistemas Operativos porque permite experimentar con:

Kernel
Planificación
Memoria
Redes
Seguridad
Sistemas embebidos
Computación distribuida

Es un laboratorio real, barato y físico.

🧠 Pregunta clave para examen

¿Por qué Raspberry Pi es ideal para estudiar Sistemas Operativos?

Porque permite experimentar con hardware real, arquitectura ARM y Linux en un entorno controlado y de bajo costo.


1️⃣ ¿Qué diferencia hay entre Raspberry Pi y Raspberry Pi Pico?
❓ ¿Qué es Raspberry Pi (normal)?

Es una microcomputadora completa.

Tiene:

CPU
RAM
Sistema operativo
HDMI
USB
Red
Puede ejecutar Linux

Ejemplo: Raspberry Pi 4 o 5 puede correr Raspberry Pi OS (Linux) .

Es como una mini PC.

❓ ¿Qué es Raspberry Pi Pico?

Es un microcontrolador, no una computadora completa .

Eso significa:

No ejecuta un sistema operativo como Linux.
Ejecuta programas directamente.
Se usa para controlar hardware físico.
🎯 Diferencia clave
Raspberry Pi	Raspberry Pi Pico
Corre Linux	No corre Linux
Multitarea	Programa único
Tiene sistema operativo	No necesita SO complejo
Mini PC	Microcontrolador
🧠 En términos de SO

Raspberry Pi → Estudias procesos, memoria, kernel.
Raspberry Pi Pico → Estudias programación embebida sin SO complejo.

2️⃣ ¿Por qué usa arquitectura ARM y no x86?
❓ ¿Qué es ARM?

Es una arquitectura de procesador eficiente y de bajo consumo.

Los modelos usan CPU ARM Cortex (A53, A72, A76) .

❓ ¿Qué es x86?

Arquitectura tradicional de PCs (Intel, AMD).

Consume más energía.
Es más compleja.

❓ ¿Por qué ARM en Raspberry Pi?

Porque:

Consume menos energía.
Genera menos calor.
Es más barata.
Ideal para dispositivos pequeños.
🧠 En Sistemas Operativos

El SO debe estar compilado para la arquitectura correcta.

No puedes instalar Windows tradicional (x86) en Raspberry Pi (ARM).

Eso demuestra:

El sistema operativo depende del hardware.

3️⃣ ¿Cómo influye la cantidad de RAM en el rendimiento del sistema operativo?

Esta es muy importante.

❓ ¿Qué hace la RAM?

Guarda:

Procesos en ejecución
Datos temporales
Caché
❓ ¿Qué pasa si hay poca RAM?

El sistema:

Empieza a usar memoria virtual (swap).
Se vuelve más lento.
Hace más accesos al disco.

Ejemplo:
Raspberry Pi 1 tenía 512 MB .
Raspberry Pi 4 puede tener hasta 8 GB .

Más RAM → más procesos simultáneos → mejor rendimiento.

🧠 En Sistemas Operativos

La RAM afecta:

Planificación
Paginación
Swapping
Rendimiento global

Si hay poca RAM:
El SO debe gestionar memoria cuidadosamente.

4️⃣ ¿Por qué es útil para estudiar planificación de procesos?
❓ ¿Qué es planificación?

Es decidir:

¿Qué proceso usa la CPU y cuándo?

❓ ¿Por qué Raspberry Pi es buena para esto?

Porque:

Corre Linux real.
Tiene recursos limitados.
Permite experimentar sin dañar una PC principal.

Puedes:

Crear múltiples procesos.
Cambiar prioridades.
Medir tiempos.
Observar uso de CPU.
🧠 En práctica

Si ejecutas varios programas pesados, verás cómo el scheduler reparte CPU.

Eso te permite entender:

Round Robin
Prioridades
Starvation
Context switching

Es teoría convertida en práctica.

5️⃣ ¿Cuál modelo sería mejor para montar un servidor pequeño?
❓ ¿Qué necesita un servidor?
Buena CPU
Suficiente RAM
Red rápida
USB rápido (si hay almacenamiento externo)
🔍 Comparación rápida

Raspberry Pi 3:

1 GB RAM
Ethernet 100 Mbps

Raspberry Pi 4:

Hasta 8 GB RAM
Ethernet Gigabit
USB 3.0

Raspberry Pi 5:

CPU más potente
Hasta 8 GB RAM
Mejor rendimiento general
🎯 Respuesta correcta

Para servidor pequeño:

👉 Raspberry Pi 4 o 5.

Porque:

Más RAM
Mejor red
Mejor CPU
🧠 Integración final (lo que debes entender realmente)

Estas preguntas no son solo datos.

Evalúan si entendiste:

Relación hardware–software.
Arquitectura del sistema.
Gestión de memoria.
Planificación de CPU.
Uso real del sistema operativo.

Si puedes explicar esto con tus propias palabras,
ya dominaste el tema.


