---
title: PivotFieldTop10AutoShowSettings
second_title: Aspose.Cells for Java API Reference
description: Represents the Top 10 AutoShow settings for a pivot field.
type: docs
url: /java/com.aspose.cells/pivotfieldtop10autoshowsettings/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldTop10AutoShowSettings
```

Represents the Top 10 AutoShow settings for a pivot field.

**Remarks**

In xls : Implementing top 10 filters in Xls through Top 10 AutoShow In ooxml files: The underlying ooxml file format supports Top10 AutoShow, but Excel 2007 and later user interface only provides access via Top10 filter. If XLS compatibility is not required, it is recommended to use Top10 filter instead.

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
 
         //Show top 2 items by row field label.
         rowField.top10AutoShow(true, true, 2, -1);
 
         PivotFieldTop10AutoShowSettings sortSetting = rowField.getTop10AutoShowSettings();
         System.out.println(sortSetting.isAutoShow());
 
          pivot.calculateData();
 
         book.save("out.xlsx");
```
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoShowCount()](#getAutoShowCount--) | Represent the number of top or bottom items that are automatically shown in the specified PivotTable field. |
| [getClass()](#getClass--) |  |
| [getRankBy()](#getRankBy--) | Specifies the index of data field for AutoShow ranking. |
| [hashCode()](#hashCode--) |  |
| [isAutoShow()](#isAutoShow--) | Indicates whether an "Top 10 AutoShow" filter is applied to this field. |
| [isTop()](#isTop--) | Indicates whether the specified PivotTable field is autoshown ascending. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | Indicates whether an "Top 10 AutoShow" filter is applied to this field. |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | Represent the number of top or bottom items that are automatically shown in the specified PivotTable field. |
| [setRankBy(int value)](#setRankBy-int-) | Specifies the index of data field for AutoShow ranking. |
| [setTop(boolean value)](#setTop-boolean-) | Indicates whether the specified PivotTable field is autoshown ascending. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAutoShowCount() {#getAutoShowCount--}
```
public int getAutoShowCount()
```


Represent the number of top or bottom items that are automatically shown in the specified PivotTable field.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getRankBy() {#getRankBy--}
```
public int getRankBy()
```


Specifies the index of data field for AutoShow ranking. Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoShow() {#isAutoShow--}
```
public boolean isAutoShow()
```


Indicates whether an "Top 10 AutoShow" filter is applied to this field.

**Returns:**
boolean
### isTop() {#isTop--}
```
public boolean isTop()
```


Indicates whether the specified PivotTable field is autoshown ascending.

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




### setAutoShow(boolean value) {#setAutoShow-boolean-}
```
public void setAutoShow(boolean value)
```


Indicates whether an "Top 10 AutoShow" filter is applied to this field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoShowCount(int value) {#setAutoShowCount-int-}
```
public void setAutoShowCount(int value)
```


Represent the number of top or bottom items that are automatically shown in the specified PivotTable field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRankBy(int value) {#setRankBy-int-}
```
public void setRankBy(int value)
```


Specifies the index of data field for AutoShow ranking. Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTop(boolean value) {#setTop-boolean-}
```
public void setTop(boolean value)
```


Indicates whether the specified PivotTable field is autoshown ascending.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

