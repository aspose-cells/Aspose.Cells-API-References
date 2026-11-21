---
title: "DataSorterKey"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar nyckeln för data-sorteraren."
type: docs
url: /sv/java/com.aspose.cells/datasorterkey/
---

**Inheritance:**
java.lang.Object
```
public class DataSorterKey
```

Representerar nyckeln för data-sorteraren.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Hämtar den sorterade färgen. |
| [getIconId()](#getIconId--) | Representerar id för ikonsättstypen. |
| [getIconSetType()](#getIconSetType--) | Representerar ikonsättstypen. |
| [getIndex()](#getIndex--) | Hämtar det sorterade kolumnindexet (absolut position, kolumn A är 0, B är 1, ...). |
| [getOrder()](#getOrder--) | Anger sorteringsordningen. |
| [getType()](#getType--) | Representerar sorteringstypen. |
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
| Parameter | Typ | Beskrivning |
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


Hämtar den sorterade färgen.

**Remarks**

Gäller endast när [getType()](../../com.aspose.cells/datasorterkey\#getType--) är [SortOnType.CELL\_COLOR](../../com.aspose.cells/sortontype\#CELL-COLOR) eller [SortOnType.FONT\_COLOR](../../com.aspose.cells/sortontype\#FONT-COLOR).

**Returns:**
[Color](../../com.aspose.cells/color)
### getIconId() {#getIconId--}
```
public int getIconId()
```


Representerar id för ikonsättstypen.

**Remarks**

Gäller endast när [getType()](../../com.aspose.cells/datasorterkey\#getType--) är [SortOnType.ICON](../../com.aspose.cells/sortontype\#ICON).

**Returns:**
int
### getIconSetType() {#getIconSetType--}
```
public int getIconSetType()
```


Representerar ikonsättstypen.

Se [IconSetType](../../com.aspose.cells/iconsettype).

**Remarks**

Gäller endast när [getType()](../../com.aspose.cells/datasorterkey\#getType--) är [SortOnType.ICON](../../com.aspose.cells/sortontype\#ICON).

**Returns:**
int
### getIndex() {#getIndex--}
```
public int getIndex()
```


Hämtar det sorterade kolumnindexet (absolut position, kolumn A är 0, B är 1, ...).

**Returns:**
int
### getOrder() {#getOrder--}
```
public int getOrder()
```


Anger sorteringsordningen.

Se [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Representerar sorteringstypen.

Se [SortOnType](../../com.aspose.cells/sortontype).

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

