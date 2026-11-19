---
title: "RevisionCellComment"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un enregistrement de révision d'une modification de commentaire de cellule."
type: docs
url: /fr/java/com.aspose.cells/revisioncellcomment/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellComment extends Revision
```

Représente un enregistrement de révision d'une modification de commentaire de cellule.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | Obtient le type d'action de la révision. |
| [getCellName()](#getCellName--) | Obtient le nom de la cellule. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Obtient l’indice de colonne de la cellule qui contient un commentaire. |
| [getId()](#getId--) | Obtient le numéro de cette révision. |
| [getNewLength()](#getNewLength--) | Obtient la longueur du commentaire avant que cette révision ne soit effectuée. |
| [getOldLength()](#getOldLength--) | Obtient la longueur du texte du commentaire ajouté dans cette révision. |
| [getRow()](#getRow--) | Obtient l’indice de ligne de la cellule qui contient un commentaire. |
| [getType()](#getType--) | Obtient le type de révision. |
| [getWorksheet()](#getWorksheet--) | Obtient la feuille de calcul. |
| [hashCode()](#hashCode--) |  |
| [isOldComment()](#isOldComment--) | Indique s’il s’agit d’un ancien commentaire. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCellName(String value)](#setCellName-java.lang.String-) | Obtient le nom de la cellule. |
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


Obtient le type d'action de la révision.

Voir [RevisionActionType](../../com.aspose.cells/revisionactiontype).

**Returns:**
int
### getCellName() {#getCellName--}
```
public String getCellName()
```


Obtient le nom de la cellule.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Obtient l’indice de colonne de la cellule qui contient un commentaire.

**Returns:**
int
### getId() {#getId--}
```
public int getId()
```


Obtient le numéro de cette révision.

**Remarks**

Zéro signifie que cette révision ne contient pas d'ID.

**Returns:**
int
### getNewLength() {#getNewLength--}
```
public int getNewLength()
```


Obtient la longueur du commentaire avant que cette révision ne soit effectuée.

**Returns:**
int
### getOldLength() {#getOldLength--}
```
public int getOldLength()
```


Obtient la longueur du texte du commentaire ajouté dans cette révision.

**Returns:**
int
### getRow() {#getRow--}
```
public int getRow()
```


Obtient l’indice de ligne de la cellule qui contient un commentaire.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Obtient le type de révision.

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
### isOldComment() {#isOldComment--}
```
public boolean isOldComment()
```


Indique s’il s’agit d’un ancien commentaire.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCellName(String value) {#setCellName-java.lang.String-}
```
public void setCellName(String value)
```


Obtient le nom de la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

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

