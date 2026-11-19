---
title: "DataSorterKey"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente la clé du DataSorter."
type: docs
url: /fr/java/com.aspose.cells/datasorterkey/
---

**Inheritance:**
java.lang.Object
```
public class DataSorterKey
```

Représente la clé du DataSorter.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Obtient la couleur triée. |
| [getIconId()](#getIconId--) | Représente l'ID du type d'ensemble d'icônes. |
| [getIconSetType()](#getIconSetType--) | Représente le type d'ensemble d'icônes. |
| [getIndex()](#getIndex--) | Obtient l'index de la colonne triée (position absolue, la colonne A est 0, B est 1, ...). |
| [getOrder()](#getOrder--) | Indique l'ordre du tri. |
| [getType()](#getType--) | Représente le type de tri. |
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
### getColor() {#getColor--}
```
public Color getColor()
```


Obtient la couleur triée.

**Remarks**

Ne prend effet que lorsque [getType()](../../com.aspose.cells/datasorterkey\#getType--) est [SortOnType.CELL\_COLOR](../../com.aspose.cells/sortontype\#CELL-COLOR) ou [SortOnType.FONT\_COLOR](../../com.aspose.cells/sortontype\#FONT-COLOR).

**Returns:**
[Color](../../com.aspose.cells/color)
### getIconId() {#getIconId--}
```
public int getIconId()
```


Représente l'ID du type d'ensemble d'icônes.

**Remarks**

Ne prend effet que lorsque [getType()](../../com.aspose.cells/datasorterkey\#getType--) est [SortOnType.ICON](../../com.aspose.cells/sortontype\#ICON).

**Returns:**
int
### getIconSetType() {#getIconSetType--}
```
public int getIconSetType()
```


Représente le type d'ensemble d'icônes.

Voir [IconSetType](../../com.aspose.cells/iconsettype).

**Remarks**

Ne prend effet que lorsque [getType()](../../com.aspose.cells/datasorterkey\#getType--) est [SortOnType.ICON](../../com.aspose.cells/sortontype\#ICON).

**Returns:**
int
### getIndex() {#getIndex--}
```
public int getIndex()
```


Obtient l'index de la colonne triée (position absolue, la colonne A est 0, B est 1, ...).

**Returns:**
int
### getOrder() {#getOrder--}
```
public int getOrder()
```


Indique l'ordre du tri.

Voir le [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Représente le type de tri.

Voir [SortOnType](../../com.aspose.cells/sortontype).

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

