---
title: "TxtLoadStyleStrategy"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Specifica come applicare lo stile ai valori analizzati quando si converte una stringa in numero o data/ora."
type: docs
url: /it/java/com.aspose.cells/txtloadstylestrategy/
---

**Inheritance:**
java.lang.Object
```
public final class TxtLoadStyleStrategy
```

Specifica come applicare lo stile ai valori analizzati quando si converte una stringa in numero o data/ora.
## Campi

| Campo | Descrizione |
| --- | --- |
| [BUILT_IN](#BUILT-IN) | Imposta lo stile come numero/data‑ora incorporato quando il valore analizzato è un valore numerico/data‑ora semplice. |
| [EXACT_FORMAT](#EXACT-FORMAT) | Imposta il formato personalizzato esatto per il valore analizzato in modo che il valore formattato sia identico all'input originale. |
| [NONE](#NONE) | Non imposta lo stile per il valore analizzato. |
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
### BUILT_IN {#BUILT-IN}
```
public static final int BUILT_IN
```


Imposta lo stile come numero/data‑ora incorporato quando il valore analizzato è un valore numerico/data‑ora semplice.

**Remarks**

Quando ms excel analizza valori data‑ora o numerici in base all'input dell'utente (ad esempio file CSV), la formattazione di tali valori può cambiare, come gli zeri iniziali/finali del numero, l'ordine anno/mese/giorno della data‑ora, ...etc. Questo tipo serve a simulare il comportamento di ms excel.

### EXACT_FORMAT {#EXACT-FORMAT}
```
public static final int EXACT_FORMAT
```


Imposta il formato personalizzato esatto per il valore analizzato in modo che il valore formattato sia identico all'input originale.

### NONE {#NONE}
```
public static final int NONE
```


Non imposta lo stile per il valore analizzato.

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

