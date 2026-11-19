---
title: "RevisionCellChange"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente la révision qui modifie les cellules."
type: docs
url: /fr/java/com.aspose.cells/revisioncellchange/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellChange extends Revision
```

Représente la révision qui modifie les cellules.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellName()](#getCellName--) | Obtient le nom de la cellule. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Obtient l'index de colonne de la cellule. |
| [getId()](#getId--) | Obtient le numéro de cette révision. |
| [getNewFormula()](#getNewFormula--) | Obtient l'ancienne formule. |
| [getNewStyle()](#getNewStyle--) | Obtient le nouveau style de la cellule. |
| [getNewValue()](#getNewValue--) | Obtient la nouvelle valeur de la cellule. |
| [getOldFormula()](#getOldFormula--) | Obtient l'ancienne formule. |
| [getOldStyle()](#getOldStyle--) | Obtient l'ancien style de la cellule. |
| [getOldValue()](#getOldValue--) | Obtient l'ancienne valeur de la cellule. |
| [getRow()](#getRow--) | Obtient l'index de ligne de la cellule. |
| [getType()](#getType--) | Représente le type de révision. |
| [getWorksheet()](#getWorksheet--) | Obtient la feuille de calcul. |
| [hashCode()](#hashCode--) |  |
| [isNewFormatted()](#isNewFormatted--) | Indique si cette cellule est formatée comme nouvelle. |
| [isOldFormatted()](#isOldFormatted--) | Indique si cette cellule est formatée comme ancienne. |
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


Obtient l'index de colonne de la cellule.

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
### getNewFormula() {#getNewFormula--}
```
public String getNewFormula()
```


Obtient l'ancienne formule.

**Returns:**
java.lang.String
### getNewStyle() {#getNewStyle--}
```
public Style getNewStyle()
```


Obtient le nouveau style de la cellule.

**Returns:**
[Style](../../com.aspose.cells/style)
### getNewValue() {#getNewValue--}
```
public Object getNewValue()
```


Obtient la nouvelle valeur de la cellule.

**Returns:**
java.lang.Object
### getOldFormula() {#getOldFormula--}
```
public String getOldFormula()
```


Obtient l'ancienne formule.

**Returns:**
java.lang.String
### getOldStyle() {#getOldStyle--}
```
public Style getOldStyle()
```


Obtient l'ancien style de la cellule.

**Returns:**
[Style](../../com.aspose.cells/style)
### getOldValue() {#getOldValue--}
```
public Object getOldValue()
```


Obtient l'ancienne valeur de la cellule.

**Returns:**
java.lang.Object
### getRow() {#getRow--}
```
public int getRow()
```


Obtient l'index de ligne de la cellule.

**Returns:**
int
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
### isNewFormatted() {#isNewFormatted--}
```
public boolean isNewFormatted()
```


Indique si cette cellule est formatée comme nouvelle.

**Returns:**
boolean
### isOldFormatted() {#isOldFormatted--}
```
public boolean isOldFormatted()
```


Indique si cette cellule est formatée comme ancienne.

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

