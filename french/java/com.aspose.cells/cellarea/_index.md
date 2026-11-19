---
title: "CellArea"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente une zone de cellules."
type: docs
url: /fr/java/com.aspose.cells/cellarea/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public final class CellArea implements Comparable
```

Représente une zone de cellules.

**Example**

```
         //Create Cell Area
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
```
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [CellArea()](#CellArea--) |  |
## Champs

| Champ | Description |
| --- | --- |
| [EndColumn](#EndColumn) | Obtient ou définit la colonne de fin de cette zone. |
| [EndRow](#EndRow) | Obtient ou définit la ligne de fin de cette zone. |
| [StartColumn](#StartColumn) | Obtient ou définit la colonne de départ de cette zone. |
| [StartRow](#StartRow) | Obtient ou définit la ligne de départ de cette zone. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [compareTo(Object obj)](#compareTo-java.lang.Object-) | Compare deux objets CellArea selon leur coin supérieur gauche. |
| [createCellArea(int startRow, int startColumn, int endRow, int endColumn)](#createCellArea-int-int-int-int-) | Crée une zone de cellules. |
| [createCellArea(String startCellName, String endCellName)](#createCellArea-java.lang.String-java.lang.String-) | Crée une zone de cellules. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | Renvoie une chaîne qui représente l'objet de zone de cellules actuel. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CellArea() {#CellArea--}
```
public CellArea()
```


### EndColumn {#EndColumn}
```
public int EndColumn
```


Obtient ou définit la colonne de fin de cette zone.

### EndRow {#EndRow}
```
public int EndRow
```


Obtient ou définit la ligne de fin de cette zone.

### StartColumn {#StartColumn}
```
public int StartColumn
```


Obtient ou définit la colonne de départ de cette zone.

### StartRow {#StartRow}
```
public int StartRow
```


Obtient ou définit la ligne de départ de cette zone.

### compareTo(Object obj) {#compareTo-java.lang.Object-}
```
public int compareTo(Object obj)
```


Compare deux objets CellArea selon leur coin supérieur gauche.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
int - Si deux coins sont dans des lignes différentes, comparez alors leur indice de ligne. Sinon comparez leur indice de colonne. Si les deux coins sont identiques, 0 sera renvoyé.
### createCellArea(int startRow, int startColumn, int endRow, int endColumn) {#createCellArea-int-int-int-int-}
```
public static CellArea createCellArea(int startRow, int startColumn, int endRow, int endColumn)
```


Crée une zone de cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | La ligne de départ. |
| startColumn | int | La colonne de départ. |
| endRow | int | La ligne de fin. |
| endColumn | int | La colonne de fin. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Return a [CellArea](../../com.aspose.cells/cellarea).
### createCellArea(String startCellName, String endCellName) {#createCellArea-java.lang.String-java.lang.String-}
```
public static CellArea createCellArea(String startCellName, String endCellName)
```


Crée une zone de cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startCellName | java.lang.String | La cellule en haut à gauche de la plage. |
| endCellName | java.lang.String | La cellule en bas à droite de la plage. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Return a [CellArea](../../com.aspose.cells/cellarea).
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


Renvoie une chaîne qui représente l'objet de zone de cellules actuel.

**Returns:**
java.lang.String -
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

