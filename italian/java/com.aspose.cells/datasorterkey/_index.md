---
title: "DataSorterKey"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta la chiave del data sorter."
type: docs
url: /it/java/com.aspose.cells/datasorterkey/
---

**Inheritance:**
java.lang.Object
```
public class DataSorterKey
```

Rappresenta la chiave del data sorter.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Ottiene il colore ordinato. |
| [getIconId()](#getIconId--) | Rappresenta l'ID del tipo di set di icone. |
| [getIconSetType()](#getIconSetType--) | Rappresenta il tipo di set di icone. |
| [getIndex()](#getIndex--) | Ottiene l'indice della colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...). |
| [getOrder()](#getOrder--) | Indica l'ordine di ordinamento. |
| [getType()](#getType--) | Rappresenta il tipo di ordinamento. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getColor() {#getColor--}
```
public Color getColor()
```


Ottiene il colore ordinato.

**Remarks**

Ha effetto solo quando [getType()](../../com.aspose.cells/datasorterkey\#getType--) è [SortOnType.CELL\_COLOR](../../com.aspose.cells/sortontype\#CELL-COLOR) o [SortOnType.FONT\_COLOR](../../com.aspose.cells/sortontype\#FONT-COLOR).

**Returns:**
[Color](../../com.aspose.cells/color)
### getIconId() {#getIconId--}
```
public int getIconId()
```


Rappresenta l'ID del tipo di set di icone.

**Remarks**

Ha effetto solo quando [getType()](../../com.aspose.cells/datasorterkey\#getType--) è [SortOnType.ICON](../../com.aspose.cells/sortontype\#ICON).

**Returns:**
int
### getIconSetType() {#getIconSetType--}
```
public int getIconSetType()
```


Rappresenta il tipo di set di icone.

Vedi [IconSetType](../../com.aspose.cells/iconsettype).

**Remarks**

Ha effetto solo quando [getType()](../../com.aspose.cells/datasorterkey\#getType--) è [SortOnType.ICON](../../com.aspose.cells/sortontype\#ICON).

**Returns:**
int
### getIndex() {#getIndex--}
```
public int getIndex()
```


Ottiene l'indice della colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...).

**Returns:**
int
### getOrder() {#getOrder--}
```
public int getOrder()
```


Indica l'ordine di ordinamento.

Vedi [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Rappresenta il tipo di ordinamento.

Vedi [SortOnType](../../com.aspose.cells/sortontype).

**Returns:**
int
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

