---
title: "PivotFieldSortSetting"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar inställningen för sortering av pivottfält."
type: docs
url: /sv/java/com.aspose.cells/pivotfieldsortsetting/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldSortSetting
```

Representerar inställningen för sortering av pivottfält.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCell()](#getCell--) | Sorterar efter värdena i vilken rad eller kolumn. |
| [getClass()](#getClass--) |  |
| [getFieldIndex()](#getFieldIndex--) | Representerar indexet för fältet som sorteras efter |
| [getLineTypeSortedBy()](#getLineTypeSortedBy--) | Pivotlinjetypen som sorteras efter. |
| [getSortBy()](#getSortBy--) | Representerar indexet för fältet som sorteras efter. |
| [getSortType()](#getSortType--) | Representerar [SortOrder](../../com.aspose.cells/sortorder). |
| [hashCode()](#hashCode--) |  |
| [isSimpleSort()](#isSimpleSort--) | Anger om en enkel datasorteringsoperation kommer att tillämpas. |
| [isSortByLabels()](#isSortByLabels--) | Anger om fältet ska sorteras efter sig självt eller efter datafältet. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFieldIndex(int value)](#setFieldIndex-int-) | Representerar indexet för fältet som sorteras efter |
| [setSimpleSort(boolean value)](#setSimpleSort-boolean-) | Anger om en enkel datasorteringsoperation kommer att tillämpas. |
| [setSortBy(int value)](#setSortBy-int-) | Representerar indexet för fältet som sorteras efter. |
| [setSortType(int value)](#setSortType-int-) | Representerar [SortOrder](../../com.aspose.cells/sortorder). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCell() {#getCell--}
```
public String getCell()
```


Sorterar efter värdena i vilken rad eller kolumn.

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


Representerar indexet för fältet som sorteras efter. -1 betyder att PivotField sorteras efter etiketter, andra värden betyder sortering efter datafältet.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotFieldSortSetting.SortBy-egenskapen. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getLineTypeSortedBy() {#getLineTypeSortedBy--}
```
public int getLineTypeSortedBy()
```


Pivotlinjetypen som sorteras efter.

Se [PivotLineType](../../com.aspose.cells/pivotlinetype).

**Remarks**

Fungerar endast när detta fält inte sorteras efter etiketter.

**Returns:**
int
### getSortBy() {#getSortBy--}
```
public int getSortBy()
```


Representerar indexet för fältet som sorteras efter. Ett värde på -1 indikerar sortering efter pivot-objektets egna värden. När värdet är större än eller lika med noll representerar det indexet för datafältet i dataområdet.

**Returns:**
int
### getSortType() {#getSortType--}
```
public int getSortType()
```


Representerar [SortOrder](../../com.aspose.cells/sortorder).

Se [SortOrder](../../com.aspose.cells/sortorder).

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


Anger om en enkel datasorteringsoperation kommer att tillämpas.

**Remarks**

Standardvärdet är true.

**Returns:**
boolean
### isSortByLabels() {#isSortByLabels--}
```
public boolean isSortByLabels()
```


Anger om fältet ska sorteras efter sig självt eller efter datafältet.

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


Representerar indexet för fältet som sorteras efter. -1 betyder att PivotField sorteras efter etiketter, andra värden betyder sortering efter datafältet.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotFieldSortSetting.SortBy-egenskapen. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSimpleSort(boolean value) {#setSimpleSort-boolean-}
```
public void setSimpleSort(boolean value)
```


Anger om en enkel datasorteringsoperation kommer att tillämpas.

**Remarks**

Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSortBy(int value) {#setSortBy-int-}
```
public void setSortBy(int value)
```


Representerar indexet för fältet som sorteras efter. Ett värde på -1 indikerar sortering efter pivot-objektets egna värden. När värdet är större än eller lika med noll representerar det indexet för datafältet i dataområdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSortType(int value) {#setSortType-int-}
```
public void setSortType(int value)
```


Representerar [SortOrder](../../com.aspose.cells/sortorder).

Se [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

