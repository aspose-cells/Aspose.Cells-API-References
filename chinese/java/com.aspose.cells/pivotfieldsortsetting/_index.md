---
title: "PivotFieldSortSetting"
second_title: "Aspose.Cells for Java API 参考"
description: "表示用于对数据透视字段排序的设置。"
type: docs
url: /zh/java/com.aspose.cells/pivotfieldsortsetting/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldSortSetting
```

表示用于对数据透视字段排序的设置。

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
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCell()](#getCell--) | 按行或列中的值进行排序。 |
| [getClass()](#getClass--) |  |
| [getFieldIndex()](#getFieldIndex--) | 表示排序字段的索引 |
| [getLineTypeSortedBy()](#getLineTypeSortedBy--) | 表示排序的透视线类型。 |
| [getSortBy()](#getSortBy--) | 表示排序字段的索引。 |
| [getSortType()](#getSortType--) | 表示 [SortOrder](../../com.aspose.cells/sortorder)。 |
| [hashCode()](#hashCode--) |  |
| [isSimpleSort()](#isSimpleSort--) | 指示是否将应用简单的数据排序操作。 |
| [isSortByLabels()](#isSortByLabels--) | 指示是按字段本身还是按数据字段进行排序。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFieldIndex(int value)](#setFieldIndex-int-) | 表示排序字段的索引 |
| [setSimpleSort(boolean value)](#setSimpleSort-boolean-) | 指示是否将应用简单的数据排序操作。 |
| [setSortBy(int value)](#setSortBy-int-) | 表示排序字段的索引。 |
| [setSortType(int value)](#setSortType-int-) | 表示 [SortOrder](../../com.aspose.cells/sortorder)。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCell() {#getCell--}
```
public String getCell()
```


按行或列中的值进行排序。

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


表示排序字段的索引。-1 表示按标签对 PivotField 排序，其他值表示按数据字段排序。

**Remarks**

注意：此属性已过时。请改用 PivotFieldSortSetting.SortBy 属性。该方法将在自2026年9月起的12个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getLineTypeSortedBy() {#getLineTypeSortedBy--}
```
public int getLineTypeSortedBy()
```


表示排序的透视线类型。

参见 [PivotLineType](../../com.aspose.cells/pivotlinetype)。

**Remarks**

仅在未按标签对该字段进行排序时有效。

**Returns:**
int
### getSortBy() {#getSortBy--}
```
public int getSortBy()
```


表示排序字段的索引。-1 表示按透视项自身的值排序。大于或等于零时，表示数据区域中数据字段的索引。

**Returns:**
int
### getSortType() {#getSortType--}
```
public int getSortType()
```


表示 [SortOrder](../../com.aspose.cells/sortorder)。

参见 [SortOrder](../../com.aspose.cells/sortorder)。

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


指示是否将应用简单的数据排序操作。

**Remarks**

默认值为 true。

**Returns:**
boolean
### isSortByLabels() {#isSortByLabels--}
```
public boolean isSortByLabels()
```


指示是按字段本身还是按数据字段进行排序。

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


表示排序字段的索引。-1 表示按标签对 PivotField 排序，其他值表示按数据字段排序。

**Remarks**

注意：此属性已过时。请改用 PivotFieldSortSetting.SortBy 属性。该方法将在自2026年9月起的12个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSimpleSort(boolean value) {#setSimpleSort-boolean-}
```
public void setSimpleSort(boolean value)
```


指示是否将应用简单的数据排序操作。

**Remarks**

默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSortBy(int value) {#setSortBy-int-}
```
public void setSortBy(int value)
```


表示排序字段的索引。-1 表示按透视项自身的值排序。大于或等于零时，表示数据区域中数据字段的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSortType(int value) {#setSortType-int-}
```
public void setSortType(int value)
```


表示 [SortOrder](../../com.aspose.cells/sortorder)。

参见 [SortOrder](../../com.aspose.cells/sortorder)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

