# 📘 Raspberry Pi en Sistemas Operativos  
## Guía Completa para Estudio Académico

---

# 1️⃣ ¿Qué es Raspberry Pi?

Raspberry Pi es una **microcomputadora del tamaño de una tarjeta de crédito** diseñada para educación, experimentación y proyectos tecnológicos.

Permite:

- Ejecutar sistemas operativos (principalmente Linux).
- Conectar dispositivos físicos.
- Realizar proyectos de redes, servidores y sistemas embebidos.

Se basa en arquitectura **ARM** y ha evolucionado desde modelos con 512 MB de RAM hasta versiones con 8 GB y CPUs de alto rendimiento.

---

# 2️⃣ Arquitectura ARM

## ¿Qué es ARM?

ARM es una arquitectura de procesador basada en el modelo:

> RISC (Reduced Instruction Set Computer)

Esto significa:

- Instrucciones más simples.
- Menor consumo energético.
- Mayor eficiencia por watt.

## ¿Por qué Raspberry Pi usa ARM?

- Bajo consumo de energía.
- Menor generación de calor.
- Menor costo.
- Ideal para sistemas pequeños y embebidos.

## Importancia en Sistemas Operativos

El sistema operativo debe:

- Estar compilado específicamente para ARM.
- Gestionar su conjunto de instrucciones.
- Adaptarse a su modelo de memoria.

No se puede instalar un sistema operativo diseñado para x86 directamente en ARM.

---

# 3️⃣ Compatibilidad Multiplataforma

## ¿Qué significa?

Un sistema operativo multiplataforma puede ejecutarse en diferentes arquitecturas.

Linux puede ejecutarse en:

- x86
- ARM
- RISC-V
- PowerPC

Raspberry Pi utiliza principalmente **Raspberry Pi OS**, basado en Debian Linux.

## Importancia

Demuestra que el kernel puede adaptarse a distintos tipos de hardware gracias a su diseño modular.

---

# 4️⃣ Adaptación de Kernel

## ¿Qué es el kernel?

Es el núcleo del sistema operativo. Gestiona:

- CPU
- Memoria
- Procesos
- Dispositivos

## ¿Qué significa adaptarlo?

Configurar y compilar el kernel específicamente para el hardware de Raspberry Pi:

- CPU ARM
- Controladores (drivers)
- Puertos GPIO
- Dispositivos USB, red, etc.

## ¿Qué se aprende?

- Relación hardware–software.
- Compilación de kernel.
- Manejo de interrupciones.
- Drivers.

---

# 5️⃣ Gestión de Recursos en Hardware Limitado

## ¿Qué significa hardware limitado?

Comparado con una PC tradicional:

- Menor RAM.
- Menor potencia de CPU.
- Almacenamiento en microSD.

## ¿Qué debe hacer el sistema operativo?

- Administrar memoria eficientemente.
- Evitar consumo innecesario.
- Gestionar procesos correctamente.
- Optimizar uso de CPU.

## ¿Qué conceptos se aplican?

- Memoria virtual.
- Swapping.
- Planificación.
- Prioridades.

---

# 6️⃣ Planificación de Procesos

## ¿Qué es?

Es el mecanismo mediante el cual el sistema operativo decide:

> Qué proceso usa la CPU y por cuánto tiempo.

## ¿Qué se puede experimentar?

- Crear múltiples procesos.
- Cambiar prioridades.
- Analizar uso de CPU.
- Observar distribución de recursos.

## Conceptos clave

- Round Robin
- Prioridades
- Starvation
- Context switching

---

# 7️⃣ Sistemas Embebidos

## ¿Qué es un sistema embebido?

Sistema dedicado a una tarea específica.

Ejemplos:

- Robots
- Control industrial
- Domótica

## ¿Por qué Raspberry Pi?

- Tamaño reducido.
- Bajo consumo.
- Pines GPIO.
- Capacidad de ejecutar Linux.

## ¿Qué se aprende?

- Interacción hardware–software.
- Control de sensores.
- Sistemas en tiempo real.

---

# 8️⃣ Servidor Web Casero

Raspberry Pi puede funcionar como:

- Servidor Apache
- Servidor Nginx
- Servidor Node.js

## ¿Qué se aprende?

- Concurrencia.
- Manejo de sockets.
- Gestión de procesos.
- Administración de memoria bajo carga.

---

# 9️⃣ Firewall

Raspberry Pi puede funcionar como firewall utilizando:

- iptables
- nftables

Permite:

- Filtrar tráfico.
- Bloquear puertos.
- Implementar reglas de seguridad.

## Conceptos aplicados

- Redes en sistemas operativos.
- Seguridad.
- Gestión de paquetes.

---

# 🔟 Nodo de Red

Raspberry Pi puede actuar como:

- Servidor DNS
- Proxy
- Router
- Cliente en cluster

## ¿Qué se aprende?

- Comunicación entre procesos.
- Protocolos de red.
- Computación distribuida.
- Sincronización entre máquinas.

Clusters de múltiples Raspberry Pi pueden simular sistemas distribuidos.

---

# 1️⃣1️⃣ Raspberry Pi vs Raspberry Pi Pico

| Raspberry Pi | Raspberry Pi Pico |
|--------------|------------------|
| Corre Linux | No corre Linux |
| Multitarea | Programa único |
| Tiene sistema operativo completo | Microcontrolador |
| Mini PC | Dispositivo para control físico |

---

# 🎯 Conclusión Académica

Raspberry Pi es ideal para estudiar Sistemas Operativos porque permite experimentar con:

- Kernel
- Arquitectura ARM
- Planificación
- Gestión de memoria
- Redes
- Seguridad
- Sistemas embebidos
- Computación distribuida

Es económica, accesible y permite laboratorio real con hardware físico.

---

# 🧠 Preguntas Clave de Examen

1. ¿Por qué la arquitectura ARM es importante en Raspberry Pi?
2. ¿Cómo influye la RAM en el rendimiento del sistema operativo?
3. ¿Qué es planificación de procesos y cómo se prueba en Raspberry Pi?
4. ¿Por qué Linux es considerado portable?
5. ¿Cuál modelo sería ideal para un servidor pequeño y por qué?

---

**Fin del documento**
