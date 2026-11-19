---
title: "CalculationData"
second_title: "Aspose.Cells for Java API 参考"
description: "表示在计算单个函数（例如函数名称、参数等）时所需的数据。"
type: docs
url: /zh/java/com.aspose.cells/calculationdata/
---

**Inheritance:**
java.lang.Object
```
public class CalculationData
```

表示计算单个函数时所需的数据，例如函数名称、参数等。

**Remarks**

此类提供的所有对象仅用于“读取”目的。用户不应在公式计算过程中更改工作簿中的任何数据，否则可能导致意外结果或异常。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | 获取此函数的计算值。 |
| [getCell()](#getCell--) | 获取函数所在的 Cell 对象。 |
| [getCellColumn()](#getCellColumn--) | 获取函数所在单元格的列索引。 |
| [getCellRow()](#getCellRow--) | 获取函数所在单元格的行索引。 |
| [getClass()](#getClass--) |  |
| [getFunctionName()](#getFunctionName--) | 获取要计算的函数名称。 |
| [getParamCount()](#getParamCount--) | 获取参数的数量 |
| [getParamText(int index)](#getParamText-int-) | 获取给定索引处参数的文字文本。 |
| [getParamValue(int index)](#getParamValue-int-) | 获取给定索引处参数的表示值对象。 |
| [getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)](#getParamValueInArrayMode-int-int-int-) | 获取给定索引处参数的值。 |
| [getWorkbook()](#getWorkbook--) | 获取函数所在的 Workbook 对象。 |
| [getWorksheet()](#getWorksheet--) | 获取函数所在的 Worksheet 对象。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object value)](#setCalculatedValue-java.lang.Object-) | 设置此函数的计算值。 |
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
### getCalculatedValue() {#getCalculatedValue--}
```
public Object getCalculatedValue()
```


获取此函数的计算值。

**Remarks**

用户应在其自定义计算引擎中为引擎支持的那些函数设置此属性，随后在获取此属性时将返回已设置的值。已设置的值可以是 [Cell.getValue()](../../com.aspose.cells/cell\#getValue--) 的可能类型，或此类值的数组，或 Range、Name、ReferredArea。若在设置值之前获取此属性，函数将由 Aspose.Cells 的默认计算引擎进行计算，然后返回计算后的值（对于用户自定义函数通常应为 \#NAME?）。

**Returns:**
java.lang.Object
### getCell() {#getCell--}
```
public Cell getCell()
```


获取函数所在的 Cell 对象。

**Remarks**

在不将公式设置到单元格的情况下计算公式，例如通过 [Worksheet.calculateFormula(String,CalculationOptions)](../../com.aspose.cells/worksheet\#calculateFormula-String-CalculationOptions-)，公式将像已设置到单元格 A1 那样进行计算，因此 [getCellRow()](../../com.aspose.cells/calculationdata\#getCellRow--) 和 [getCellColumn()](../../com.aspose.cells/calculationdata\#getCellColumn--) 均为 0。但工作表中的单元格 A1 可能尚未实例化。因此在此类情况下，此属性将为 null。

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getCellColumn() {#getCellColumn--}
```
public int getCellColumn()
```


获取函数所在单元格的列索引。

**Returns:**
int
### getCellRow() {#getCellRow--}
```
public int getCellRow()
```


获取函数所在单元格的行索引。

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFunctionName() {#getFunctionName--}
```
public String getFunctionName()
```


获取要计算的函数名称。

**Returns:**
java.lang.String
### getParamCount() {#getParamCount--}
```
public int getParamCount()
```


获取参数的数量

**Returns:**
int
### getParamText(int index) {#getParamText-int-}
```
public String getParamText(int index)
```


获取给定索引处参数的文字文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 参数的索引（基于 0） |

**Returns:**
java.lang.String - 参数的文字文本
### getParamValue(int index) {#getParamValue-int-}
```
public Object getParamValue(int index)
```


获取给定索引处参数的表示值对象。

**Remarks**

对于单个参数：

如果是普通值，则返回该普通值本身；

如果是引用，则返回 ReferredArea 对象；

如果它引用了具有多个值的数据集，则返回对象数组；

如果是需要计算的某种表达式，则会在值模式下进行计算，通常根据当前单元格基准返回单个值。例如，如果 D2 公式的一个参数是 A:A+B:B，则会计算 A2+B2 并返回。然而，如果该参数已被指定为数组模式（通过  或 ），则会返回一个数组（object[][]），其项为 A1+B1、A2+B2、....

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 参数的索引（基于 0） |

**Returns:**
java.lang.Object - 参数的计算值。
### getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount) {#getParamValueInArrayMode-int-int-int-}
```
public Object[][] getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)
```


获取给定索引处参数的值。若参数是需要计算的某种表达式，则会在数组模式下进行计算。

**Remarks**

对于需要计算的表达式，以 A:A+B:B 为例：在值模式下，它会根据当前单元格基准计算为单个值。但在数组模式下，A1+B1、A2+B2、A3+B3、... 的所有值都会被计算并用于构建返回的数组。对于此类情况，最好指定行/列计数的上限（例如依据 [Cells.getMaxDataRow()](../../com.aspose.cells/cells\#getMaxDataRow--) 和 [Cells.getMaxDataColumn()](../../com.aspose.cells/cells\#getMaxDataColumn--)），否则返回的大数组可能因大量无用数据而增加内存开销。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 参数的索引（基于 0） |
| maxRowCount | int | 返回数组的行数上限。如果为非正数或大于实际行数，则使用实际行数。 |
| maxColumnCount | int | 返回数组的列数上限。如果为非正数或大于实际行数，则使用实际列数。 |

**Returns:**
java.lang.Object[][] - 包含指定参数所表示的所有项的数组。
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


获取函数所在的 Workbook 对象。

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


获取函数所在的 Worksheet 对象。

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
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




### setCalculatedValue(Object value) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object value)
```


设置此函数的计算值。

**Remarks**

用户应在其自定义计算引擎中为引擎支持的那些函数设置此属性，随后在获取此属性时将返回已设置的值。已设置的值可以是 [Cell.getValue()](../../com.aspose.cells/cell\#getValue--) 的可能类型，或此类值的数组，或 Range、Name、ReferredArea。若在设置值之前获取此属性，函数将由 Aspose.Cells 的默认计算引擎进行计算，然后返回计算后的值（对于用户自定义函数通常应为 \#NAME?）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object |  |

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

