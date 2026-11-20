---
title: "TxtValueQuoteType"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Specifica il tipo di utilizzo delle virgolette per i valori nei file di testo."
type: docs
url: /it/java/com.aspose.cells/txtvaluequotetype/
---

**Inheritance:**
java.lang.Object
```
public final class TxtValueQuoteType
```

Specifica il tipo di utilizzo delle virgolette per i valori nei file di testo.
## Campi

| Campo | Descrizione |
| --- | --- |
| [ALWAYS](#ALWAYS) | Tutti i valori saranno sempre tra virgolette. |
| [MINIMUM](#MINIMUM) | Metti tra virgolette i valori solo quando necessario. |
| [NEVER](#NEVER) | Tutti i valori non saranno tra virgolette. |
| [NORMAL](#NORMAL) | Tutti i valori che contengono caratteri speciali come il segno di virgolette o il carattere separatore saranno tra virgolette. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALWAYS {#ALWAYS}
```
public static final int ALWAYS
```


Tutti i valori saranno sempre tra virgolette.

### MINIMUM {#MINIMUM}
```
public static final int MINIMUM
```


Metti tra virgolette i valori solo quando necessario. Ad esempio, se un valore contiene il segno di virgolette ma il segno di virgolette non è all'inizio di questo valore, questo valore non sarà tra virgolette.

### NEVER {#NEVER}
```
public static final int NEVER
```


Tutti i valori non saranno racchiusi tra virgolette. Il file di testo esportato con questo tipo potrebbe non essere riletto correttamente perché mancano le virgolette necessarie.

### NORMAL {#NORMAL}
```
public static final int NORMAL
```


Tutti i valori che contengono caratteri speciali come il segno di virgolette o il carattere separatore saranno racchiusi tra virgolette. Lo stesso vale per il comportamento di MS Excel durante l'esportazione di file di testo.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
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
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

