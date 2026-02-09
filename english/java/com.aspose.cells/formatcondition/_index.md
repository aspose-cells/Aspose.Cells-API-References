---
title: FormatCondition
second_title: Aspose.Cells for Java API Reference
description: Represents conditional formatting condition.
type: docs
url: /java/com.aspose.cells/formatcondition/
---

**Inheritance:**
java.lang.Object
```
public class FormatCondition
```

Represents conditional formatting condition.

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
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAboveAverage()](#getAboveAverage--) | Get the conditional formatting's "AboveAverage" instance. |
| [getClass()](#getClass--) |  |
| [getColorScale()](#getColorScale--) | Get the conditional formatting's "ColorScale" instance. |
| [getDataBar()](#getDataBar--) | Get the conditional formatting's "DataBar" instance. |
| [getFormula1()](#getFormula1--) | Gets the value or expression associated with conditional formatting. |
| [getFormula1(boolean isR1C1, boolean isLocal)](#getFormula1-boolean-boolean-) | Gets the value or expression associated with this format condition. |
| [getFormula1(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula1-boolean-boolean-int-int-) | Gets the value or expression of the conditional formatting of the cell. |
| [getFormula1(int row, int column)](#getFormula1-int-int-) | Gets the formula of the conditional formatting of the cell. |
| [getFormula2()](#getFormula2--) | Gets the value or expression associated with conditional formatting. |
| [getFormula2(boolean isR1C1, boolean isLocal)](#getFormula2-boolean-boolean-) | Gets the value or expression associated with this format condition. |
| [getFormula2(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula2-boolean-boolean-int-int-) | Gets the value or expression of the conditional formatting of the cell. |
| [getFormula2(int row, int column)](#getFormula2-int-int-) | Gets the formula of the conditional formatting of the cell. |
| [getIconSet()](#getIconSet--) | Get the conditional formatting's "IconSet" instance. |
| [getOperator()](#getOperator--) | Gets the conditional format operator type. |
| [getPriority()](#getPriority--) | The priority of this conditional formatting rule. |
| [getStopIfTrue()](#getStopIfTrue--) | True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. |
| [getStyle()](#getStyle--) | Gets or setts style of conditional formatted cell ranges. |
| [getText()](#getText--) | The text value in a "text contains" conditional formatting rule. |
| [getTimePeriod()](#getTimePeriod--) | The applicable time period in a "date occurrin" conditional formatting rule. |
| [getTop10()](#getTop10--) | Get the conditional formatting's "Top10" instance. |
| [getType()](#getType--) | Gets whether the conditional format Type. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Sets the value or expression associated with conditional formatting. |
| [setFormula1(String formula, boolean isR1C1, boolean isLocal)](#setFormula1-java.lang.String-boolean-boolean-) | Sets the value or expression associated with this format condition. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Sets the value or expression associated with conditional formatting. |
| [setFormula2(String formula, boolean isR1C1, boolean isLocal)](#setFormula2-java.lang.String-boolean-boolean-) | Sets the value or expression associated with this format condition. |
| [setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal)](#setFormulas-java.lang.String-java.lang.String-boolean-boolean-) | Sets the value or expression associated with this format condition. |
| [setOperator(int value)](#setOperator-int-) | Sets the conditional format operator type. |
| [setPriority(int value)](#setPriority-int-) | The priority of this conditional formatting rule. |
| [setStopIfTrue(boolean value)](#setStopIfTrue-boolean-) | True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Gets or setts style of conditional formatted cell ranges. |
| [setText(String value)](#setText-java.lang.String-) | The text value in a "text contains" conditional formatting rule. |
| [setTimePeriod(int value)](#setTimePeriod-int-) | The applicable time period in a "date occurrin" conditional formatting rule. |
| [setType(int value)](#setType-int-) | Sets whether the conditional format Type. |
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
### getAboveAverage() {#getAboveAverage--}
```
public AboveAverage getAboveAverage()
```


Get the conditional formatting's "AboveAverage" instance. The default instance's rule highlights cells that are above the average for all values in the range. Valid only for type = AboveAverage.

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


Get the conditional formatting's "ColorScale" instance. The default instance is a "green-yellow-red" 3ColorScale . Valid only for type = ColorScale.

**Returns:**
[ColorScale](../../com.aspose.cells/colorscale) - 
### getDataBar() {#getDataBar--}
```
public DataBar getDataBar()
```


Get the conditional formatting's "DataBar" instance. The default instance's color is blue. Valid only for type is DataBar.

**Returns:**
[DataBar](../../com.aspose.cells/databar) - 
### getFormula1() {#getFormula1--}
```
public String getFormula1()
```


Gets the value or expression associated with conditional formatting.

**Remarks**

Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\\"=...\\"".

**Returns:**
java.lang.String
### getFormula1(boolean isR1C1, boolean isLocal) {#getFormula1-boolean-boolean-}
```
public String getFormula1(boolean isR1C1, boolean isLocal)
```


Gets the value or expression associated with this format condition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns:**
java.lang.String - The value or expression associated with this format condition.
### getFormula1(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula1-boolean-boolean-int-int-}
```
public String getFormula1(boolean isR1C1, boolean isLocal, int row, int column)
```


Gets the value or expression of the conditional formatting of the cell.

**Remarks**

The given cell must be contained by this conditional formatting, otherwise null will be returned.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
| row | int | The row index. |
| column | int | The column index. |

**Returns:**
java.lang.String - The value or expression associated with the conditional formatting of the cell.
### getFormula1(int row, int column) {#getFormula1-int-int-}
```
public String getFormula1(int row, int column)
```


Gets the formula of the conditional formatting of the cell.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |
| column | int | The column index. |

**Returns:**
java.lang.String - The formula.
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Gets the value or expression associated with conditional formatting.

**Remarks**

Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\\"=...\\"".

**Returns:**
java.lang.String
### getFormula2(boolean isR1C1, boolean isLocal) {#getFormula2-boolean-boolean-}
```
public String getFormula2(boolean isR1C1, boolean isLocal)
```


Gets the value or expression associated with this format condition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns:**
java.lang.String - The value or expression associated with this format condition.
### getFormula2(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula2-boolean-boolean-int-int-}
```
public String getFormula2(boolean isR1C1, boolean isLocal, int row, int column)
```


Gets the value or expression of the conditional formatting of the cell.

**Remarks**

The given cell must be contained by this conditional formatting, otherwise null will be returned.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
| row | int | The row index. |
| column | int | The column index. |

**Returns:**
java.lang.String - The value or expression associated with the conditional formatting of the cell.
### getFormula2(int row, int column) {#getFormula2-int-int-}
```
public String getFormula2(int row, int column)
```


Gets the formula of the conditional formatting of the cell.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |
| column | int | The column index. |

**Returns:**
java.lang.String - The formula.
### getIconSet() {#getIconSet--}
```
public IconSet getIconSet()
```


Get the conditional formatting's "IconSet" instance. The default instance's IconSetType is TrafficLights31. Valid only for type = IconSet.

**Returns:**
[IconSet](../../com.aspose.cells/iconset) - 
### getOperator() {#getOperator--}
```
public int getOperator()
```


Gets the conditional format operator type.

See [OperatorType](../../com.aspose.cells/operatortype).

**Returns:**
int
### getPriority() {#getPriority--}
```
public int getPriority()
```


The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values, where '1' is the highest priority.

**Returns:**
int
### getStopIfTrue() {#getStopIfTrue--}
```
public boolean getStopIfTrue()
```


True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. Only applies for Excel 2007;

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Gets or setts style of conditional formatted cell ranges.

**Returns:**
[Style](../../com.aspose.cells/style)
### getText() {#getText--}
```
public String getText()
```


The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, beginsWith and endsWith. The default value is null.

**Returns:**
java.lang.String
### getTimePeriod() {#getTimePeriod--}
```
public int getTimePeriod()
```


The applicable time period in a "date occurrin" conditional formatting rule. Valid only for type is timePeriod. The default value is TimePeriodType.Today.

See [TimePeriodType](../../com.aspose.cells/timeperiodtype).

**Returns:**
int
### getTop10() {#getTop10--}
```
public Top10 getTop10()
```


Get the conditional formatting's "Top10" instance. The default instance's rule highlights cells whose values fall in the top 10 bracket. Valid only for type is Top10.

**Returns:**
[Top10](../../com.aspose.cells/top10) - 
### getType() {#getType--}
```
public int getType()
```


Gets whether the conditional format Type.

See [FormatConditionType](../../com.aspose.cells/formatconditiontype).

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


Sets the value or expression associated with conditional formatting.

**Remarks**

Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\\"=...\\"".

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setFormula1(String formula, boolean isR1C1, boolean isLocal) {#setFormula1-java.lang.String-boolean-boolean-}
```
public void setFormula1(String formula, boolean isR1C1, boolean isLocal)
```


Sets the value or expression associated with this format condition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | The value or expression associated with this format condition. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\\"=...\\"". |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Sets the value or expression associated with conditional formatting.

**Remarks**

Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\\"=...\\"".

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setFormula2(String formula, boolean isR1C1, boolean isLocal) {#setFormula2-java.lang.String-boolean-boolean-}
```
public void setFormula2(String formula, boolean isR1C1, boolean isLocal)
```


Sets the value or expression associated with this format condition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | The value or expression associated with this format condition. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\\"=...\\"". |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |

### setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal) {#setFormulas-java.lang.String-java.lang.String-boolean-boolean-}
```
public void setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal)
```


Sets the value or expression associated with this format condition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula1 | java.lang.String | The value or expression associated with this format condition. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\\"=...\\"". |
| formula2 | java.lang.String | The value or expression associated with this format condition. The input format is same with formula1 |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |

### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```


Sets the conditional format operator type.

See [OperatorType](../../com.aspose.cells/operatortype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPriority(int value) {#setPriority-int-}
```
public void setPriority(int value)
```


The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values, where '1' is the highest priority.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setStopIfTrue(boolean value) {#setStopIfTrue-boolean-}
```
public void setStopIfTrue(boolean value)
```


True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. Only applies for Excel 2007;

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Gets or setts style of conditional formatted cell ranges.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, beginsWith and endsWith. The default value is null.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setTimePeriod(int value) {#setTimePeriod-int-}
```
public void setTimePeriod(int value)
```


The applicable time period in a "date occurrin" conditional formatting rule. Valid only for type is timePeriod. The default value is TimePeriodType.Today.

See [TimePeriodType](../../com.aspose.cells/timeperiodtype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Sets whether the conditional format Type.

See [FormatConditionType](../../com.aspose.cells/formatconditiontype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

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

