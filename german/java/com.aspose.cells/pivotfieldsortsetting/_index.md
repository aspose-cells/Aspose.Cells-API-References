---
title: "PivotFieldSortSetting"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Einstellung für das Sortieren von Pivotfeldern dar."
type: docs
url: /de/java/com.aspose.cells/pivotfieldsortsetting/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldSortSetting
```

Stellt die Einstellung für das Sortieren von Pivotfeldern dar.

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
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCell()](#getCell--) | Sortiert nach den Werten in Zeile oder Spalte. |
| [getClass()](#getClass--) |  |
| [getFieldIndex()](#getFieldIndex--) | Stellt den Index des Feldes dar, nach dem sortiert wird |
| [getLineTypeSortedBy()](#getLineTypeSortedBy--) | Der Pivot-Zeilentyp, nach dem sortiert wird. |
| [getSortBy()](#getSortBy--) | Stellt den Index des Feldes dar, nach dem sortiert wird. |
| [getSortType()](#getSortType--) | Stellt den [SortOrder](../../com.aspose.cells/sortorder) dar. |
| [hashCode()](#hashCode--) |  |
| [isSimpleSort()](#isSimpleSort--) | Gibt an, ob ein einfacher Datensortiervorgang angewendet wird. |
| [isSortByLabels()](#isSortByLabels--) | Gibt an, ob das Feld nach sich selbst oder nach dem Datenfeld sortiert werden soll. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFieldIndex(int value)](#setFieldIndex-int-) | Stellt den Index des Feldes dar, nach dem sortiert wird |
| [setSimpleSort(boolean value)](#setSimpleSort-boolean-) | Gibt an, ob ein einfacher Datensortiervorgang angewendet wird. |
| [setSortBy(int value)](#setSortBy-int-) | Stellt den Index des Feldes dar, nach dem sortiert wird. |
| [setSortType(int value)](#setSortType-int-) | Stellt den [SortOrder](../../com.aspose.cells/sortorder) dar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCell() {#getCell--}
```
public String getCell()
```


Sortiert nach den Werten in Zeile oder Spalte.

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


Stellt den Index des Feldes dar, nach dem sortiert wird. -1 bedeutet, dass das PivotField nach den Bezeichnungen sortiert wird, andere Werte bedeuten, dass nach dem Datenfeld sortiert wird.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Stattdessen bitte die Eigenschaft PivotFieldSortSetting.SortBy verwenden. Diese Methode wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Returns:**
int
### getLineTypeSortedBy() {#getLineTypeSortedBy--}
```
public int getLineTypeSortedBy()
```


Der Pivot-Zeilentyp, nach dem sortiert wird.

Siehe [PivotLineType](../../com.aspose.cells/pivotlinetype).

**Remarks**

Funktioniert nur, wenn dieses Feld nicht nach Bezeichnungen sortiert wird.

**Returns:**
int
### getSortBy() {#getSortBy--}
```
public int getSortBy()
```


Stellt den Index des Feldes dar, nach dem sortiert wird. Ein Wert von -1 bedeutet, dass nach den eigenen Werten des Pivot-Elements sortiert wird. Bei einem Wert größer oder gleich Null stellt er den Index des Datenfeldes im Datenbereich dar.

**Returns:**
int
### getSortType() {#getSortType--}
```
public int getSortType()
```


Stellt den [SortOrder](../../com.aspose.cells/sortorder) dar.

Siehe [SortOrder](../../com.aspose.cells/sortorder).

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


Gibt an, ob ein einfacher Datensortiervorgang angewendet wird.

**Remarks**

Der Standardwert ist true.

**Returns:**
boolean
### isSortByLabels() {#isSortByLabels--}
```
public boolean isSortByLabels()
```


Gibt an, ob das Feld nach sich selbst oder nach dem Datenfeld sortiert werden soll.

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


Stellt den Index des Feldes dar, nach dem sortiert wird. -1 bedeutet, dass das PivotField nach den Bezeichnungen sortiert wird, andere Werte bedeuten, dass nach dem Datenfeld sortiert wird.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Stattdessen bitte die Eigenschaft PivotFieldSortSetting.SortBy verwenden. Diese Methode wird 12 Monate später, seit September 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setSimpleSort(boolean value) {#setSimpleSort-boolean-}
```
public void setSimpleSort(boolean value)
```


Gibt an, ob ein einfacher Datensortiervorgang angewendet wird.

**Remarks**

Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSortBy(int value) {#setSortBy-int-}
```
public void setSortBy(int value)
```


Stellt den Index des Feldes dar, nach dem sortiert wird. Ein Wert von -1 bedeutet, dass nach den eigenen Werten des Pivot-Elements sortiert wird. Bei einem Wert größer oder gleich Null stellt er den Index des Datenfeldes im Datenbereich dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setSortType(int value) {#setSortType-int-}
```
public void setSortType(int value)
```


Stellt den [SortOrder](../../com.aspose.cells/sortorder) dar.

Siehe [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

