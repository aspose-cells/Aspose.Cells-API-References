---
title: "SlicerCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Spécifie la collection de tous les objets Slicer sur la feuille de calcul spécifiée."
type: docs
url: /fr/java/com.aspose.cells/slicercollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SlicerCollection extends CollectionBase
```

Spécifie la collection de tous les objets Slicer sur la feuille de calcul spécifiée.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
 
         SlicerCollection slicers = sheet.getSlicers();
         int slicerIndex = slicers.add(pivot, "E12", "fruit");
         Slicer slicer = slicers.get(slicerIndex);
 
         //do your business
 
         book.save("out.xlsx");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(ListObject table, ListColumn listColumn, int row, int column)](#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-int-int-) | Ajouter un nouveau Slicer en utilisant ListObjet comme source de données |
| [add(ListObject table, ListColumn listColumn, String destCellName)](#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-java.lang.String-) | Ajouter un nouveau Slicer en utilisant ListObjet comme source de données |
| [add(ListObject table, int index, String destCellName)](#add-com.aspose.cells.ListObject-int-java.lang.String-) | Ajouter un nouveau Slicer en utilisant ListObjet comme source de données |
| [add(PivotTable pivot, int row, int column, PivotField baseField)](#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-) | Ajouter un nouveau Slicer en utilisant PivotTable comme source de données |
| [add(PivotTable pivot, int row, int column, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-int-int-int-) | Ajouter un nouveau Slicer en utilisant PivotTable comme source de données |
| [add(PivotTable pivot, int row, int column, String baseFieldName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | Ajouter un nouveau Slicer en utilisant PivotTable comme source de données |
| [add(PivotTable pivot, String destCellName, PivotField baseField)](#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-) | Ajouter un nouveau Slicer en utilisant PivotTable comme source de données |
| [add(PivotTable pivot, String destCellName, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-java.lang.String-int-) | Ajouter un nouveau Slicer en utilisant PivotTable comme source de données |
| [add(PivotTable pivot, String destCellName, String baseFieldName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | Ajouter un nouveau Slicer en utilisant PivotTable comme source de données |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [clear()](#clear--) | Effacer tous les Slicers. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient le Slicer par index. |
| [get(String name)](#get-java.lang.String-) | Obtient le Slicer par le nom du slicer. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt l'instance CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Slicer slicer)](#remove-com.aspose.cells.Slicer-) | Supprimer le Slicer spécifié |
| [removeAt(int index)](#removeAt-int-) | Supprime le Slicer à l'index spécifié |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(ListObject table, ListColumn listColumn, int row, int column) {#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-int-int-}
```
public int add(ListObject table, ListColumn listColumn, int row, int column)
```


Ajouter un nouveau Slicer en utilisant ListObjet comme source de données

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | Objet ListObject |
| listColumn | [ListColumn](../../com.aspose.cells/listcolumn) | La ListColumn dans ListObject.ListColumns |
| ligne | int | Indice de ligne de la cellule dans le coin supérieur gauche de la plage du Slicer. |
| colonne | int | Indice de colonne de la cellule dans le coin supérieur gauche de la plage du Slicer. |

**Returns:**
int - Le nouvel indice du Slicer ajouté
### add(ListObject table, ListColumn listColumn, String destCellName) {#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-java.lang.String-}
```
public int add(ListObject table, ListColumn listColumn, String destCellName)
```


Ajouter un nouveau Slicer en utilisant ListObjet comme source de données

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | Objet ListObject |
| listColumn | [ListColumn](../../com.aspose.cells/listcolumn) | La ListColumn dans ListObject.ListColumns |
| destCellName | java.lang.String | La cellule dans le coin supérieur gauche de la plage du Slicer. |

**Returns:**
int - Le nouvel indice du Slicer ajouté
### add(ListObject table, int index, String destCellName) {#add-com.aspose.cells.ListObject-int-java.lang.String-}
```
public int add(ListObject table, int index, String destCellName)
```


Ajouter un nouveau Slicer en utilisant ListObjet comme source de données

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | Objet ListObject |
| index | int | L'indice de ListColumn dans ListObject.ListColumns |
| destCellName | java.lang.String | La cellule dans le coin supérieur gauche de la plage du Slicer. |

**Returns:**
int - Le nouvel indice du Slicer ajouté
### add(PivotTable pivot, int row, int column, PivotField baseField) {#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, int row, int column, PivotField baseField)
```


Ajouter un nouveau Slicer en utilisant PivotTable comme source de données

**Example**

