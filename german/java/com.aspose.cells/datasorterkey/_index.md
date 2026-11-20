---
title: "DataSorterKey"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt den Schlüssel des DataSorters dar."
type: docs
url: /de/java/com.aspose.cells/datasorterkey/
---

**Inheritance:**
java.lang.Object
```
public class DataSorterKey
```

Stellt den Schlüssel des DataSorters dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Liefert die sortierte Farbe. |
| [getIconId()](#getIconId--) | Stellt die ID des Symbolsatztyps dar. |
| [getIconSetType()](#getIconSetType--) | Stellt den Symbolsatztyp dar. |
| [getIndex()](#getIndex--) | Liefert den sortierten Spaltenindex (absolute Position, Spalte A ist 0, B ist 1, ...). |
| [getOrder()](#getOrder--) | Gibt die Sortierreihenfolge an. |
| [getType()](#getType--) | Stellt den Sortierungstyp dar. |
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
### getColor() {#getColor--}
```
public Color getColor()
```


Liefert die sortierte Farbe.

**Remarks**

Wirkt nur, wenn [getType()](../../com.aspose.cells/datasorterkey\#getType--) [SortOnType.CELL\_COLOR](../../com.aspose.cells/sortontype\#CELL-COLOR) oder [SortOnType.FONT\_COLOR](../../com.aspose.cells/sortontype\#FONT-COLOR) ist.

**Returns:**
[Color](../../com.aspose.cells/color)
### getIconId() {#getIconId--}
```
public int getIconId()
```


Stellt die ID des Symbolsatztyps dar.

**Remarks**

Wirkt nur, wenn [getType()](../../com.aspose.cells/datasorterkey\#getType--) [SortOnType.ICON](../../com.aspose.cells/sortontype\#ICON) ist.

**Returns:**
int
### getIconSetType() {#getIconSetType--}
```
public int getIconSetType()
```


Stellt den Symbolsatztyp dar.

Siehe [IconSetType](../../com.aspose.cells/iconsettype).

**Remarks**

Wirkt nur, wenn [getType()](../../com.aspose.cells/datasorterkey\#getType--) [SortOnType.ICON](../../com.aspose.cells/sortontype\#ICON) ist.

**Returns:**
int
### getIndex() {#getIndex--}
```
public int getIndex()
```


Liefert den sortierten Spaltenindex (absolute Position, Spalte A ist 0, B ist 1, ...).

**Returns:**
int
### getOrder() {#getOrder--}
```
public int getOrder()
```


Gibt die Sortierreihenfolge an.

Siehe [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Stellt den Sortierungstyp dar.

Siehe [SortOnType](../../com.aspose.cells/sortontype).

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

