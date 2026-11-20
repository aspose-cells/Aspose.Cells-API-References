---
title: "CellValueFormatStrategy"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Specifica come applicare lo stile al valore della cella."
type: docs
url: /it/java/com.aspose.cells/cellvalueformatstrategy/
---

**Inheritance:**
java.lang.Object
```
public final class CellValueFormatStrategy
```

Specifica come applicare lo stile al valore della cella.
## Campi

| Campo | Descrizione |
| --- | --- |
| [CELL_STYLE](#CELL-STYLE) | Formattato solo con lo stile originale della cella. |
| [DISPLAY_STRING](#DISPLAY-STRING) | Restituisce la stringa visualizzata mostrata in MS Excel. |
| [DISPLAY_STYLE](#DISPLAY-STYLE) | Formattato con lo stile visualizzato della cella. |
| [NONE](#NONE) | Non formattato. |
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
### CELL_STYLE {#CELL-STYLE}
```
public static final int CELL_STYLE
```


Formattato solo con lo stile originale della cella.

### DISPLAY_STRING {#DISPLAY-STRING}
```
public static final int DISPLAY_STRING
```


Restituisce la stringa visualizzata mostrata in MS Excel. La principale differenza rispetto a [DISPLAY\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#DISPLAY-STYLE) è che questa opzione considera anche l'effetto della larghezza della colonna. Se la larghezza della colonna è troppo piccola per mostrare completamente la stringa formattata, \"\\#\" può essere visualizzato, proprio come fa MS Excel.

### DISPLAY_STYLE {#DISPLAY-STYLE}
```
public static final int DISPLAY_STYLE
```


Formattato con lo stile visualizzato della cella.

### NONE {#NONE}
```
public static final int NONE
```


Non formattato.

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

