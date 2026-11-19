---
title: "PivotTableFormatCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente la collection de formats appliqués au tableau croisé dynamique."
type: docs
url: /fr/java/com.aspose.cells/pivottableformatcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotTableFormatCollection extends CollectionBase
```

Représente la collection de formats appliqués au tableau croisé dynamique.
## Méthodes

| Méthode | Description |
| --- | --- |
| [add()](#add--) | Ajoute un [PivotTableFormat](../../com.aspose.cells/pivottableformat). |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [clear()](#clear--) | Supprime tous les objets de l'instance CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [format(CellArea ca, Style style)](#format-com.aspose.cells.CellArea-com.aspose.cells.Style-) | Formate la zone sélectionnée du tableau croisé dynamique. |
| [format(PivotArea pivotArea, Style style)](#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-) | Formate la zone sélectionnée du tableau croisé dynamique. |
| [format(int row, int column, Style style)](#format-int-int-com.aspose.cells.Style-) | Formate la cellule dans la zone du tableau croisé dynamique |
| [formatArea(int axisType, int fieldPosition, int subtotalType, int selectionType, boolean isGrandRow, boolean isGrandColumn, Style style)](#formatArea-int-int-int-int-boolean-boolean-com.aspose.cells.Style-) | Formate la zone sélectionnée. |
| [get(int index)](#get-int-) | Obtient le format par l'index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt l'instance CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Supprime l'élément à l'index spécifié. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


Ajoute un [PivotTableFormat](../../com.aspose.cells/pivottableformat).

**Returns:**
int - L'index du nouveau format.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Ajoute un élément à l'instance CollectionBase.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | L'objet à ajouter à l'instance CollectionBase. |

**Returns:**
int - La position dans laquelle le nouvel élément a été inséré.
### clear() {#clear--}
```
public void clear()
```


Supprime tous les objets de l'instance CollectionBase.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Renvoie si l'instance contient cet objet

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | objet de test |

**Returns:**
boolean - Si l'instance contient cet objet
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
### format(CellArea ca, Style style) {#format-com.aspose.cells.CellArea-com.aspose.cells.Style-}
```
public void format(CellArea ca, Style style)
```


Formate la zone sélectionnée du tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | La plage des cellules. |
| style | [Style](../../com.aspose.cells/style) | Le style |

### format(PivotArea pivotArea, Style style) {#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-}
```
public void format(PivotArea pivotArea, Style style)
```


Formate la zone sélectionnée du tableau croisé dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pivotArea | [PivotArea](../../com.aspose.cells/pivotarea) | La zone de vue pivot sélectionnée. |
| style | [Style](../../com.aspose.cells/style) | Le paramètre formaté. |

### format(int row, int column, Style style) {#format-int-int-com.aspose.cells.Style-}
```
public void format(int row, int column, Style style)
```


Formate la cellule dans la zone du tableau croisé dynamique

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Index de ligne de la cellule |
| colonne | int | Indice de colonne de la cellule |
| style | [Style](../../com.aspose.cells/style) | Style utilisé pour formater la cellule |

### formatArea(int axisType, int fieldPosition, int subtotalType, int selectionType, boolean isGrandRow, boolean isGrandColumn, Style style) {#formatArea-int-int-int-int-boolean-boolean-com.aspose.cells.Style-}
```
public PivotTableFormat formatArea(int axisType, int fieldPosition, int subtotalType, int selectionType, boolean isGrandRow, boolean isGrandColumn, Style style)
```


Formate la zone sélectionnée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). La région du tableau croisé dynamique à laquelle cette règle s'applique. |
| fieldPosition | int | Position du champ dans l'axe auquel cette règle s'applique. |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Le type de filtre de sous-total du champ pivot. |
| selectionType | int | [PivotTableSelectionType](../../com.aspose.cells/pivottableselectiontype). Indique comment sélectionner les données. |
| isGrandRow | boolean | Indique si les lignes de total général sont sélectionnées. |
| isGrandColumn | boolean | Indique si les colonnes de total général sont sélectionnées. |
| style | [Style](../../com.aspose.cells/style) | Le style qui s'applique à la zone du tableau croisé dynamique. |

**Returns:**
[PivotTableFormat](../../com.aspose.cells/pivottableformat) - 
### get(int index) {#get-int-}
```
public PivotTableFormat get(int index)
```


Obtient le format par l'index.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index. |

**Returns:**
[PivotTableFormat](../../com.aspose.cells/pivottableformat) - 
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


Obtient le nombre d'éléments contenus dans l'instance CollectionBase.

**Returns:**
int - Le nombre d'éléments contenus dans l'instance CollectionBase.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Détermine l'index d'un élément spécifique dans l'instance CollectionBase.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |

**Returns:**
int - L'index de la valeur si elle est trouvée dans la liste ; sinon, -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Renvoie un énumérateur qui parcourt l'instance CollectionBase.

**Returns:**
java.util.Iterator - Un itérateur pour l'instance CollectionBase.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Supprime l'élément à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index basé sur zéro de l'élément à supprimer. |

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

