---
title: "RevisionInsertDelete"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un enregistrement de révision d'une action d'insertion/suppression de ligne/colonne."
type: docs
url: /fr/java/com.aspose.cells/revisioninsertdelete/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionInsertDelete extends Revision
```

Représente un enregistrement de révision d'une action d'insertion/suppression de ligne/colonne.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | Obtient le type d'action de cette révision. |
| [getCellArea()](#getCellArea--) | Obtient la plage d'insertion/suppression. |
| [getClass()](#getClass--) |  |
| [getId()](#getId--) | Obtient le numéro de cette révision. |
| [getRevisions()](#getRevisions--) | Obtient la liste des révisions par cette opération. |
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
### getActionType() {#getActionType--}
```
public int getActionType()
```


Obtient le type d'action de cette révision.

Voir [RevisionActionType](../../com.aspose.cells/revisionactiontype).

**Returns:**
int
### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Obtient la plage d'insertion/suppression.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getId() {#getId--}
```
public int getId()
```


Obtient le numéro de cette révision.

**Remarks**

Zéro signifie que cette révision ne contient pas d'ID.

**Returns:**
int
### getRevisions() {#getRevisions--}
```
public RevisionCollection getRevisions()
```


Obtient la liste des révisions par cette opération.

**Returns:**
[RevisionCollection](../../com.aspose.cells/revisioncollection)
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

