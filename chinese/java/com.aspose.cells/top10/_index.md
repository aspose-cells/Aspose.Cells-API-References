---
title: "Top10"
second_title: "Aspose.Cells for Java API 参考"
description: "描述 Top10 条件格式规则。"
type: docs
url: /zh/java/com.aspose.cells/top10/
---

**Inheritance:**
java.lang.Object
```
public class Top10
```

描述 Top10 条件格式规则。此条件格式规则突出显示值位于指定的前 N 或后 N 区间的单元格。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
 
         //Sets the conditional format range.
         CellArea ca = CellArea.createCellArea(0, 0, 10, 10);
         fcs.addArea(ca);
 
         //Adds condition.
         int conditionIndex = fcs.addCondition(FormatConditionType.TOP_10, OperatorType.NONE, null, null);   
         //Sets the background color.
         FormatCondition fc = fcs.get(conditionIndex);
         fc.getStyle().setBackgroundColor(Color.getRed());
         Top10 top10 = fc.getTop10();
         //Set the Top N 
         top10.setRank(5);  
         //Saving the Excel file
         workbook.save("output.xls");
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Top10()](#Top10--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getRank()](#getRank--) | 获取 "top/bottom n" 条件格式规则中 "n" 的值。 |
| [hashCode()](#hashCode--) |  |
| [isBottom()](#isBottom--) | 获取 "top/bottom n" 规则是否为 "bottom n" 规则。 |
| [isPercent()](#isPercent--) | 获取 "top/bottom n" 规则是否为 "top/bottom n percent" 规则。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBottom(boolean value)](#setBottom-boolean-) | 设置 "top/bottom n" 规则是否为 "bottom n" 规则。 |
| [setPercent(boolean value)](#setPercent-boolean-) | 设置 "top/bottom n" 规则是否为 "top/bottom n percent" 规则。 |
| [setRank(int value)](#setRank-int-) | 设置 "top/bottom n" 条件格式规则中 "n" 的值。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Top10() {#Top10--}
```
public Top10()
```


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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getRank() {#getRank--}
```
public int getRank()
```


获取 "top/bottom n" 条件格式规则中 "n" 的值。如果 IsPercent 为 true，则该值必须在 0 到 100 之间。否则必须在 0 到 1000 之间。默认值为 10。

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBottom() {#isBottom--}
```
public boolean isBottom()
```


获取 "top/bottom n" 规则是否为 "bottom n" 规则。默认值为 false。

**Returns:**
boolean
### isPercent() {#isPercent--}
```
public boolean isPercent()
```


获取 "top/bottom n" 规则是否为 "top/bottom n percent" 规则。默认值为 false。

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




### setBottom(boolean value) {#setBottom-boolean-}
```
public void setBottom(boolean value)
```


设置 "top/bottom n" 规则是否为 "bottom n" 规则。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPercent(boolean value) {#setPercent-boolean-}
```
public void setPercent(boolean value)
```


设置 "top/bottom n" 规则是否为 "top/bottom n percent" 规则。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRank(int value) {#setRank-int-}
```
public void setRank(int value)
```


设置 "top/bottom n" 条件格式规则中 "n" 的值。如果 IsPercent 为 true，则该值必须在 0 到 100 之间。否则必须在 0 到 1000 之间。默认值为 10。

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

