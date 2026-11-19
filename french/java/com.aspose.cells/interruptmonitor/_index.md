---
title: "InterruptMonitor"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente tous les opérateurs concernant l'interruption."
type: docs
url: /fr/java/com.aspose.cells/interruptmonitor/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
```
public class InterruptMonitor extends AbstractInterruptMonitor
```

Représente tous les opérateurs concernant l'interruption.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [InterruptMonitor()](#InterruptMonitor--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getTerminateWithoutException()](#getTerminateWithoutException--) | Lorsque la procédure est interrompue, indique s'il faut terminer la procédure silencieusement ou lever une Exception. |
| [hashCode()](#hashCode--) |  |
| [interrupt()](#interrupt--) | Interrompt l'opérateur actuel. |
| [isInterruptionRequested()](#isInterruptionRequested--) | Marque le moniteur comme demandant une interruption |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### InterruptMonitor() {#InterruptMonitor--}
```
public InterruptMonitor()
```


### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
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


Lorsque la procédure est interrompue, qu'il faut‑il terminer la procédure silencieusement ou lever une Exception. La valeur par défaut est false, c’est‑à‑dire que lorsque [isInterruptionRequested()](../../com.aspose.cells/abstractinterruptmonitor\\#isInterruptionRequested--) est true, une [CellsException](../../com.aspose.cells/cellsexception) avec le code [ExceptionType.INTERRUPTED](../../com.aspose.cells/exceptiontype\\#INTERRUPTED) sera levée.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### interrupt() {#interrupt--}
```
public void interrupt()
```


Interrompt l'opérateur actuel.

### isInterruptionRequested() {#isInterruptionRequested--}
```
public boolean isInterruptionRequested()
```


Marque le moniteur comme demandant une interruption

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
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

