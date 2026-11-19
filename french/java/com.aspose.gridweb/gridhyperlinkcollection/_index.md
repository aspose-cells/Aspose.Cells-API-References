---
title: "GridHyperlinkCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule une collection d'objets."
type: docs
url: /fr/java/com.aspose.gridweb/gridhyperlinkcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridHyperlinkCollection
```

Encapsule une collection d'objets [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)](#add-int-int-int-int-java.lang.String-) | Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules. |
| [add(String cellName, int totalRows, int totalColumns, String address)](#add-java.lang.String-int-int-java.lang.String-) | Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules. |
| [add(String cellName, String address)](#add-java.lang.String-java.lang.String-) | Ajoute un hyperlien à une cellule spécifiée. |
| [add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)](#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules. |
| [clear()](#clear--) | Efface tous les hyperliens. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient l'élément [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) à l'index spécifié. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient la taille de l'énumérateur |
| [getHyperlink(GridCell cell)](#getHyperlink-com.aspose.gridweb.GridCell-) | Obtient l'objet Hyperlink de la cellule. |
| [getHyperlink(int row, int column)](#getHyperlink-int-int-) | Obtient l'objet Hyperlink de la cellule. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(GridCellArea area)](#remove-com.aspose.gridweb.GridCellArea-) | Supprime l'hyperlien à la zone spécifiée. |
| [removeAt(int index)](#removeAt-int-) | Supprime l'hyperlien à l'index spécifié. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address) {#add-int-int-int-int-java.lang.String-}
```
public int add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)
```


Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | int | Première ligne de la plage d'hyperliens. |
| firstColumn | int | Première colonne de la plage d'hyperliens. |
| totalRows | int | Nombre de lignes dans cette plage d'hyperliens. |
| totalColumns | int | Nombre de colonnes de cette plage d'hyperliens. |
| adresse | java.lang.String | Adresse du lien hypertexte. |

**Returns:**
int - index de l'objet [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
### add(String cellName, int totalRows, int totalColumns, String address) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String cellName, int totalRows, int totalColumns, String address)
```


Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Nom de cellule. |
| totalRows | int | Nombre de lignes dans cette plage d'hyperliens. |
| totalColumns | int | Nombre de colonnes de cette plage d'hyperliens. |
| adresse | java.lang.String | Adresse du lien hypertexte. |

**Returns:**
int - index de l'objet [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
### add(String cellName, String address) {#add-java.lang.String-java.lang.String-}
```
public int add(String cellName, String address)
```


Ajoute un hyperlien à une cellule spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Nom de cellule. |
| adresse | java.lang.String | Adresse du lien hypertexte. |

**Returns:**
int - index de l'objet [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
### add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip) {#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)
```


Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startCellName | java.lang.String | La cellule en haut à gauche de la plage. |
| endCellName | java.lang.String | La cellule en bas à droite de la plage. |
| adresse | java.lang.String | Adresse du lien hypertexte. |
| textToDisplay | java.lang.String | Le texte à afficher pour le lien hypertexte spécifié. |
| screenTip | java.lang.String | Le texte d’infobulle pour le lien hypertexte spécifié. |

**Returns:**
int - index de l'objet [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
### clear() {#clear--}
```
public void clear()
```


Efface tous les hyperliens.

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
### get(int index) {#get-int-}
```
public GridHyperlink get(int index)
```


Obtient l'élément [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de base zéro de l'élément. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - The element at the specified index.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Obtient la taille de l'énumérateur

**Returns:**
int
### getHyperlink(GridCell cell) {#getHyperlink-com.aspose.gridweb.GridCell-}
```
public GridHyperlink getHyperlink(GridCell cell)
```


Obtient l'objet Hyperlink de la cellule. S'il n'y a pas d'Hyperlink pour la cellule, renvoie null.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cell | [GridCell](../../com.aspose.gridweb/gridcell) | L'objet GridCell. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) the GridHyperlink object.
### getHyperlink(int row, int column) {#getHyperlink-int-int-}
```
public GridHyperlink getHyperlink(int row, int column)
```


Obtient l'objet Hyperlink de la cellule. S'il n'y a pas d'Hyperlink pour la cellule, renvoie null.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | La ligne de la cellule. |
| colonne | int | La colonne de la cellule. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) the GridHyperlink object.
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




### remove(GridCellArea area) {#remove-com.aspose.gridweb.GridCellArea-}
```
public void remove(GridCellArea area)
```


Supprime l'hyperlien à la zone spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | La zone qui contient le lien hypertexte. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Supprime l'hyperlien à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de base zéro de l'élément. |

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