```
         slicers.add(pivot, 3, 12, pivot.getBaseFields().get(0));
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Objet PivotTable |
| ligne | int | Indice de ligne de la cellule dans le coin supérieur gauche de la plage du Slicer. |
| colonne | int | Indice de colonne de la cellule dans le coin supérieur gauche de la plage du Slicer. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | Le PivotField dans PivotTable.BaseFields |

**Returns:**
int - Le nouvel indice du Slicer ajouté
### add(PivotTable pivot, int row, int column, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-int-int-int-}
```
public int add(PivotTable pivot, int row, int column, int baseFieldIndex)
```


Ajouter un nouveau Slicer en utilisant PivotTable comme source de données

**Example**

```
         slicers.add(pivot, 20, 8, 0);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Objet PivotTable |
| ligne | int | Indice de ligne de la cellule dans le coin supérieur gauche de la plage du Slicer. |
| colonne | int | Indice de colonne de la cellule dans le coin supérieur gauche de la plage du Slicer. |
| baseFieldIndex | int | L'index du PivotField dans PivotTable.BaseFields |

**Returns:**
int - Le nouvel indice du Slicer ajouté
### add(PivotTable pivot, int row, int column, String baseFieldName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivot, int row, int column, String baseFieldName)
```


Ajouter un nouveau Slicer en utilisant PivotTable comme source de données

**Example**

```
         slicers.add(pivot, 20, 12, "fruit");
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Objet PivotTable |
| ligne | int | Indice de ligne de la cellule dans le coin supérieur gauche de la plage du Slicer. |
| colonne | int | Indice de colonne de la cellule dans le coin supérieur gauche de la plage du Slicer. |
| baseFieldName | java.lang.String | Le nom du PivotField dans PivotTable.BaseFields |

**Returns:**
int - Le nouvel indice du Slicer ajouté
### add(PivotTable pivot, String destCellName, PivotField baseField) {#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, String destCellName, PivotField baseField)
```


Ajouter un nouveau Slicer en utilisant PivotTable comme source de données

**Example**

```
         slicers.add(pivot, "I3", pivot.getBaseFields().get(0));
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Objet PivotTable |
| destCellName | java.lang.String | La cellule dans le coin supérieur gauche de la plage du Slicer. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | Le PivotField dans PivotTable.BaseFields |

**Returns:**
int - Le nouvel indice du Slicer ajouté
### add(PivotTable pivot, String destCellName, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-java.lang.String-int-}
```
public int add(PivotTable pivot, String destCellName, int baseFieldIndex)
```


Ajouter un nouveau Slicer en utilisant PivotTable comme source de données

**Example**

```
         slicers.add(pivot, "E20", 0);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Objet PivotTable |
| destCellName | java.lang.String | La cellule dans le coin supérieur gauche de la plage du Slicer. |
| baseFieldIndex | int | L'index du PivotField dans PivotTable.BaseFields |

**Returns:**
int - Le nouvel indice du Slicer ajouté
### add(PivotTable pivot, String destCellName, String baseFieldName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivot, String destCellName, String baseFieldName)
```


Ajouter un nouveau Slicer en utilisant PivotTable comme source de données

**Example**

```
         slicers.add(pivot, "E3", "fruit");
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | Objet PivotTable |
| destCellName | java.lang.String | La cellule dans le coin supérieur gauche de la plage du Slicer. |
| baseFieldName | java.lang.String | Le nom du PivotField dans PivotTable.BaseFields |

**Returns:**
int - Le nouvel indice du Slicer ajouté
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


Effacer tous les Slicers.

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
### get(int index) {#get-int-}
```
public Slicer get(int index)
```


Obtient le Slicer par index.

**Example**

```
         Slicer slicerByIndex = slicers.get(0);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int |  |

**Returns:**
[Slicer](../../com.aspose.cells/slicer)
### get(String name) {#get-java.lang.String-}
```
public Slicer get(String name)
```


Obtient le Slicer par le nom du slicer.

**Example**

```
         Slicer slicerByName = slicers.get("fruit");
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[Slicer](../../com.aspose.cells/slicer)
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




### remove(Slicer slicer) {#remove-com.aspose.cells.Slicer-}
```
public void remove(Slicer slicer)
```


Supprimer le Slicer spécifié

**Example**

```
         Slicer delSlicer = slicers.get(0);
         slicers.remove(delSlicer);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| slicer | [Slicer](../../com.aspose.cells/slicer) | L'objet Slicer |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Supprime le Slicer à l'index spécifié

**Example**

```
         slicers.removeAt(1);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de position dans la collection Slicer |

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

