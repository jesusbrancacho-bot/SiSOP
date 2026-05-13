# Contexto General:
Capitulo de procesos e hilos, especificamente en el tema de:
  - Comunicación entre procesos (IPC)
  - Sincronización
  - Problemas de concurrencia
  - Regiones críticas
  - Condiciones de carrera (rare conditions)

**El problema central es:**
<pre>
¿Cómo coordinamos múltiples procesos o hilos que acceden a recursos compartidos sin que el sistema se vuelva caótico?
</pre>

**Ejemplo Tipico**
- Productor que agrega datos a un buffer
- Consumidor que lo saca
- Ambos acceden al mismo espacio de memoria

Si no hay control -> corrupción de datos **errores inesperados en los archivos informáticos que ocurren durante la escritura, lectura, almacenamiento o tranmisión, provocando cambios no deseados
en la información original. Esto provoca que los datos sean ilegibles, inutilizables o se comportan de manera errónea, sin que el archivo desaparezca por completo.**
