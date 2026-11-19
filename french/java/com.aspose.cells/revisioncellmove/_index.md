---
title: "RevisionCellMove"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un enregistrement de révision sur des cellules qui ont été déplacées."
type: docs
url: /fr/java/com.aspose.cells/revisioncellmove/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellMove extends Revision
```

Représente un enregistrement de révision d'une ou plusieurs cellules déplacées.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDestinationArea()](#getDestinationArea--) | Obtient la zone de destination. |
| [getId()](#getId--) | Obtient le numéro de cette révision. |
| [getSourceArea()](#getSourceArea--) | Obtient la zone source. |
| [getSourceWorksheet()](#getSourceWorksheet--) | Obtient la feuille de calcul source. |
| [getType()](#getType--) | Représente le type de révision. |
| [getWorksheet()](#getWorksheet--) | Obtient la feuille de calcul. |
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
### getDestinationArea() {#getDestinationArea--}
```
public CellArea getDestinationArea()
```


Obtient la zone de destination.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getId() {#getId--}
```
public int getId()
```


Obtient le numéro de cette révision.

**Remarks**

Zéro signifie que cette révision ne contient pas d'ID.

**Returns:**
int
### getSourceArea() {#getSourceArea--}
```
public CellArea getSourceArea()
```


Obtient la zone source.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getSourceWorksheet() {#getSourceWorksheet--}
```
public Worksheet getSourceWorksheet()
```


Obtient la feuille de calcul source.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### getType() {#getType--}
```
public int getType()
```


Représente le type de révision.

Voir [RevisionType](../../com.aspose.cells/revisiontype).

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Obtient la feuille de calcul.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
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

