---
title: "趋势线"
second_title: "Aspose.Cells for Java API 参考"
description: "表示图表中的趋势线。"
type: docs
url: /zh/java/com.aspose.cells/trendline/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Line](../../com.aspose.cells/line)
```
public class Trendline extends Line
```

表示图表中的趋势线。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Excel object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
         //Adding a sample value to "A4" cell
         worksheet.getCells().get("A4").putValue(200);
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a sample value to "B4" cell
         worksheet.getCells().get("B4").putValue(40);
         //Adding a sample value to "C1" cell as category data
         worksheet.getCells().get("C1").putValue("Q1");
         //Adding a sample value to "C2" cell as category data
         worksheet.getCells().get("C2").putValue("Q2");
         //Adding a sample value to "C3" cell as category data
         worksheet.getCells().get("C3").putValue("Y1");
         //Adding a sample value to "C4" cell as category data
         worksheet.getCells().get("C4").putValue("Y2");
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
         chart.getNSeries().add("A1:B4", true);
         //Setting the data source for the category data of NSeries
         chart.getNSeries().setCategoryData("C1:C4");
         //adding a linear trendline
         int index = chart.getNSeries().get(0).getTrendLines().add(TrendlineType.LINEAR);
         Trendline trendline = chart.getNSeries().get(0).getTrendLines().get(index);
         //Setting the custom name of the trendline.
         trendline.setName("Linear");
         //Displaying the equation on chart
         trendline.setDisplayEquation(true);
         //Displaying the R-Squared value on chart
         trendline.setDisplayRSquared(true);
         //Saving the Excel file
         workbook.save("book1.xls");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackward()](#getBackward--) | 返回或设置趋势线向后延伸的周期数（或散点图上的单位数）。 |
| [getBeginArrowLength()](#getBeginArrowLength--) | 指定线段起点的箭头长度。 |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | 指定线段起点的箭头宽度。 |
| [getBeginType()](#getBeginType--) | 指定线段起点的箭头。 |
| [getCapType()](#getCapType--) | 指定结束端帽。 |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | 表示线段的 [Color](../../com.aspose.cells/color)。 |
| [getCompoundType()](#getCompoundType--) | 指定复合线类型 |
| [getDashType()](#getDashType--) | 指定虚线类型 |
| [getDataLabels()](#getDataLabels--) | 表示指定系列的 DataLabels 对象。 |
| [getDisplayEquation()](#getDisplayEquation--) | 表示是否在图表上显示趋势线的方程（与 R 平方值在同一数据标签中）。 |
| [getDisplayRSquared()](#getDisplayRSquared--) | 表示是否在图表上显示趋势线的 R 平方值（与方程在同一数据标签中）。 |
| [getEndArrowLength()](#getEndArrowLength--) | 指定线段终点的箭头长度。 |
| [getEndArrowWidth()](#getEndArrowWidth--) | 指定线段终点的箭头宽度。 |
| [getEndType()](#getEndType--) | 指定线段末端的箭头。 |
| [getFormattingType()](#getFormattingType--) | 获取格式类型。 |
| [getForward()](#getForward--) | 返回或设置趋势线向前延伸的周期数（或散点图上的单位数）。 |
| [getGradientFill()](#getGradientFill--) | 表示渐变填充。 |
| [getIntercept()](#getIntercept--) | 返回或设置趋势线与数值轴交叉的点。 |
| [getJoinType()](#getJoinType--) | 指定连接端帽。 |
| [getLegendEntry()](#getLegendEntry--) | 获取根据此趋势线的图例项 |
| [getName()](#getName--) | 返回趋势线的名称。 |
| [getOrder()](#getOrder--) | 当趋势线类型为多项式时，返回或设置趋势线的阶数（大于 1 的整数）。 |
| [getPeriod()](#getPeriod--) | 返回或设置移动平均趋势线的周期。 |
| [getStyle()](#getStyle--) | 表示线条的样式。 |
| [getThemeColor()](#getThemeColor--) | 获取主题颜色。 |
| [getTransparency()](#getTransparency--) | 返回或设置线条的透明度，取值范围为 0.0（不透明）到 1.0（透明）。 |
| [getType()](#getType--) | 返回趋势线类型。 |
| [getWeight()](#getWeight--) | 获取线条的 [WeightType](../../com.aspose.cells/weighttype)。 |
| [getWeightPt()](#getWeightPt--) | 获取线条的粗细，单位为磅。 |
| [getWeightPx()](#getWeightPx--) | 获取线条的粗细，单位为像素。 |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | 指示此线条样式是否自动分配。 |
| [isAutomaticColor()](#isAutomaticColor--) | 指示线条颜色是否自动分配。 |
| [isInterceptAuto()](#isInterceptAuto--) | 指示 Microsoft Workbook 是否自动确定趋势线的截距。 |
| [isNameAuto()](#isNameAuto--) | 返回 Microsoft Excel 是否自动确定趋势线的名称。 |
| [isVisible()](#isVisible--) | 表示线条是否可见。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuto(boolean value)](#setAuto-boolean-) | 指示此线条样式是否自动分配。 |
| [setBackward(double value)](#setBackward-double-) | 返回或设置趋势线向后延伸的周期数（或散点图上的单位数）。 |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | 指定线段起点的箭头长度。 |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | 指定线段起点的箭头宽度。 |
| [setBeginType(int value)](#setBeginType-int-) | 指定线段起点的箭头。 |
| [setCapType(int value)](#setCapType-int-) | 指定结束端帽。 |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | 表示线段的 [Color](../../com.aspose.cells/color)。 |
| [setCompoundType(int value)](#setCompoundType-int-) | 指定复合线类型 |
| [setDashType(int value)](#setDashType-int-) | 指定虚线类型 |
| [setDisplayEquation(boolean value)](#setDisplayEquation-boolean-) | 表示是否在图表上显示趋势线的方程（与 R 平方值在同一数据标签中）。 |
| [setDisplayRSquared(boolean value)](#setDisplayRSquared-boolean-) | 表示是否在图表上显示趋势线的 R 平方值（与方程在同一数据标签中）。 |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | 指定线段终点的箭头长度。 |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | 指定线段终点的箭头宽度。 |
| [setEndType(int value)](#setEndType-int-) | 指定线段末端的箭头。 |
| [setFormattingType(int value)](#setFormattingType-int-) | 设置格式类型。 |
| [setForward(double value)](#setForward-double-) | 返回或设置趋势线向前延伸的周期数（或散点图上的单位数）。 |
| [setIntercept(double value)](#setIntercept-double-) | 返回或设置趋势线与数值轴交叉的点。 |
| [setInterceptAuto(boolean isInterceptAuto)](#setInterceptAuto-boolean-) | 设置 Microsoft Workbook 是否自动确定趋势线的截距。 |
| [setJoinType(int value)](#setJoinType-int-) | 指定连接端帽。 |
| [setName(String value)](#setName-java.lang.String-) | 返回趋势线的名称。 |
| [setNameAuto(boolean value)](#setNameAuto-boolean-) | 返回 Microsoft Excel 是否自动确定趋势线的名称。 |
| [setOrder(int value)](#setOrder-int-) | 当趋势线类型为多项式时，返回或设置趋势线的阶数（大于 1 的整数）。 |
| [setPeriod(int value)](#setPeriod-int-) | 返回或设置移动平均趋势线的周期。 |
| [setStyle(int value)](#setStyle-int-) | 表示线条的样式。 |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | 设置主题颜色。 |
| [setTransparency(double value)](#setTransparency-double-) | 返回或设置线条的透明度，取值范围为 0.0（不透明）到 1.0（透明）。 |
| [setVisible(boolean value)](#setVisible-boolean-) | 表示线条是否可见。 |
| [setWeight(int value)](#setWeight-int-) | 设置线条的 [WeightType](../../com.aspose.cells/weighttype)。 |
| [setWeightPt(double value)](#setWeightPt-double-) | 设置线条的粗细，单位为点。 |
| [setWeightPx(double value)](#setWeightPx-double-) | 设置线条的粗细，单位为像素。 |
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
### getBackward() {#getBackward--}
```
public double getBackward()
```


返回或设置趋势线向后延伸的周期数（或散点图上的单位）。周期数必须大于或等于零。如果图表类型为柱形图，周期数必须在 0 到 0.5 之间。

**Returns:**
double
### getBeginArrowLength() {#getBeginArrowLength--}
```
public int getBeginArrowLength()
```


指定线段起点的箭头长度。

参见 [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength)。

**Returns:**
int
### getBeginArrowWidth() {#getBeginArrowWidth--}
```
public int getBeginArrowWidth()
```


指定线段起点的箭头宽度。

参见 [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth)。

**Returns:**
int
### getBeginType() {#getBeginType--}
```
public int getBeginType()
```


指定线段起点的箭头。

参见 [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle)。

**Returns:**
int
### getCapType() {#getCapType--}
```
public int getCapType()
```


指定结束端帽。

参见 [LineCapType](../../com.aspose.cells/linecaptype)。

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


表示线段的 [Color](../../com.aspose.cells/color)。

**Returns:**
[Color](../../com.aspose.cells/color)
### getCompoundType() {#getCompoundType--}
```
public int getCompoundType()
```


指定复合线类型

参见 [MsoLineStyle](../../com.aspose.cells/msolinestyle)。

**Returns:**
int
### getDashType() {#getDashType--}
```
public int getDashType()
```


指定虚线类型

参见 [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle)。

**Returns:**
int
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


表示指定系列的 DataLabels 对象。

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDisplayEquation() {#getDisplayEquation--}
```
public boolean getDisplayEquation()
```


表示是否在图表上显示趋势线的方程（与 R 平方值在同一数据标签中）。将此属性设置为 True 会自动打开数据标签。

**Returns:**
boolean
### getDisplayRSquared() {#getDisplayRSquared--}
```
public boolean getDisplayRSquared()
```


表示是否在图表上显示趋势线的 R 平方值（与方程在同一数据标签中）。将此属性设置为 True 会自动打开数据标签。

**Returns:**
boolean
### getEndArrowLength() {#getEndArrowLength--}
```
public int getEndArrowLength()
```


指定线段终点的箭头长度。

参见 [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength)。

**Returns:**
int
### getEndArrowWidth() {#getEndArrowWidth--}
```
public int getEndArrowWidth()
```


指定线段终点的箭头宽度。

参见 [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth)。

**Returns:**
int
### getEndType() {#getEndType--}
```
public int getEndType()
```


指定线段末端的箭头。

参见 [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle)。

**Returns:**
int
### getFormattingType() {#getFormattingType--}
```
public int getFormattingType()
```


获取格式类型。

参见 [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype)。

**Returns:**
int
### getForward() {#getForward--}
```
public double getForward()
```


返回或设置趋势线向前延伸的周期数（或散点图上的单位）。周期数必须大于或等于零。

**Returns:**
double
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


表示渐变填充。

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getIntercept() {#getIntercept--}
```
public double getIntercept()
```


返回或设置趋势线与数值轴交叉的点。

**Returns:**
double
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


指定连接端帽。

参见 [LineJoinType](../../com.aspose.cells/linejointype)。

**Returns:**
int
### getLegendEntry() {#getLegendEntry--}
```
public LegendEntry getLegendEntry()
```


获取根据此趋势线的图例项

**Returns:**
[LegendEntry](../../com.aspose.cells/legendentry)
### getName() {#getName--}
```
public String getName()
```


返回趋势线的名称。

**Returns:**
java.lang.String
### getOrder() {#getOrder--}
```
public int getOrder()
```


返回或设置趋势线类型为多项式时的趋势线阶数（大于 1 的整数）。阶数必须在 2 到 6 之间。

**Returns:**
int
### getPeriod() {#getPeriod--}
```
public int getPeriod()
```


返回或设置移动平均趋势线的周期。

**Remarks**

该值应在 2 到 255 之间，并且必须小于系列中的图表点数。

**Returns:**
int
### getStyle() {#getStyle--}
```
public int getStyle()
```


表示线条的样式。

参见 [LineType](../../com.aspose.cells/linetype)。

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


获取主题颜色。

**Remarks**

如果前景色不是主题颜色，将返回 NULL。

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


返回或设置线条的透明度，取值范围为 0.0（不透明）到 1.0（透明）。

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


返回趋势线类型。

参见 [TrendlineType](../../com.aspose.cells/trendlinetype)。

**Returns:**
int
### getWeight() {#getWeight--}
```
public int getWeight()
```


获取线条的 [WeightType](../../com.aspose.cells/weighttype)。

参见 [WeightType](../../com.aspose.cells/weighttype)。

**Returns:**
int
### getWeightPt() {#getWeightPt--}
```
public double getWeightPt()
```


获取线条的粗细，单位为磅。

**Returns:**
double
### getWeightPx() {#getWeightPx--}
```
public double getWeightPx()
```


获取线条的粗细，单位为像素。

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAuto() {#isAuto--}
```
public boolean isAuto()
```


指示此线条样式是否自动分配。

**Returns:**
boolean
### isAutomaticColor() {#isAutomaticColor--}
```
public boolean isAutomaticColor()
```


指示线条颜色是否自动分配。

**Returns:**
boolean
### isInterceptAuto() {#isInterceptAuto--}
```
public boolean isInterceptAuto()
```


指示 Microsoft Workbook 是否自动确定趋势线的截距。

**Returns:**
boolean
### isNameAuto() {#isNameAuto--}
```
public boolean isNameAuto()
```


返回 Microsoft Excel 是否自动确定趋势线的名称。

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


表示线条是否可见。

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




### setAuto(boolean value) {#setAuto-boolean-}
```
public void setAuto(boolean value)
```


指示此线条样式是否自动分配。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setBackward(double value) {#setBackward-double-}
```
public void setBackward(double value)
```


返回或设置趋势线向后延伸的周期数（或散点图上的单位）。周期数必须大于或等于零。如果图表类型为柱形图，周期数必须在 0 到 0.5 之间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setBeginArrowLength(int value) {#setBeginArrowLength-int-}
```
public void setBeginArrowLength(int value)
```


指定线段起点的箭头长度。

参见 [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBeginArrowWidth(int value) {#setBeginArrowWidth-int-}
```
public void setBeginArrowWidth(int value)
```


指定线段起点的箭头宽度。

参见 [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBeginType(int value) {#setBeginType-int-}
```
public void setBeginType(int value)
```


指定线段起点的箭头。

参见 [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setCapType(int value) {#setCapType-int-}
```
public void setCapType(int value)
```


指定结束端帽。

参见 [LineCapType](../../com.aspose.cells/linecaptype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


表示线段的 [Color](../../com.aspose.cells/color)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```


指定复合线类型

参见 [MsoLineStyle](../../com.aspose.cells/msolinestyle)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setDashType(int value) {#setDashType-int-}
```
public void setDashType(int value)
```


指定虚线类型

参见 [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setDisplayEquation(boolean value) {#setDisplayEquation-boolean-}
```
public void setDisplayEquation(boolean value)
```


表示是否在图表上显示趋势线的方程（与 R 平方值在同一数据标签中）。将此属性设置为 True 会自动打开数据标签。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDisplayRSquared(boolean value) {#setDisplayRSquared-boolean-}
```
public void setDisplayRSquared(boolean value)
```


表示是否在图表上显示趋势线的 R 平方值（与方程在同一数据标签中）。将此属性设置为 True 会自动打开数据标签。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEndArrowLength(int value) {#setEndArrowLength-int-}
```
public void setEndArrowLength(int value)
```


指定线段终点的箭头长度。

参见 [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setEndArrowWidth(int value) {#setEndArrowWidth-int-}
```
public void setEndArrowWidth(int value)
```


指定线段终点的箭头宽度。

参见 [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setEndType(int value) {#setEndType-int-}
```
public void setEndType(int value)
```


指定线段末端的箭头。

参见 [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setFormattingType(int value) {#setFormattingType-int-}
```
public void setFormattingType(int value)
```


设置格式类型。

参见 [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setForward(double value) {#setForward-double-}
```
public void setForward(double value)
```


返回或设置趋势线向前延伸的周期数（或散点图上的单位）。周期数必须大于或等于零。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setIntercept(double value) {#setIntercept-double-}
```
public void setIntercept(double value)
```


返回或设置趋势线与数值轴交叉的点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setInterceptAuto(boolean isInterceptAuto) {#setInterceptAuto-boolean-}
```
public void setInterceptAuto(boolean isInterceptAuto)
```


设置 Microsoft Workbook 是否自动确定趋势线的截距。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isInterceptAuto | boolean |  |

### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```


指定连接端帽。

参见 [LineJoinType](../../com.aspose.cells/linejointype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


返回趋势线的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setNameAuto(boolean value) {#setNameAuto-boolean-}
```
public void setNameAuto(boolean value)
```


返回 Microsoft Excel 是否自动确定趋势线的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setOrder(int value) {#setOrder-int-}
```
public void setOrder(int value)
```


返回或设置趋势线类型为多项式时的趋势线阶数（大于 1 的整数）。阶数必须在 2 到 6 之间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPeriod(int value) {#setPeriod-int-}
```
public void setPeriod(int value)
```


返回或设置移动平均趋势线的周期。

**Remarks**

该值应在 2 到 255 之间，并且必须小于系列中的图表点数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```


表示线条的样式。

参见 [LineType](../../com.aspose.cells/linetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


设置主题颜色。

**Remarks**

如果前景色不是主题颜色，将返回 NULL。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


返回或设置线条的透明度，取值范围为 0.0（不透明）到 1.0（透明）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


表示线条是否可见。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setWeight(int value) {#setWeight-int-}
```
public void setWeight(int value)
```


设置线条的 [WeightType](../../com.aspose.cells/weighttype)。

参见 [WeightType](../../com.aspose.cells/weighttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setWeightPt(double value) {#setWeightPt-double-}
```
public void setWeightPt(double value)
```


设置线条的粗细，单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setWeightPx(double value) {#setWeightPx-double-}
```
public void setWeightPx(double value)
```


设置线条的粗细，单位为像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

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

