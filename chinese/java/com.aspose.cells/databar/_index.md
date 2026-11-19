---
title: "数据条"
second_title: "Aspose.Cells for Java API 参考"
description: "描述数据条的条件格式规则。"
type: docs
url: /zh/java/com.aspose.cells/databar/
---

**Inheritance:**
java.lang.Object
```
public class DataBar
```

描述 DataBar 条件格式规则。此条件格式规则在单元格范围内显示渐变数据条。

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
 
         ca.EndRow = 2;
 
         ca.StartColumn = 0;
 
         ca.EndColumn = 0;
 
         fcs.addArea(ca);
 
         //Adds condition.
         int idx = fcs.addCondition(FormatConditionType.DATA_BAR);
 
         fcs.addArea(ca);
 
         FormatCondition cond = fcs.get(idx);
 
         //Get Databar
         DataBar dataBar = cond.getDataBar();
 
         dataBar.setColor(Color.getOrange());
 
         //Set Databar properties
         dataBar.getMinCfvo().setType(FormatConditionValueType.PERCENTILE);
 
         dataBar.getMinCfvo().setValue(30);
 
         dataBar.setShowValue(false);
 
         dataBar.getBarBorder().setType(DataBarBorderType.SOLID);
 
         dataBar.getBarBorder().setColor(Color.getPlum());
 
          dataBar.setBarFillType(DataBarFillType.SOLID);
 
          dataBar.setAxisColor(Color.getRed());
 
          dataBar.setAxisPosition(DataBarAxisPosition.MIDPOINT);
 
          dataBar.getNegativeBarFormat().setColorType(DataBarNegativeColorType.COLOR);
 
          dataBar.getNegativeBarFormat().setColor(Color.getWhite());
 
          dataBar.getNegativeBarFormat().setBorderColorType(DataBarNegativeColorType.COLOR);
 
          dataBar.getNegativeBarFormat().setBorderColor(Color.getYellow());
 
         //Put Cell Values
         Cell cell1 = sheet.getCells().get("A1");
 
         cell1.putValue(10);
 
         Cell cell2 = sheet.getCells().get("A2");
 
         cell2.putValue(120);
 
         Cell cell3 = sheet.getCells().get("A3");
 
         cell3.putValue(260);
 
         //Saving the Excel file
         workbook.save("book1.xlsx");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAxisColor()](#getAxisColor--) | 获取作为数据条的条件格式单元格的轴颜色。 |
| [getAxisPosition()](#getAxisPosition--) | 获取由条件格式规则指定的数据条轴的位置。 |
| [getBarBorder()](#getBarBorder--) | 获取指定数据条边框的对象。 |
| [getBarFillType()](#getBarFillType--) | 获取数据条的填充颜色方式。 |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | 获取此 DataBar 的颜色。 |
| [getDirection()](#getDirection--) | 获取数据条显示的方向。 |
| [getMaxCfvo()](#getMaxCfvo--) | 获取此 DataBar 的最大值对象。 |
| [getMaxLength()](#getMaxLength--) | 表示数据条的最大长度。 |
| [getMinCfvo()](#getMinCfvo--) | 获取此 DataBar 的最小值对象。 |
| [getMinLength()](#getMinLength--) | 表示数据条的最小长度。 |
| [getNegativeBarFormat()](#getNegativeBarFormat--) | 获取与数据条条件格式规则关联的 NegativeBarFormat 对象。 |
| [getShowValue()](#getShowValue--) | 获取指示是否显示此数据条所应用单元格值的标志。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAxisColor(Color value)](#setAxisColor-com.aspose.cells.Color-) | 获取作为数据条的条件格式单元格的轴颜色。 |
| [setAxisPosition(int value)](#setAxisPosition-int-) | 设置由条件格式规则指定的数据条轴的位置。 |
| [setBarFillType(int value)](#setBarFillType-int-) | 设置数据条的填充颜色方式。 |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | 设置此 DataBar 的颜色。 |
| [setDirection(int value)](#setDirection-int-) | 设置数据条显示的方向。 |
| [setMaxLength(int value)](#setMaxLength-int-) | 表示数据条的最大长度。 |
| [setMinLength(int value)](#setMinLength-int-) | 表示数据条的最小长度。 |
| [setShowValue(boolean value)](#setShowValue-boolean-) | 设置指示是否显示此数据条所应用单元格值的标志。 |
| [toImage(Cell cell, ImageOrPrintOptions imgOpts)](#toImage-com.aspose.cells.Cell-com.aspose.cells.ImageOrPrintOptions-) | 将单元格中的数据条渲染为图像字节数组。 |
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
### getAxisColor() {#getAxisColor--}
```
public Color getAxisColor()
```


获取作为数据条的条件格式单元格的轴颜色。

**Returns:**
[Color](../../com.aspose.cells/color)
### getAxisPosition() {#getAxisPosition--}
```
public int getAxisPosition()
```


获取由条件格式规则指定的数据条轴的位置。

参见 [DataBarAxisPosition](../../com.aspose.cells/databaraxisposition)。

**Returns:**
int
### getBarBorder() {#getBarBorder--}
```
public DataBarBorder getBarBorder()
```


获取指定数据条边框的对象。

**Returns:**
[DataBarBorder](../../com.aspose.cells/databarborder)
### getBarFillType() {#getBarFillType--}
```
public int getBarFillType()
```


获取数据条的填充颜色方式。

参见 [DataBarFillType](../../com.aspose.cells/databarfilltype)。

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```


获取此 DataBar 的颜色。

**Returns:**
[Color](../../com.aspose.cells/color)
### getDirection() {#getDirection--}
```
public int getDirection()
```


获取数据条显示的方向。

参见 [TextDirectionType](../../com.aspose.cells/textdirectiontype)。

**Returns:**
int
### getMaxCfvo() {#getMaxCfvo--}
```
public ConditionalFormattingValue getMaxCfvo()
```


获取此 DataBar 的最大值对象。不能将 null 或类型为 FormatConditionValueType.Min 的 CFValueObject 设置给它。

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


表示数据条的最大长度。

**Returns:**
int
### getMinCfvo() {#getMinCfvo--}
```
public ConditionalFormattingValue getMinCfvo()
```


获取此 DataBar 的最小值对象。不能将 null 或类型为 FormatConditionValueType.Max 的 CFValueObject 设置给它。

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMinLength() {#getMinLength--}
```
public int getMinLength()
```


表示数据条的最小长度。

**Returns:**
int
### getNegativeBarFormat() {#getNegativeBarFormat--}
```
public NegativeBarFormat getNegativeBarFormat()
```


获取与数据条条件格式规则关联的 NegativeBarFormat 对象。

**Returns:**
[NegativeBarFormat](../../com.aspose.cells/negativebarformat)
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


获取指示是否显示此数据条所应用单元格值的标志。默认值为 true。

**Returns:**
boolean
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




### setAxisColor(Color value) {#setAxisColor-com.aspose.cells.Color-}
```
public void setAxisColor(Color value)
```


获取作为数据条的条件格式单元格的轴颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setAxisPosition(int value) {#setAxisPosition-int-}
```
public void setAxisPosition(int value)
```


设置由条件格式规则指定的数据条轴的位置。

参见 [DataBarAxisPosition](../../com.aspose.cells/databaraxisposition)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBarFillType(int value) {#setBarFillType-int-}
```
public void setBarFillType(int value)
```


设置数据条的填充颜色方式。

参见 [DataBarFillType](../../com.aspose.cells/databarfilltype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


设置此 DataBar 的颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDirection(int value) {#setDirection-int-}
```
public void setDirection(int value)
```


设置数据条显示的方向。

参见 [TextDirectionType](../../com.aspose.cells/textdirectiontype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```


表示数据条的最大长度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMinLength(int value) {#setMinLength-int-}
```
public void setMinLength(int value)
```


表示数据条的最小长度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


设置标志，指示是否显示应用此数据条的单元格的值。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### toImage(Cell cell, ImageOrPrintOptions imgOpts) {#toImage-com.aspose.cells.Cell-com.aspose.cells.ImageOrPrintOptions-}
```
public byte[] toImage(Cell cell, ImageOrPrintOptions imgOpts)
```


将单元格中的数据条渲染为图像字节数组。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | 指示数据条应渲染的单元格 |
| imgOpts | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions 包含一些输出图像的属性 |

**Returns:**
byte[] -
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

