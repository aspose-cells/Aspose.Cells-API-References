---
title: "AbstractInterruptMonitor"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Überwacht Unterbrechungsanfragen bei allen zeitintensiven Vorgängen."
type: docs
url: /de/java/com.aspose.cells/abstractinterruptmonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractInterruptMonitor
```

Überwacht Unterbrechungsanfragen bei allen zeitintensiven Vorgängen.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [AbstractInterruptMonitor()](#AbstractInterruptMonitor--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getTerminateWithoutException()](#getTerminateWithoutException--) | Wenn das Verfahren unterbrochen wird, ob das Verfahren stillschweigend beendet oder eine Ausnahme ausgelöst wird. |
| [hashCode()](#hashCode--) |  |
| [isInterruptionRequested()](#isInterruptionRequested--) | Gibt an, ob für den aktuellen Vorgang eine Unterbrechung angefordert wurde. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractInterruptMonitor() {#AbstractInterruptMonitor--}
```
public AbstractInterruptMonitor()
```


### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
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


Wenn das Verfahren unterbrochen wird, ob das Verfahren stillschweigend beendet oder eine Ausnahme ausgelöst wird. Standard ist false, das heißt, wenn [isInterruptionRequested()](../../com.aspose.cells/abstractinterruptmonitor\#isInterruptionRequested--) true ist, wird eine [CellsException](../../com.aspose.cells/cellsexception) mit dem Code [ExceptionType.INTERRUPTED](../../com.aspose.cells/exceptiontype\#INTERRUPTED) ausgelöst.

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
public abstract boolean isInterruptionRequested()
```


Gibt an, ob für den aktuellen Vorgang eine Unterbrechung angefordert wurde. Wenn true, wird der aktuelle Vorgang unterbrochen. Die Implementierung sollte hier eine schnelle und effiziente Prüfung durchführen, sonst könnte sie zum weiteren Engpass für das Verfahren werden.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

