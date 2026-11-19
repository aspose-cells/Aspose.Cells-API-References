---
title: "ChartDataTable"
second_title: "Aspose.Cells for Java API 参考"
description: "表示图表数据表。"
type: docs
url: /zh/java/com.aspose.cells/chartdatatable/
---

**Inheritance:**
java.lang.Object
```
public class ChartDataTable
```

表示图表数据表。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
 
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
 
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
 
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
 
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
 
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
 
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 25, 10);
 
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
 
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
 
         chart.setShowDataTable(true);
 
         //Getting Chart Table
         ChartDataTable chartTable = chart.getChartDataTable();
 
         //Setting Chart Table Font Color
         chartTable.getFont().setColor(com.aspose.cells.Color.getRed());
 
         //Setting Legend Key VisibilityOptions
         chartTable.setShowLegendKey(false);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoScaleFont()](#getAutoScaleFont--) | 如果对象中的文本在对象大小变化时会更改字体大小，则为 True。 |
| [getBackgroundMode()](#getBackgroundMode--) | 获取背景的显示模式 |
| [getBorder()](#getBorder--) | 返回表示对象边框的 Border 对象 |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | 获取一个 [getFont()](../../com.aspose.cells/chartdatatable\#getFont--) 对象，该对象表示指定图表数据表的字体设置。 |
| [getShowLegendKey()](#getShowLegendKey--) | 如果数据标签图例键可见，则为 True。 |
| [hasBorderHorizontal()](#hasBorderHorizontal--) | 如果图表数据表具有水平单元格边框，则为 True |
| [hasBorderOutline()](#hasBorderOutline--) | 如果图表数据表具有轮廓边框，则为 True |
| [hasBorderVertical()](#hasBorderVertical--) | 如果图表数据表具有垂直单元格边框，则为 True |
| [hasHorizontalBorder()](#hasHorizontalBorder--) | 如果图表数据表具有水平单元格边框，则为 True |
| [hasOutlineBorder()](#hasOutlineBorder--) | 如果图表数据表具有轮廓边框，则为 True |
| [hasVerticalBorder()](#hasVerticalBorder--) | 如果图表数据表具有垂直单元格边框，则为 True |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | 如果对象中的文本在对象大小变化时会更改字体大小，则为 True。 |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | 设置背景的显示模式 |
| [setHasBorderHorizontal(boolean value)](#setHasBorderHorizontal-boolean-) | 如果图表数据表具有水平单元格边框，则为 True |
| [setHasBorderOutline(boolean value)](#setHasBorderOutline-boolean-) | 如果图表数据表具有轮廓边框，则为 True |
| [setHasBorderVertical(boolean value)](#setHasBorderVertical-boolean-) | 如果图表数据表具有垂直单元格边框，则为 True |
| [setHasHorizontalBorder(boolean value)](#setHasHorizontalBorder-boolean-) | 如果图表数据表具有水平单元格边框，则为 True |
| [setHasOutlineBorder(boolean value)](#setHasOutlineBorder-boolean-) | 如果图表数据表具有轮廓边框，则为 True |
| [setHasVerticalBorder(boolean value)](#setHasVerticalBorder-boolean-) | 如果图表数据表具有垂直单元格边框，则为 True |
| [setShowLegendKey(boolean value)](#setShowLegendKey-boolean-) | 如果数据标签图例键可见，则为 True。 |
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
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


如果对象中的文本在对象大小变化时会更改字体大小，则为 True。默认值为 True。

**Returns:**
boolean
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


获取背景的显示模式

参见 [BackgroundMode](../../com.aspose.cells/backgroundmode)。

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


返回表示对象边框的 Border 对象

**Returns:**
[Line](../../com.aspose.cells/line)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFont() {#getFont--}
```
public Font getFont()
```


获取一个 [getFont()](../../com.aspose.cells/chartdatatable\#getFont--) 对象，该对象表示指定图表数据表的字体设置。

**Returns:**
[Font](../../com.aspose.cells/font)
### getShowLegendKey() {#getShowLegendKey--}
```
public boolean getShowLegendKey()
```


如果数据标签图例键可见，则为 True。

**Returns:**
boolean
### hasBorderHorizontal() {#hasBorderHorizontal--}
```
public boolean hasBorderHorizontal()
```


如果图表数据表具有水平单元格边框，则为 True

**Remarks**

注意：此属性已过时。请改用 ChartDataTable.HasHorizontalBorder 属性。自 2024 年 6 月起，此属性将在 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### hasBorderOutline() {#hasBorderOutline--}
```
public boolean hasBorderOutline()
```


如果图表数据表具有轮廓边框，则为 True

**Remarks**

注意：此属性已过时。请改用 ChartDataTable.HasOutlineBorder 属性。自 2024 年 6 月起，此属性将在 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### hasBorderVertical() {#hasBorderVertical--}
```
public boolean hasBorderVertical()
```


如果图表数据表具有垂直单元格边框，则为 True

**Remarks**

注意：此属性已过时。请改用 ChartDataTable.HasVerticalBorder 属性。自 2024 年 6 月起，此属性将在 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### hasHorizontalBorder() {#hasHorizontalBorder--}
```
public boolean hasHorizontalBorder()
```


如果图表数据表具有水平单元格边框，则为 True

**Returns:**
boolean
### hasOutlineBorder() {#hasOutlineBorder--}
```
public boolean hasOutlineBorder()
```


如果图表数据表具有轮廓边框，则为 True

**Returns:**
boolean
### hasVerticalBorder() {#hasVerticalBorder--}
```
public boolean hasVerticalBorder()
```


如果图表数据表具有垂直单元格边框，则为 True

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




### setAutoScaleFont(boolean value) {#setAutoScaleFont-boolean-}
```
public void setAutoScaleFont(boolean value)
```


如果对象中的文本在对象大小变化时会更改字体大小，则为 True。默认值为 True。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


设置背景的显示模式

参见 [BackgroundMode](../../com.aspose.cells/backgroundmode)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHasBorderHorizontal(boolean value) {#setHasBorderHorizontal-boolean-}
```
public void setHasBorderHorizontal(boolean value)
```


如果图表数据表具有水平单元格边框，则为 True

**Remarks**

注意：此属性已过时。请改用 ChartDataTable.HasHorizontalBorder 属性。自 2024 年 6 月起，此属性将在 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHasBorderOutline(boolean value) {#setHasBorderOutline-boolean-}
```
public void setHasBorderOutline(boolean value)
```


如果图表数据表具有轮廓边框，则为 True

**Remarks**

注意：此属性已过时。请改用 ChartDataTable.HasOutlineBorder 属性。自 2024 年 6 月起，此属性将在 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHasBorderVertical(boolean value) {#setHasBorderVertical-boolean-}
```
public void setHasBorderVertical(boolean value)
```


如果图表数据表具有垂直单元格边框，则为 True

**Remarks**

注意：此属性已过时。请改用 ChartDataTable.HasVerticalBorder 属性。自 2024 年 6 月起，此属性将在 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHasHorizontalBorder(boolean value) {#setHasHorizontalBorder-boolean-}
```
public void setHasHorizontalBorder(boolean value)
```


如果图表数据表具有水平单元格边框，则为 True

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHasOutlineBorder(boolean value) {#setHasOutlineBorder-boolean-}
```
public void setHasOutlineBorder(boolean value)
```


如果图表数据表具有轮廓边框，则为 True

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHasVerticalBorder(boolean value) {#setHasVerticalBorder-boolean-}
```
public void setHasVerticalBorder(boolean value)
```


如果图表数据表具有垂直单元格边框，则为 True

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowLegendKey(boolean value) {#setShowLegendKey-boolean-}
```
public void setShowLegendKey(boolean value)
```


如果数据标签图例键可见，则为 True。

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

