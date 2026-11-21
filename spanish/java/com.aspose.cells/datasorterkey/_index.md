---
title: "DataSorterKey"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la clave del DataSorter."
type: docs
url: /es/java/com.aspose.cells/datasorterkey/
---

**Inheritance:**
java.lang.Object
```
public class DataSorterKey
```

Representa la clave del DataSorter.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Obtiene el color ordenado. |
| [getIconId()](#getIconId--) | Representa el id del tipo de conjunto de iconos. |
| [getIconSetType()](#getIconSetType--) | Representa el tipo de conjunto de iconos. |
| [getIndex()](#getIndex--) | Obtiene el índice de columna ordenada (posición absoluta, la columna A es 0, B es 1, ...). |
| [getOrder()](#getOrder--) | Indica el orden de clasificación. |
| [getType()](#getType--) | Representa el tipo de clasificación. |
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
| Parámetro | Tipo | Descripción |
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


Obtiene el color ordenado.

**Remarks**

Solo tiene efecto cuando [getType()](../../com.aspose.cells/datasorterkey\#getType--) es [SortOnType.CELL\_COLOR](../../com.aspose.cells/sortontype\#CELL-COLOR) o [SortOnType.FONT\_COLOR](../../com.aspose.cells/sortontype\#FONT-COLOR).

**Returns:**
[Color](../../com.aspose.cells/color)
### getIconId() {#getIconId--}
```
public int getIconId()
```


Representa el id del tipo de conjunto de iconos.

**Remarks**

Solo tiene efecto cuando [getType()](../../com.aspose.cells/datasorterkey\#getType--) es [SortOnType.ICON](../../com.aspose.cells/sortontype\#ICON).

**Returns:**
int
### getIconSetType() {#getIconSetType--}
```
public int getIconSetType()
```


Representa el tipo de conjunto de iconos.

Ver [IconSetType](../../com.aspose.cells/iconsettype).

**Remarks**

Solo tiene efecto cuando [getType()](../../com.aspose.cells/datasorterkey\#getType--) es [SortOnType.ICON](../../com.aspose.cells/sortontype\#ICON).

**Returns:**
int
### getIndex() {#getIndex--}
```
public int getIndex()
```


Obtiene el índice de columna ordenada (posición absoluta, la columna A es 0, B es 1, ...).

**Returns:**
int
### getOrder() {#getOrder--}
```
public int getOrder()
```


Indica el orden de clasificación.

Ver [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Representa el tipo de clasificación.

Ver [SortOnType](../../com.aspose.cells/sortontype).

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

