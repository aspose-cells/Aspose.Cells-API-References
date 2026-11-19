---
title: "PivotFieldSortSetting"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le paramètre de tri des champs pivot."
type: docs
url: /fr/java/com.aspose.cells/pivotfieldsortsetting/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldSortSetting
```

Représente le paramètre de tri des champs pivot.

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
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Sort by the first data field ascending.
         rowField.sortBy(SortOrder.ASCENDING, 0, null);
 
         //Gets sort settings of the pivot field.
         PivotFieldSortSetting sortSetting = rowField.getSortSetting();
         System.out.println(sortSetting.getSortType());
         //do your business
 
         pivot.calculateData();
         book.save("out.xlsx");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCell()](#getCell--) | Trie par les valeurs dans la ligne ou la colonne. |
| [getClass()](#getClass--) |  |
| [getFieldIndex()](#getFieldIndex--) | Représente l’index du champ trié par |
| [getLineTypeSortedBy()](#getLineTypeSortedBy--) | Le type de ligne de tableau croisé dynamique trié par. |
| [getSortBy()](#getSortBy--) | Représente l’index du champ trié par. |
| [getSortType()](#getSortType--) | Représente le [SortOrder](../../com.aspose.cells/sortorder). |
| [hashCode()](#hashCode--) |  |
| [isSimpleSort()](#isSimpleSort--) | Indique si une opération de tri simple des données sera appliquée. |
| [isSortByLabels()](#isSortByLabels--) | Indique s’il faut trier le champ par lui-même ou par le champ de données. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFieldIndex(int value)](#setFieldIndex-int-) | Représente l’index du champ trié par |
| [setSimpleSort(boolean value)](#setSimpleSort-boolean-) | Indique si une opération de tri simple des données sera appliquée. |
| [setSortBy(int value)](#setSortBy-int-) | Représente l’index du champ trié par. |
| [setSortType(int value)](#setSortType-int-) | Représente le [SortOrder](../../com.aspose.cells/sortorder). |
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
### getCell() {#getCell--}
```
public String getCell()
```


Trie par les valeurs dans la ligne ou la colonne.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Représente l’index du champ trié par. -1 signifie trier le PivotField par les libellés, d’autres valeurs signifient trier par le champ de données.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotFieldSortSetting.SortBy. Cette méthode sera supprimée 12 mois plus tard, à compter de septembre 2026. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getLineTypeSortedBy() {#getLineTypeSortedBy--}
```
public int getLineTypeSortedBy()
```


Le type de ligne de tableau croisé dynamique trié par.

Voir le [PivotLineType](../../com.aspose.cells/pivotlinetype).

**Remarks**

Fonctionne uniquement lorsque ce champ n’est pas trié par les libellés.

**Returns:**
int
### getSortBy() {#getSortBy--}
```
public int getSortBy()
```


Représente l’index du champ trié par. Une valeur de -1 indique un tri par les propres valeurs de l’élément de tableau croisé dynamique. Lorsqu’elle est supérieure ou égale à zéro, elle représente l’index du champ de données dans la région des données.

**Returns:**
int
### getSortType() {#getSortType--}
```
public int getSortType()
```


Représente le [SortOrder](../../com.aspose.cells/sortorder).

Voir le [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isSimpleSort() {#isSimpleSort--}
```
public boolean isSimpleSort()
```


Indique si une opération de tri simple des données sera appliquée.

**Remarks**

La valeur par défaut est true.

**Returns:**
boolean
### isSortByLabels() {#isSortByLabels--}
```
public boolean isSortByLabels()
```


Indique s’il faut trier le champ par lui-même ou par le champ de données.

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




### setFieldIndex(int value) {#setFieldIndex-int-}
```
public void setFieldIndex(int value)
```


Représente l’index du champ trié par. -1 signifie trier le PivotField par les libellés, d’autres valeurs signifient trier par le champ de données.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotFieldSortSetting.SortBy. Cette méthode sera supprimée 12 mois plus tard, à compter de septembre 2026. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSimpleSort(boolean value) {#setSimpleSort-boolean-}
```
public void setSimpleSort(boolean value)
```


Indique si une opération de tri simple des données sera appliquée.

**Remarks**

La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSortBy(int value) {#setSortBy-int-}
```
public void setSortBy(int value)
```


Représente l’index du champ trié par. Une valeur de -1 indique un tri par les propres valeurs de l’élément de tableau croisé dynamique. Lorsqu’elle est supérieure ou égale à zéro, elle représente l’index du champ de données dans la région des données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSortType(int value) {#setSortType-int-}
```
public void setSortType(int value)
```


Représente le [SortOrder](../../com.aspose.cells/sortorder).

Voir le [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

