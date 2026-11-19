---
title: "FormatCondition"
second_title: "Aspose.Cells for Java API 参考"
description: "表示条件格式的条件。"
type: docs
url: /zh/java/com.aspose.cells/formatcondition/
---

**Inheritance:**
java.lang.Object
```
public class FormatCondition
```

表示条件格式的条件。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
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
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAboveAverage()](#getAboveAverage--) | 获取条件格式的 "AboveAverage" 实例。 |
| [getClass()](#getClass--) |  |
| [getColorScale()](#getColorScale--) | 获取条件格式的 "ColorScale" 实例。 |
| [getDataBar()](#getDataBar--) | 获取条件格式的 "DataBar" 实例。 |
| [getFormula1()](#getFormula1--) | 获取与条件格式关联的值或表达式。 |
| [getFormula1(boolean isR1C1, boolean isLocal)](#getFormula1-boolean-boolean-) | 获取与此格式条件关联的值或表达式。 |
| [getFormula1(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula1-boolean-boolean-int-int-) | 获取单元格条件格式的值或表达式。 |
| [getFormula1(int row, int column)](#getFormula1-int-int-) | 获取单元格条件格式的公式。 |
| [getFormula2()](#getFormula2--) | 获取与条件格式关联的值或表达式。 |
| [getFormula2(boolean isR1C1, boolean isLocal)](#getFormula2-boolean-boolean-) | 获取与此格式条件关联的值或表达式。 |
| [getFormula2(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula2-boolean-boolean-int-int-) | 获取单元格条件格式的值或表达式。 |
| [getFormula2(int row, int column)](#getFormula2-int-int-) | 获取单元格条件格式的公式。 |
| [getIconSet()](#getIconSet--) | 获取条件格式的 "IconSet" 实例。 |
| [getOperator()](#getOperator--) | 获取条件格式运算符类型。 |
| [getPriority()](#getPriority--) | 此条件格式规则的优先级。 |
| [getStopIfTrue()](#getStopIfTrue--) | True，低优先级的规则不能覆盖此规则，当此规则评估为 true 时。 |
| [getStyle()](#getStyle--) | 获取或设置条件格式化单元格范围的样式。 |
| [getText()](#getText--) | 在 "text contains" 条件格式规则中的文本值。 |
| [getTimePeriod()](#getTimePeriod--) | 在 "date occurrin" 条件格式规则中适用的时间段。 |
| [getTop10()](#getTop10--) | 获取条件格式的 "Top10" 实例。 |
| [getType()](#getType--) | 获取条件格式类型的布尔值。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | 设置与条件格式关联的值或表达式。 |
| [setFormula1(String formula, boolean isR1C1, boolean isLocal)](#setFormula1-java.lang.String-boolean-boolean-) | 设置与此格式条件关联的值或表达式。 |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | 设置与条件格式关联的值或表达式。 |
| [setFormula2(String formula, boolean isR1C1, boolean isLocal)](#setFormula2-java.lang.String-boolean-boolean-) | 设置与此格式条件关联的值或表达式。 |
| [setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal)](#setFormulas-java.lang.String-java.lang.String-boolean-boolean-) | 设置与此格式条件关联的值或表达式。 |
| [setOperator(int value)](#setOperator-int-) | 设置条件格式运算符类型。 |
| [setPriority(int value)](#setPriority-int-) | 此条件格式规则的优先级。 |
| [setStopIfTrue(boolean value)](#setStopIfTrue-boolean-) | True，低优先级的规则不能覆盖此规则，当此规则评估为 true 时。 |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | 获取或设置条件格式化单元格范围的样式。 |
| [setText(String value)](#setText-java.lang.String-) | 在 "text contains" 条件格式规则中的文本值。 |
| [setTimePeriod(int value)](#setTimePeriod-int-) | 在 "date occurrin" 条件格式规则中适用的时间段。 |
| [setType(int value)](#setType-int-) | 设置条件格式类型的布尔值。 |
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
### getAboveAverage() {#getAboveAverage--}
```
public AboveAverage getAboveAverage()
```


获取条件格式的 "AboveAverage" 实例。默认实例的规则会突出显示范围内所有值的平均值以上的单元格。仅在 type = AboveAverage 时有效。

**Returns:**
[AboveAverage](../../com.aspose.cells/aboveaverage) - 
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColorScale() {#getColorScale--}
```
public ColorScale getColorScale()
```


获取条件格式的 "ColorScale" 实例。默认实例是 "green-yellow-red" 3ColorScale。仅在 type = ColorScale 时有效。

**Returns:**
[ColorScale](../../com.aspose.cells/colorscale) - 
### getDataBar() {#getDataBar--}
```
public DataBar getDataBar()
```


获取条件格式的 "DataBar" 实例。默认实例的颜色为蓝色。仅在 type 为 DataBar 时有效。

**Returns:**
[DataBar](../../com.aspose.cells/databar) - 
### getFormula1() {#getFormula1--}
```
public String getFormula1()
```


获取与条件格式关联的值或表达式。

**Remarks**

请在设置公式前添加所有区域。为此条件设置公式时，如果输入值以 '=' 开头，则视为公式；否则视为普通值（文本、数字、布尔）。对于以 '=' 开头的文本值，用户可以按以下格式输入公式："=\\\"=...\\\""。

**Returns:**
java.lang.String
### getFormula1(boolean isR1C1, boolean isLocal) {#getFormula1-boolean-boolean-}
```
public String getFormula1(boolean isR1C1, boolean isLocal)
```


获取与此格式条件关联的值或表达式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isR1C1 | boolean | 公式是否需要以 R1C1 格式化。 |
| isLocal | boolean | 公式是否需要根据区域设置进行格式化。 |

**Returns:**
java.lang.String - 与此格式条件关联的值或表达式。
### getFormula1(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula1-boolean-boolean-int-int-}
```
public String getFormula1(boolean isR1C1, boolean isLocal, int row, int column)
```


获取单元格条件格式的值或表达式。

**Remarks**

给定的单元格必须包含在此条件格式中，否则返回 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isR1C1 | boolean | 公式是否需要以 R1C1 格式化。 |
| isLocal | boolean | 公式是否需要根据区域设置进行格式化。 |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

**Returns:**
java.lang.String - 与单元格的条件格式关联的值或表达式。
### getFormula1(int row, int column) {#getFormula1-int-int-}
```
public String getFormula1(int row, int column)
```


获取单元格条件格式的公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

**Returns:**
java.lang.String - 公式。
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


获取与条件格式关联的值或表达式。

**Remarks**

请在设置公式前添加所有区域。为此条件设置公式时，如果输入值以 '=' 开头，则视为公式；否则视为普通值（文本、数字、布尔）。对于以 '=' 开头的文本值，用户可以按以下格式输入公式："=\\\"=...\\\""。

**Returns:**
java.lang.String
### getFormula2(boolean isR1C1, boolean isLocal) {#getFormula2-boolean-boolean-}
```
public String getFormula2(boolean isR1C1, boolean isLocal)
```


获取与此格式条件关联的值或表达式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isR1C1 | boolean | 公式是否需要以 R1C1 格式化。 |
| isLocal | boolean | 公式是否需要根据区域设置进行格式化。 |

**Returns:**
java.lang.String - 与此格式条件关联的值或表达式。
### getFormula2(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula2-boolean-boolean-int-int-}
```
public String getFormula2(boolean isR1C1, boolean isLocal, int row, int column)
```


获取单元格条件格式的值或表达式。

**Remarks**

给定的单元格必须包含在此条件格式中，否则返回 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isR1C1 | boolean | 公式是否需要以 R1C1 格式化。 |
| isLocal | boolean | 公式是否需要根据区域设置进行格式化。 |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

**Returns:**
java.lang.String - 与单元格的条件格式关联的值或表达式。
### getFormula2(int row, int column) {#getFormula2-int-int-}
```
public String getFormula2(int row, int column)
```


获取单元格条件格式的公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

**Returns:**
java.lang.String - 公式。
### getIconSet() {#getIconSet--}
```
public IconSet getIconSet()
```


获取条件格式的 "IconSet" 实例。默认实例的 IconSetType 为 TrafficLights31。仅在 type = IconSet 时有效。

**Returns:**
[IconSet](../../com.aspose.cells/iconset) - 
### getOperator() {#getOperator--}
```
public int getOperator()
```


获取条件格式运算符类型。

请参阅 [OperatorType](../../com.aspose.cells/operatortype)。

**Returns:**
int
### getPriority() {#getPriority--}
```
public int getPriority()
```


此条件格式规则的优先级。该值用于确定应先评估和呈现哪个格式。数值越小优先级越高，例如 '1' 为最高优先级。

**Returns:**
int
### getStopIfTrue() {#getStopIfTrue--}
```
public boolean getStopIfTrue()
```


True，低优先级的规则不能覆盖此规则，当此规则评估为 true 时。仅适用于 Excel 2007；

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public Style getStyle()
```


获取或设置条件格式化单元格范围的样式。

**Returns:**
[Style](../../com.aspose.cells/style)
### getText() {#getText--}
```
public String getText()
```


在 "text contains" 条件格式规则中的文本值。仅在 type = containsText、notContainsText、beginsWith 和 endsWith 时有效。默认值为 null。

**Returns:**
java.lang.String
### getTimePeriod() {#getTimePeriod--}
```
public int getTimePeriod()
```


在 "date occurrin" 条件格式规则中适用的时间段。仅在 type 为 timePeriod 时有效。默认值为 TimePeriodType.Today。

参见 [TimePeriodType](../../com.aspose.cells/timeperiodtype)。

**Returns:**
int
### getTop10() {#getTop10--}
```
public Top10 getTop10()
```


获取条件格式的 "Top10" 实例。默认实例的规则会突出显示值位于前 10% 区间的单元格。仅在 type 为 Top10 时有效。

**Returns:**
[Top10](../../com.aspose.cells/top10) - 
### getType() {#getType--}
```
public int getType()
```


获取条件格式类型的布尔值。

请参阅 [FormatConditionType](../../com.aspose.cells/formatconditiontype)。

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




### setFormula1(String value) {#setFormula1-java.lang.String-}
```
public void setFormula1(String value)
```


设置与条件格式关联的值或表达式。

**Remarks**

请在设置公式前添加所有区域。为此条件设置公式时，如果输入值以 '=' 开头，则视为公式；否则视为普通值（文本、数字、布尔）。对于以 '=' 开头的文本值，用户可以按以下格式输入公式："=\\\"=...\\\""。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setFormula1(String formula, boolean isR1C1, boolean isLocal) {#setFormula1-java.lang.String-boolean-boolean-}
```
public void setFormula1(String formula, boolean isR1C1, boolean isLocal)
```


设置与此格式条件关联的值或表达式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String | 此格式条件关联的值或表达式。如果输入值以 '=' 开头，则将其视为公式。否则将被视为普通值（文本、数字、布尔）。对于以 '=' 开头的文本值，用户可以使用以下格式输入公式：\"=\\\"=...\\\"\"。 |
| isR1C1 | boolean | 公式是否为 R1C1 公式。 |
| isLocal | boolean | 公式是否已本地化格式化。 |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


设置与条件格式关联的值或表达式。

**Remarks**

请在设置公式前添加所有区域。为此条件设置公式时，如果输入值以 '=' 开头，则视为公式；否则视为普通值（文本、数字、布尔）。对于以 '=' 开头的文本值，用户可以按以下格式输入公式："=\\\"=...\\\""。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setFormula2(String formula, boolean isR1C1, boolean isLocal) {#setFormula2-java.lang.String-boolean-boolean-}
```
public void setFormula2(String formula, boolean isR1C1, boolean isLocal)
```


设置与此格式条件关联的值或表达式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String | 此格式条件关联的值或表达式。如果输入值以 '=' 开头，则将其视为公式。否则将被视为普通值（文本、数字、布尔）。对于以 '=' 开头的文本值，用户可以使用以下格式输入公式：\"=\\\"=...\\\"\"。 |
| isR1C1 | boolean | 公式是否为 R1C1 公式。 |
| isLocal | boolean | 公式是否已本地化格式化。 |

### setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal) {#setFormulas-java.lang.String-java.lang.String-boolean-boolean-}
```
public void setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal)
```


设置与此格式条件关联的值或表达式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula1 | java.lang.String | 此格式条件关联的值或表达式。如果输入值以 '=' 开头，则将其视为公式。否则将被视为普通值（文本、数字、布尔）。对于以 '=' 开头的文本值，用户可以使用以下格式输入公式：\"=\\\"=...\\\"\"。 |
| formula2 | java.lang.String | 此格式条件关联的值或表达式。输入格式与 formula1 相同。 |
| isR1C1 | boolean | 公式是否为 R1C1 公式。 |
| isLocal | boolean | 公式是否已本地化格式化。 |

### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```


设置条件格式运算符类型。

请参阅 [OperatorType](../../com.aspose.cells/operatortype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPriority(int value) {#setPriority-int-}
```
public void setPriority(int value)
```


此条件格式规则的优先级。该值用于确定应先评估和呈现哪个格式。数值越小优先级越高，例如 '1' 为最高优先级。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setStopIfTrue(boolean value) {#setStopIfTrue-boolean-}
```
public void setStopIfTrue(boolean value)
```


True，低优先级的规则不能覆盖此规则，当此规则评估为 true 时。仅适用于 Excel 2007；

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


获取或设置条件格式化单元格范围的样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


在 "text contains" 条件格式规则中的文本值。仅在 type = containsText、notContainsText、beginsWith 和 endsWith 时有效。默认值为 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setTimePeriod(int value) {#setTimePeriod-int-}
```
public void setTimePeriod(int value)
```


在 "date occurrin" 条件格式规则中适用的时间段。仅在 type 为 timePeriod 时有效。默认值为 TimePeriodType.Today。

参见 [TimePeriodType](../../com.aspose.cells/timeperiodtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


设置条件格式类型的布尔值。

请参阅 [FormatConditionType](../../com.aspose.cells/formatconditiontype)。

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

