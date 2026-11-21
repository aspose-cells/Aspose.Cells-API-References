---
title: "ThreadInterruptMonitor"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Implementación simple de  iniciando otro hilo para requerir la interrupción después de dormir el límite especificado por el usuario."
type: docs
url: /es/java/com.aspose.cells/threadinterruptmonitor/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
```
public class ThreadInterruptMonitor extends AbstractInterruptMonitor
```

Implementación simple de [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) iniciando otro hilo para requerir la interrupción después de dormir el límite especificado por el usuario.

**Remarks**

Una instancia de monitor puede usarse repetidamente, siempre que monitorees cada proceso en secuencia. No debe usarse para monitorear múltiples procedimientos concurrentemente en hilos múltiples.

**Example**

El siguiente ejemplo muestra cómo monitorizar el procedimiento de carga y guardado con un límite de tiempo especificado:

```
         ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
         LoadOptions lopts = new LoadOptions();
         lopts.setInterruptMonitor(monitor);
         monitor.startMonitor(1000); //time limit is 1 second
         Workbook wb = new Workbook("Large.xlsx", lopts);
         //if the time cost of loading the template file exceeds one second, interruption will be required and exception will be thrown here
         //otherwise finishes the monitor thread and starts to monitor the save procedure
         monitor.finishMonitor();
         monitor.startMonitor(1500); //time limit is 1.5 seconds
         wb.save("result.xlsx");
         monitor.finishMonitor();
```
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ThreadInterruptMonitor(boolean terminateWithoutException)](#ThreadInterruptMonitor-boolean-) | Construye un monitor de interrupción. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finishMonitor()](#finishMonitor--) | Finaliza el monitor para un procedimiento. |
| [getClass()](#getClass--) |  |
| [getTerminateWithoutException()](#getTerminateWithoutException--) | Ver [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--). |
| [hashCode()](#hashCode--) |  |
| [isInterruptionRequested()](#isInterruptionRequested--) | Esta implementación solo verifica si el tiempo consumido (desde el momento en que se inició este monitor hasta ahora) es mayor que el límite especificado por el usuario. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [startMonitor(int msLimit)](#startMonitor-int-) | Inicia el monitor con el límite de tiempo especificado. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ThreadInterruptMonitor(boolean terminateWithoutException) {#ThreadInterruptMonitor-boolean-}
```
public ThreadInterruptMonitor(boolean terminateWithoutException)
```


Construye un monitor de interrupción.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| terminateWithoutException | boolean | [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--) |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### finishMonitor() {#finishMonitor--}
```
public void finishMonitor()
```


Finaliza el monitor para un procedimiento.

**Remarks**

Llamar a este método después del procedimiento monitorizado puede liberar el hilo del monitor antes, especialmente cuando no hay interrupción para él(el costo de tiempo de ese procedimiento es menor que el límite de tiempo especificado).

### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getTerminateWithoutException() {#getTerminateWithoutException--}
```
public boolean getTerminateWithoutException()
```


Ver [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--). Esta propiedad es especificada por el usuario al construir esta instancia de monitor.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isInterruptionRequested() {#isInterruptionRequested--}
```
public boolean isInterruptionRequested()
```


Esta implementación solo verifica si el tiempo consumido (desde el momento en que se inició este monitor hasta ahora) es mayor que el límite especificado por el usuario.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### startMonitor(int msLimit) {#startMonitor-int-}
```
public void startMonitor(int msLimit)
```


Inicia el monitor con el límite de tiempo especificado. El tiempo de inicio para calcular el costo de tiempo es justo cuando se llama a este método, por lo que el procedimiento que necesita ser monitoreado debe iniciarse justo después de esta llamada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| msLimit | int | límite de tiempo (ms) para requerir la interrupción. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

