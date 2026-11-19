---
title: "FormatConditionCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "表示条件格式。"
type: docs
url: /zh/java/com.aspose.cells/formatconditioncollection/
---

**Inheritance:**
java.lang.Object
```
public class FormatConditionCollection
```

表示条件格式。FormatConditions 最多可以包含三个条件格式。

**Example**

```
         //Create a new Workbook.
         Workbook workbook = new Workbook();
 
         //Get the first worksheet.
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
         //Sets the conditional format range.
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
         fcs.addArea(ca);
         ca = new CellArea();
         ca.StartRow = 1;
         ca.EndRow = 1;
         ca.StartColumn = 1;
         ca.EndColumn = 1;
         fcs.addArea(ca);
         //Adds condition.
         int conditionIndex = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100");
         //Adds condition.
         int conditionIndex2 = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100");
         //Sets the background color.
         FormatCondition fc = fcs.get(conditionIndex);
         fc.getStyle().setBackgroundColor(Color.getRed());
         //Saving the Excel file
         workbook.save("output.xls");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(CellArea cellArea, int type, int operatorType, String formula1, String formula2)](#add-com.aspose.cells.CellArea-int-int-java.lang.String-java.lang.String-) | 向 FormatConditions 添加一个格式条件和受影响的单元格范围。FormatConditions 最多可以包含三个条件格式。 |
| [addArea(CellArea cellArea)](#addArea-com.aspose.cells.CellArea-) | 添加条件格式化的单元格范围。 |
| [addCondition(int type)](#addCondition-int-) | 添加格式条件。 |
| [addCondition(int type, int operatorType, String formula1, String formula2)](#addCondition-int-int-java.lang.String-java.lang.String-) | 添加格式条件。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 通过索引获取格式条件。 |
| [getCellArea(int index)](#getCellArea-int-) | 通过索引获取条件格式化的单元格范围。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取条件的数量。 |
| [getRangeCount()](#getRangeCount--) | 获取条件格式化范围的数量。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeArea(int index)](#removeArea-int-) | 通过索引移除条件格式化的单元格范围。 |
| [removeArea(int startRow, int startColumn, int totalRows, int totalColumns)](#removeArea-int-int-int-int-) | 移除范围内的条件格式。 |
| [removeCondition(int index)](#removeCondition-int-) | 按索引删除格式条件。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(CellArea cellArea, int type, int operatorType, String formula1, String formula2) {#add-com.aspose.cells.CellArea-int-int-java.lang.String-java.lang.String-}
```
public int[] add(CellArea cellArea, int type, int operatorType, String formula1, String formula2)
```


向 FormatConditions 添加一个格式条件和受影响的单元格范围。FormatConditions 最多可以包含三个条件格式。条件格式的公式中不允许引用其他工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | 条件格式化的单元格范围。 |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). 条件格式的类型。它可以是 FormatConditionType 的成员之一。 |
| operatorType | int | [OperatorType](../../com.aspose.cells/operatortype). 比较运算符。它可以是 OperatorType 的成员之一。 |
| formula1 | java.lang.String | 与条件格式关联的值或表达式。 |
| formula2 | java.lang.String | 与条件格式关联的值或表达式 |

**Returns:**
int[] - [0]：格式条件对象索引；[1] 受影响的单元格范围索引。
### addArea(CellArea cellArea) {#addArea-com.aspose.cells.CellArea-}
```
public int addArea(CellArea cellArea)
```


添加条件格式化的单元格范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | 条件格式化的单元格范围。 |

**Returns:**
int - 条件格式化的单元格范围索引。
### addCondition(int type) {#addCondition-int-}
```
public int addCondition(int type)
```


添加格式条件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). 格式条件类型。 |

**Returns:**
int - 格式条件对象索引；
### addCondition(int type, int operatorType, String formula1, String formula2) {#addCondition-int-int-java.lang.String-java.lang.String-}
```
public int addCondition(int type, int operatorType, String formula1, String formula2)
```


添加格式条件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). 格式条件的类型。 |
| operatorType | int | [OperatorType](../../com.aspose.cells/operatortype). 运算符类型 |
| formula1 | java.lang.String | 与条件格式关联的值或表达式。如果输入值以 '=' 开头，则视为公式。否则视为普通值（文本、数字、布尔）。对于以 '=' 开头的文本值，用户可以按以下格式输入公式：\"=\\\"=...\\\"\"。 |
| formula2 | java.lang.String | 与条件格式关联的值或表达式。输入格式与 formula1 相同。 |

**Returns:**
int - 格式条件对象索引；
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
### get(int index) {#get-int-}
```
public FormatCondition get(int index)
```


通过索引获取格式条件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 要返回的格式条件的索引。 |

**Returns:**
[FormatCondition](../../com.aspose.cells/formatcondition) - the formatting condition
### getCellArea(int index) {#getCellArea-int-}
```
public CellArea getCellArea(int index)
```


通过索引获取条件格式化的单元格范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 条件格式化的单元格范围的索引。 |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the conditional formatted cell range
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


获取条件的数量。

**Returns:**
int
### getRangeCount() {#getRangeCount--}
```
public int getRangeCount()
```


获取条件格式化范围的数量。

**Returns:**
int
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




### removeArea(int index) {#removeArea-int-}
```
public void removeArea(int index)
```


通过索引移除条件格式化的单元格范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 要删除的条件格式化单元格范围的索引。 |

### removeArea(int startRow, int startColumn, int totalRows, int totalColumns) {#removeArea-int-int-int-int-}
```
public boolean removeArea(int startRow, int startColumn, int totalRows, int totalColumns)
```


移除范围内的条件格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 范围的起始行。 |
| startColumn | int | 范围的起始列。 |
| totalRows | int | 范围的行数。 |
| totalColumns | int | 范围的列数。 |

**Returns:**
boolean - 返回 TRUE，此 FormatCondtionCollection 应被移除。
### removeCondition(int index) {#removeCondition-int-}
```
public void removeCondition(int index)
```


按索引删除格式条件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 要删除的格式条件的索引。 |

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

