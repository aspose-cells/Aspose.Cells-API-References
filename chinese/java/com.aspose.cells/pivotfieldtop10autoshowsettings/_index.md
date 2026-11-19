---
title: "PivotFieldTop10AutoShowSettings"
second_title: "Aspose.Cells for Java API 参考"
description: "表示数据透视字段的前 10 项自动显示设置。"
type: docs
url: /zh/java/com.aspose.cells/pivotfieldtop10autoshowsettings/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldTop10AutoShowSettings
```

表示数据透视字段的前 10 项自动显示设置。

**Remarks**

在 xls 中：通过 Top 10 AutoShow 在 Xls 中实现前 10 过滤器。在 ooxml 文件中：底层 ooxml 文件格式支持 Top10 AutoShow，但 Excel 2007 及更高版本的用户界面仅通过 Top10 过滤器提供访问。如果不需要 XLS 兼容性，建议改用 Top10 过滤器。

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
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoShowCount()](#getAutoShowCount--) | 表示在指定的 PivotTable 字段中自动显示的前或后项目的数量。 |
| [getClass()](#getClass--) |  |
| [getRankBy()](#getRankBy--) | 指定用于 AutoShow 排名的数据字段索引。 |
| [hashCode()](#hashCode--) |  |
| [isAutoShow()](#isAutoShow--) | 指示是否对该字段应用了 "Top 10 AutoShow" 过滤器。 |
| [isTop()](#isTop--) | 指示指定的 PivotTable 字段是否以升序自动显示。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | 指示是否对该字段应用了 "Top 10 AutoShow" 过滤器。 |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | 表示在指定的 PivotTable 字段中自动显示的前或后项目的数量。 |
| [setRankBy(int value)](#setRankBy-int-) | 指定用于 AutoShow 排名的数据字段索引。 |
| [setTop(boolean value)](#setTop-boolean-) | 指示指定的 PivotTable 字段是否以升序自动显示。 |
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
### getAutoShowCount() {#getAutoShowCount--}
```
public int getAutoShowCount()
```


表示在指定的 PivotTable 字段中自动显示的前或后项目的数量。

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


指定用于 AutoShow 排名的数据字段索引。表示自动显示字段索引。-1 表示 PivotField 本身。它应当是数据字段的索引。

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


指示是否对该字段应用了 "Top 10 AutoShow" 过滤器。

**Returns:**
boolean
### isTop() {#isTop--}
```
public boolean isTop()
```


指示指定的 PivotTable 字段是否以升序自动显示。

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


指示是否对该字段应用了 "Top 10 AutoShow" 过滤器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutoShowCount(int value) {#setAutoShowCount-int-}
```
public void setAutoShowCount(int value)
```


表示在指定的 PivotTable 字段中自动显示的前或后项目的数量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setRankBy(int value) {#setRankBy-int-}
```
public void setRankBy(int value)
```


指定用于 AutoShow 排名的数据字段索引。表示自动显示字段索引。-1 表示 PivotField 本身。它应当是数据字段的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTop(boolean value) {#setTop-boolean-}
```
public void setTop(boolean value)
```


指示指定的 PivotTable 字段是否以升序自动显示。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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

