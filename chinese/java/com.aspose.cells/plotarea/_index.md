---
title: "PlotArea"
second_title: "Aspose.Cells for Java API 参考"
description: "封装表示图表中绘图区的对象。"
type: docs
url: /zh/java/com.aspose.cells/plotarea/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe)
```
public class PlotArea extends ChartFrame
```

封装表示图表中绘图区的对象。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | 获取 [getArea()](../../com.aspose.cells/chartframe\#getArea--)。 |
| [getAutoScaleFont()](#getAutoScaleFont--) | 如果对象中的文本在对象大小变化时会更改字体大小，则为 True。 |
| [getBackground()](#getBackground--) | 获取背景的显示模式。 |
| [getBackgroundMode()](#getBackgroundMode--) | 获取背景的显示模式。 |
| [getBorder()](#getBorder--) | 获取 [Line](../../com.aspose.cells/line)。 |
| [getChart()](#getChart--) | 获取此对象所属的图表。 |
| [getClass()](#getClass--) |  |
| [getDefaultHeight()](#getDefaultHeight--) | 表示默认位置的高度，单位为图表区域的 1/4000。 |
| [getDefaultHeightRatioToChart()](#getDefaultHeightRatioToChart--) | 表示默认位置的高度，单位为图表区域的比例。 |
| [getDefaultWidth()](#getDefaultWidth--) | 表示默认位置的宽度，单位为图表区域的 1/4000。 |
| [getDefaultWidthRatioToChart()](#getDefaultWidthRatioToChart--) | 表示默认位置的宽度，单位为图表区域的比例。 |
| [getDefaultX()](#getDefaultX--) | 表示默认位置的 x 坐标，单位为图表区域的 1/4000。 |
| [getDefaultXRatioToChart()](#getDefaultXRatioToChart--) | 表示默认位置的 x 坐标，单位为图表区域的比例。 |
| [getDefaultY()](#getDefaultY--) | 表示默认位置的 y 坐标，单位为图表区域的 1/4000。 |
| [getDefaultYRatioToChart()](#getDefaultYRatioToChart--) | 表示默认位置的 y 坐标，单位为图表区域的比例。 |
| [getFont()](#getFont--) | 获取指定 ChartFrame 对象的 [getFont()](../../com.aspose.cells/chartframe\#getFont--) 对象。 |
| [getHeight()](#getHeight--) | 获取绘图区边界框的高度，单位为图表区域的 1/4000。 |
| [getHeightPixel()](#getHeightPixel--) | 获取框架的高度，单位为像素。 |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | 获取绘图区边界框的高度，单位为图表区域的比例。 |
| [getInnerHeight()](#getInnerHeight--) | 获取绘图区的高度，单位为图表区域的 1/4000。 |
| [getInnerHeightRatioToChart()](#getInnerHeightRatioToChart--) | 获取绘图区的高度，单位为图表区域的比例。 |
| [getInnerWidth()](#getInnerWidth--) | 获取绘图区的宽度，单位为图表区域的 1/4000。 |
| [getInnerWidthRatioToChart()](#getInnerWidthRatioToChart--) | 获取绘图区的宽度，单位为图表区域的比例。 |
| [getInnerX()](#getInnerX--) | 获取绘图区左上角的 x 坐标，单位为图表区域的 1/4000。 |
| [getInnerXRatioToChart()](#getInnerXRatioToChart--) | 获取绘图区左上角的 x 坐标，单位为图表区域的比例。 |
| [getInnerY()](#getInnerY--) | 获取绘图区左上角的 x 坐标，单位为图表区域的 1/4000。 |
| [getInnerYRatioToChart()](#getInnerYRatioToChart--) | 获取绘图区左上角的 x 坐标，单位为图表区域的比例。 |
| [getShadow()](#getShadow--) | 如果框架有阴影，则为 true。 |
| [getShapeProperties()](#getShapeProperties--) | 获取 [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--) 对象。 |
| [getTextFont()](#getTextFont--) | 获取指定 ChartFrame 对象的 [getFont()](../../com.aspose.cells/chartframe\#getFont--) 对象。 |
| [getTextOptions()](#getTextOptions--) | 获取文本的选项。 |
| [getWidth()](#getWidth--) | 获取绘图区边界框的宽度，单位为图表区域的 1/4000。 |
| [getWidthPixel()](#getWidthPixel--) | 获取框架的宽度，单位为像素。 |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | 获取绘图区边界框的宽度，单位为图表区域的比例。 |
| [getX()](#getX--) | 获取绘图区边界框左上角的 x 坐标，单位为图表区域的 1/4000。 |
| [getXPixel()](#getXPixel--) | 获取左上角的 X 坐标，单位为像素。 |
| [getXRatioToChart()](#getXRatioToChart--) | 获取绘图区边界框左上角的 x 坐标，作为图表区域的比例。 |
| [getY()](#getY--) | 获取绘图区边界框左上角的 y 坐标，单位为图表区域的 1/4000。 |
| [getYPixel()](#getYPixel--) | 获取左上角的 Y 坐标，单位为像素。 |
| [getYRatioToChart()](#getYRatioToChart--) | 获取绘图区边界框左上角的 y 坐标，作为图表区域的比例。 |
| [hashCode()](#hashCode--) |  |
| [isAutomaticSize()](#isAutomaticSize--) | 指示绘图区是否自动调整大小。 |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | 指示是否已设置默认位置（DefaultX、DefaultY、DefaultWidth 和 DefaultHeight）。 |
| [isInnerMode()](#isInnerMode--) | 指示绘图区的大小是否包括刻度线和轴标签。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | 如果对象中的文本在对象大小变化时会更改字体大小，则为 True。 |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | 指示绘图区是否自动调整大小。 |
| [setBackground(int value)](#setBackground-int-) | 设置背景的显示模式。 |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | 设置背景的显示模式。 |
| [setHeight(int value)](#setHeight-int-) | 设置绘图区边界框的高度，单位为图表区域的 1/4000。 |
| [setHeightPixel(int value)](#setHeightPixel-int-) | 以像素为单位设置框架的高度。 |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | 设置绘图区域边界框的高度，单位为图表区域的比例。 |
| [setInnerHeight(int value)](#setInnerHeight-int-) | 设置绘图区域的高度，单位为图表区域的 1/4000。 |
| [setInnerHeightRatioToChart(double value)](#setInnerHeightRatioToChart-double-) | 设置绘图区域的高度，单位为图表区域的比例。 |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | 指示绘图区的大小是否包括刻度线和轴标签。 |
| [setInnerWidth(int value)](#setInnerWidth-int-) | 设置绘图区域的宽度，单位为图表区域的 1/4000。 |
| [setInnerWidthRatioToChart(double value)](#setInnerWidthRatioToChart-double-) | 设置绘图区域的宽度，单位为图表区域的比例。 |
| [setInnerX(int value)](#setInnerX-int-) | 设置绘图区域左上角的 x 坐标，单位为图表区域的 1/4000。 |
| [setInnerXRatioToChart(double value)](#setInnerXRatioToChart-double-) | 获取绘图区左上角的 x 坐标，单位为图表区域的比例。 |
| [setInnerY(int value)](#setInnerY-int-) | 设置绘图区域左上角的 x 坐标，单位为图表区域的 1/4000。 |
| [setInnerYRatioToChart(double value)](#setInnerYRatioToChart-double-) | 获取绘图区左上角的 x 坐标，单位为图表区域的比例。 |
| [setPositionAuto()](#setPositionAuto--) | 将绘图区域的位置设置为自动 |
| [setShadow(boolean value)](#setShadow-boolean-) | 如果框架有阴影，则为 true。 |
| [setWidth(int value)](#setWidth-int-) | 设置绘图区域边界框的宽度，单位为图表区域的 1/4000。 |
| [setWidthPixel(int value)](#setWidthPixel-int-) | 以像素为单位设置框架的宽度。 |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | 设置绘图区域边界框的宽度，单位为图表区域的比例。 |
| [setX(int value)](#setX-int-) | 设置绘图区域边界框左上角的 x 坐标，单位为图表区域的 1/4000。 |
| [setXPixel(int value)](#setXPixel-int-) | 以像素为单位设置左上角的 x 坐标。 |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | 设置绘图区域边界框左上角的 x 坐标，作为图表区域的比例。 |
| [setY(int value)](#setY-int-) | 设置绘图区域边界框左上角的 y 坐标，单位为图表区域的 1/4000。 |
| [setYPixel(int value)](#setYPixel-int-) | 以像素为单位设置左上角的 y 坐标。 |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | 设置绘图区域边界框左上角的 y 坐标，作为图表区域的比例。 |
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
### getArea() {#getArea--}
```
public Area getArea()
```


获取 [getArea()](../../com.aspose.cells/chartframe\#getArea--)。

**Returns:**
[Area](../../com.aspose.cells/area)
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


如果对象中的文本在对象大小变化时会更改字体大小，则为 True。默认值为 True。

**Returns:**
boolean
### getBackground() {#getBackground--}
```
public int getBackground()
```


获取背景的显示模式。此属性仅在 Excel 2003 或更早版本中有效。

参见 [BackgroundMode](../../com.aspose.cells/backgroundmode)。

**Remarks**

注意：此成员已过时。请改用 ChartFrame.Area.FillFormat.FillType 属性。例如，如果需要将 BackgroundMode 设置为 Opaque，可以使用以下代码：Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; 此属性将在自 2012 年 1 月起 12 个月后移除。Aspose 对给您带来的不便表示歉意。

**Returns:**
int
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


获取背景的显示模式。此属性仅在 Excel 2003 或更早版本中有效。

参见 [BackgroundMode](../../com.aspose.cells/backgroundmode)。

**Remarks**

注意：此成员已过时。请改用 ChartFrame.Area.FillFormat.FillType 属性。例如，如果需要将 BackgroundMode 设置为 Opaque，可以使用以下代码：Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; 此属性将在自 2026 年 2 月起 12 个月后移除。Aspose 对给您带来的不便表示歉意。

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


获取 [Line](../../com.aspose.cells/line)。

**Returns:**
[Line](../../com.aspose.cells/line)
### getChart() {#getChart--}
```
public Chart getChart()
```


获取此对象所属的图表。

**Returns:**
[Chart](../../com.aspose.cells/chart)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultHeight() {#getDefaultHeight--}
```
public int getDefaultHeight()
```


表示默认位置的高度，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 ChartFrame.DefaultHeightRatioToChart 属性。DefaultHeight = (int)(DefaultHeightRatioToChart \* 4000); 此属性将在自 2025 年 2 月起 12 个月后移除。Aspose 对给您带来的不便表示歉意。

**Returns:**
int
### getDefaultHeightRatioToChart() {#getDefaultHeightRatioToChart--}
```
public double getDefaultHeightRatioToChart()
```


表示默认位置的高度，单位为图表区域的比例。

**Returns:**
double
### getDefaultWidth() {#getDefaultWidth--}
```
public int getDefaultWidth()
```


表示默认位置的宽度，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 ChartFrame.DefaultWidthRatioToChart 属性。DefaultWidth = (int)(DefaultWidthRatioToChart \* 4000); 此属性将在自 2025 年 2 月起 12 个月后移除。Aspose 对给您带来的不便表示歉意。

**Returns:**
int
### getDefaultWidthRatioToChart() {#getDefaultWidthRatioToChart--}
```
public double getDefaultWidthRatioToChart()
```


表示默认位置的宽度，单位为图表区域的比例。

**Returns:**
double
### getDefaultX() {#getDefaultX--}
```
public int getDefaultX()
```


表示默认位置的 x 坐标，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 ChartFrame.DefaultXRatioToChart 属性。DefaultX = (int)(DefaultXRatioToChart \* 4000); 此属性将在自 2025 年 2 月起 12 个月后移除。Aspose 对给您带来的不便表示歉意。

**Returns:**
int
### getDefaultXRatioToChart() {#getDefaultXRatioToChart--}
```
public double getDefaultXRatioToChart()
```


表示默认位置的 x 坐标，单位为图表区域的比例。

**Returns:**
double
### getDefaultY() {#getDefaultY--}
```
public int getDefaultY()
```


表示默认位置的 y 坐标，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 ChartFrame.DefaultYRatioToChart 属性。DefaultY = (int)(DefaultYRatioToChart \* 4000); 此属性将在自 2025 年 2 月起 12 个月后移除。Aspose 对给您带来的不便表示歉意。

**Returns:**
int
### getDefaultYRatioToChart() {#getDefaultYRatioToChart--}
```
public double getDefaultYRatioToChart()
```


表示默认位置的 y 坐标，单位为图表区域的比例。

**Returns:**
double
### getFont() {#getFont--}
```
public Font getFont()
```


获取指定 ChartFrame 对象的 [getFont()](../../com.aspose.cells/chartframe\#getFont--) 对象。

**Returns:**
[Font](../../com.aspose.cells/font)
### getHeight() {#getHeight--}
```
public int getHeight()
```


获取绘图区边界框的高度，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 PlotArea.HeightRatioToChart 属性。Height = HeightRatioToChart \* 4000。此属性将在自 2025 年 2 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


获取框架的高度，单位为像素。

**Returns:**
int
### getHeightRatioToChart() {#getHeightRatioToChart--}
```
public double getHeightRatioToChart()
```


获取绘图区边界框的高度，单位为图表区域的比例。

**Remarks**

绘图区域边界框包括绘图区域、刻度线（刻度标签）以及刻度线周围的一小段边框。如果该值不是由 MS Excel 创建的，请在调用此方法之前调用 Chart.Calculate() 方法。

**PlotArea** 的 **XRatioToChart**、**YRatioToChart**、**WidthRatioToChart** 和 **HeightRatioToChart** 表示包括绘图区域、刻度线（刻度标签）以及刻度线周围小边框的绘图区域边界框。如果您想获取绘图区域的实际大小，应该调用 **InnerXRatioToChart**、**InnerYRatioToChart**、**InnerWidthRatioToChart** 和 **InnerHeightRatioToChart** 属性。

对于 Excel 2007 及更高版本，默认值为零。您应在调用 Chart.Calculate() 后获取该值。

HeightPixel = HeightRatioToChart \* chart.ChartObject.Width。注意：当设置 HeightRatioToChart 时，IsInnerMode 属性将自动设置为 false。

**Returns:**
double
### getInnerHeight() {#getInnerHeight--}
```
public int getInnerHeight()
```


获取绘图区的高度，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 PlotArea.InnerHeightRatioToChart 属性。InnerHeight = InnerHeightRatioToChart \* 4000; 此属性将在自 2025 年 2 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getInnerHeightRatioToChart() {#getInnerHeightRatioToChart--}
```
public double getInnerHeightRatioToChart()
```


获取绘图区的高度，单位为图表区域的比例。

**Remarks**

绘图区域边界框包括绘图区域、刻度线（刻度标签）以及刻度线周围的一小段边框。如果该值不是由 MS Excel 创建的，请在调用此方法之前调用 Chart.Calculate() 方法。

**PlotArea** 的 **XRatioToChart**、**YRatioToChart**、**WidthRatioToChart** 和 **HeightRatioToChart** 表示包括绘图区域、刻度线（刻度标签）以及刻度线周围小边框的绘图区域边界框。如果您想获取绘图区域的实际大小，应该调用 **InnerXRatioToChart**、**InnerYRatioToChart**、**InnerWidthRatioToChart** 和 **InnerHeightRatioToChart** 属性。

对于 Excel 2007 及更高版本，默认值为零。您应在调用 Chart.Calculate() 后获取该值。

InnerHeight（像素） = InnerXRatioToChart \* chart.ChartObject.Width。注意：当设置 InnerHeightRatioToChart 时，IsInnerMode 属性将自动设置为 True。

**Returns:**
double
### getInnerWidth() {#getInnerWidth--}
```
public int getInnerWidth()
```


获取绘图区的宽度，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 PlotArea.InnerWidthRatioToChart 属性。InnerWidth = InnerWidthRatioToChart \* 4000; 此属性将在自 2025 年 2 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getInnerWidthRatioToChart() {#getInnerWidthRatioToChart--}
```
public double getInnerWidthRatioToChart()
```


获取绘图区的宽度，单位为图表区域的比例。

**Remarks**

绘图区域边界框包括绘图区域、刻度线（刻度标签）以及刻度线周围的一小段边框。如果该值不是由 MS Excel 创建的，请在调用此方法之前调用 Chart.Calculate() 方法。

**PlotArea** 的 **XRatioToChart**、**YRatioToChart**、**WidthRatioToChart** 和 **HeightRatioToChart** 表示包括绘图区域、刻度线（刻度标签）以及刻度线周围小边框的绘图区域边界框。如果您想获取绘图区域的实际大小，应该调用 **InnerXRatioToChart**、**InnerYRatioToChart**、**InnerWidthRatioToChart** 和 **InnerHeightRatioToChart** 属性。

对于 Excel 2007 及更高版本，默认值为零。您应在调用 Chart.Calculate() 后获取该值。

InnerWidth（像素） = InnerXRatioToChart \* chart.ChartObject.Width。注意：当设置 InnerWidthRatioToChart 时，IsInnerMode 属性将自动设置为 True。

**Returns:**
double
### getInnerX() {#getInnerX--}
```
public int getInnerX()
```


获取绘图区左上角的 x 坐标，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 PlotArea.InnerXRatioToChart 属性。InnerX = InnerXRatioToChart \* 4000. 此属性将在自 2025 年 2 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getInnerXRatioToChart() {#getInnerXRatioToChart--}
```
public double getInnerXRatioToChart()
```


获取绘图区左上角的 x 坐标，单位为图表区域的比例。

**Remarks**

绘图区域边界框包括绘图区域、刻度线（刻度标签）以及刻度线周围的一小段边框。如果该值不是由 MS Excel 创建的，请在调用此方法之前调用 Chart.Calculate() 方法。

**PlotArea** 的 **XRatioToChart**、**YRatioToChart**、**WidthRatioToChart** 和 **HeightRatioToChart** 表示包括绘图区域、刻度线（刻度标签）以及刻度线周围小边框的绘图区域边界框。如果您想获取绘图区域的实际大小，应该调用 **InnerXRatioToChart**、**InnerYRatioToChart**、**InnerWidthRatioToChart** 和 **InnerHeightRatioToChart** 属性。

对于 Excel 2007 及更高版本，默认值为零。您应在调用 Chart.Calculate() 后获取该值。

InnerX（像素） = InnerXRatioToChart \* chart.ChartObject.Width。注意：当设置 InnerXRatioToChart 时，IsInnerMode 属性将自动设置为 True。

**Returns:**
double
### getInnerY() {#getInnerY--}
```
public int getInnerY()
```


获取绘图区左上角的 x 坐标，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 PlotArea.InnerYRatioToChart 属性。InnerY = InnerYRatioToChart \* 4000。此属性将在自 2025 年 2 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getInnerYRatioToChart() {#getInnerYRatioToChart--}
```
public double getInnerYRatioToChart()
```


获取绘图区左上角的 x 坐标，单位为图表区域的比例。

**Remarks**

绘图区域边界框包括绘图区域、刻度线（刻度标签）以及刻度线周围的一小段边框。如果该值不是由 MS Excel 创建的，请在调用此方法之前调用 Chart.Calculate() 方法。

**PlotArea** 的 **XRatioToChart**、**YRatioToChart**、**WidthRatioToChart** 和 **HeightRatioToChart** 表示包括绘图区域、刻度线（刻度标签）以及刻度线周围小边框的绘图区域边界框。如果您想获取绘图区域的实际大小，应该调用 **InnerXRatioToChart**、**InnerYRatioToChart**、**InnerWidthRatioToChart** 和 **InnerHeightRatioToChart** 属性。

对于 Excel 2007 及更高版本，默认值为零。您应在调用 Chart.Calculate() 后获取该值。

InnerY in Pixel = InnerYRatioToChart \* chart.ChartObject.Width。注意：当设置 InnerYRatioToChart 时，IsInnerMode 属性将自动设置为 True。

**Returns:**
double
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


如果框架有阴影，则为 true。

**Remarks**

仅适用于 xls 文件中的图表。

**Returns:**
boolean
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


获取 [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--) 对象。

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getTextFont() {#getTextFont--}
```
public Font getTextFont()
```


获取指定 ChartFrame 对象的 [getFont()](../../com.aspose.cells/chartframe\#getFont--) 对象。

**Remarks**

注意：此成员已过时。请改用 ChartFrame.Font 属性。此属性将在自 2012 年 1 月起 12 个月后移除。Aspose 对给您带来的不便表示歉意。

**Returns:**
[Font](../../com.aspose.cells/font)
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


获取文本的选项。

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getWidth() {#getWidth--}
```
public int getWidth()
```


获取绘图区边界框的宽度，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 PlotArea.WidthRatioToChart 属性。Width = WidthRatioToChart \* 4000。此属性将在自 2025 年 2 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


获取框架的宽度，单位为像素。

**Returns:**
int
### getWidthRatioToChart() {#getWidthRatioToChart--}
```
public double getWidthRatioToChart()
```


获取绘图区边界框的宽度，单位为图表区域的比例。

**Remarks**

绘图区域边界框包括绘图区域、刻度线（刻度标签）以及刻度线周围的一小段边框。如果该值不是由 MS Excel 创建的，请在调用此方法之前调用 Chart.Calculate() 方法。

**PlotArea** 的 **XRatioToChart**、**YRatioToChart**、**WidthRatioToChart** 和 **HeightRatioToChart** 表示包括绘图区域、刻度线（刻度标签）以及刻度线周围小边框的绘图区域边界框。如果您想获取绘图区域的实际大小，应该调用 **InnerXRatioToChart**、**InnerYRatioToChart**、**InnerWidthRatioToChart** 和 **InnerHeightRatioToChart** 属性。

对于 Excel 2007 及更高版本，默认值为零。您应在调用 Chart.Calculate() 后获取该值。

WidthPixel = WidthRatioToChart \* chart.ChartObject.Width。注意：当设置 WidthRatioToChart 时，IsInnerMode 属性将自动设置为 false。

**Returns:**
double
### getX() {#getX--}
```
public int getX()
```


获取绘图区边界框左上角的 x 坐标，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 PlotArea.XRatioToChart 属性。X = XRatioToChart \* 4000。此属性将在自 2025 年 2 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getXPixel() {#getXPixel--}
```
public int getXPixel()
```


获取左上角的 X 坐标，单位为像素。

**Returns:**
int
### getXRatioToChart() {#getXRatioToChart--}
```
public double getXRatioToChart()
```


获取绘图区边界框左上角的 x 坐标，作为图表区域的比例。

**Remarks**

绘图区域边界框包括绘图区域、刻度线（刻度标签）以及刻度线周围的一小段边框。如果该值不是由 MS Excel 创建的，请在调用此方法之前调用 Chart.Calculate() 方法。

**PlotArea** 的 **XRatioToChart**、**YRatioToChart**、**WidthRatioToChart** 和 **HeightRatioToChart** 表示包括绘图区域、刻度线（刻度标签）以及刻度线周围小边框的绘图区域边界框。如果您想获取绘图区域的实际大小，应该调用 **InnerXRatioToChart**、**InnerYRatioToChart**、**InnerWidthRatioToChart** 和 **InnerHeightRatioToChart** 属性。

对于 Excel 2007 及更高版本，默认值为零。您应在调用 Chart.Calculate() 后获取该值。

XPixel = XRatioToChart \* chart.ChartObject.Width。注意：当设置 XRatioToChart 时，IsInnerMode 属性将自动设置为 false。

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


获取绘图区边界框左上角的 y 坐标，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 PlotArea.YRatioToChart 属性。Y = YRatioToChart \* 4000。此属性将在自 2025 年 2 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getYPixel() {#getYPixel--}
```
public int getYPixel()
```


获取左上角的 Y 坐标，单位为像素。

**Returns:**
int
### getYRatioToChart() {#getYRatioToChart--}
```
public double getYRatioToChart()
```


获取绘图区边界框左上角的 y 坐标，作为图表区域的比例。

**Remarks**

绘图区域边界框包括绘图区域、刻度线（刻度标签）以及刻度线周围的一小段边框。如果该值不是由 MS Excel 创建的，请在调用此方法之前调用 Chart.Calculate() 方法。

**PlotArea** 的 **XRatioToChart**、**YRatioToChart**、**WidthRatioToChart** 和 **HeightRatioToChart** 表示包括绘图区域、刻度线（刻度标签）以及刻度线周围小边框的绘图区域边界框。如果您想获取绘图区域的实际大小，应该调用 **InnerXRatioToChart**、**InnerYRatioToChart**、**InnerWidthRatioToChart** 和 **InnerHeightRatioToChart** 属性。

对于 Excel 2007 及更高版本，默认值为零。您应在调用 Chart.Calculate() 后获取该值。

YPixel = YRatioToChart \* chart.ChartObject.Width。注意：当设置 YRatioToChart 时，IsInnerMode 属性将自动设置为 false。

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutomaticSize() {#isAutomaticSize--}
```
public boolean isAutomaticSize()
```


指示绘图区是否自动调整大小。

**Remarks**

注意：当 IsAutomaticSize 设置为 True 时，您手动设置的 Width 和 Height 值将被禁用。

**Returns:**
boolean
### isDefaultPosBeSet() {#isDefaultPosBeSet--}
```
public boolean isDefaultPosBeSet()
```


指示是否已设置默认位置（DefaultX、DefaultY、DefaultWidth 和 DefaultHeight）。

**Returns:**
boolean
### isInnerMode() {#isInnerMode--}
```
public boolean isInnerMode()
```


指示绘图区的大小是否包括刻度线和轴标签。False 表示大小应确定绘图区、刻度线和轴标签的尺寸。

**Remarks**

仅适用于 Xlsx 文件。

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




### setAutoScaleFont(boolean value) {#setAutoScaleFont-boolean-}
```
public void setAutoScaleFont(boolean value)
```


如果对象中的文本在对象大小变化时会更改字体大小，则为 True。默认值为 True。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutomaticSize(boolean value) {#setAutomaticSize-boolean-}
```
public void setAutomaticSize(boolean value)
```


指示绘图区是否自动调整大小。

**Remarks**

注意：当 IsAutomaticSize 设置为 True 时，您手动设置的 Width 和 Height 值将被禁用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setBackground(int value) {#setBackground-int-}
```
public void setBackground(int value)
```


设置背景的显示模式。此属性仅在 Excel 2003 或更早版本中有效。

参见 [BackgroundMode](../../com.aspose.cells/backgroundmode)。

**Remarks**

注意：此成员已过时。请改用 ChartFrame.Area.FillFormat.FillType 属性。例如，如果需要将 BackgroundMode 设置为 Opaque，可以使用以下代码：Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; 此属性将在自 2012 年 1 月起 12 个月后移除。Aspose 对给您带来的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


设置背景的显示模式。此属性仅在 Excel 2003 或更早版本中有效。

参见 [BackgroundMode](../../com.aspose.cells/backgroundmode)。

**Remarks**

注意：此成员已过时。请改用 ChartFrame.Area.FillFormat.FillType 属性。例如，如果需要将 BackgroundMode 设置为 Opaque，可以使用以下代码：Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; 此属性将在自 2026 年 2 月起 12 个月后移除。Aspose 对给您带来的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


设置绘图区边界框的高度，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 PlotArea.HeightRatioToChart 属性。Height = HeightRatioToChart \* 4000。此属性将在自 2025 年 2 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


以像素为单位设置框架的高度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHeightRatioToChart(double value) {#setHeightRatioToChart-double-}
```
public void setHeightRatioToChart(double value)
```


设置绘图区域边界框的高度，单位为图表区域的比例。

**Remarks**

绘图区域边界框包括绘图区域、刻度线（刻度标签）以及刻度线周围的一小段边框。如果该值不是由 MS Excel 创建的，请在调用此方法之前调用 Chart.Calculate() 方法。

**PlotArea** 的 **XRatioToChart**、**YRatioToChart**、**WidthRatioToChart** 和 **HeightRatioToChart** 表示包括绘图区域、刻度线（刻度标签）以及刻度线周围小边框的绘图区域边界框。如果您想获取绘图区域的实际大小，应该调用 **InnerXRatioToChart**、**InnerYRatioToChart**、**InnerWidthRatioToChart** 和 **InnerHeightRatioToChart** 属性。

对于 Excel 2007 及更高版本，默认值为零。您应在调用 Chart.Calculate() 后获取该值。

HeightPixel = HeightRatioToChart \* chart.ChartObject.Width。注意：当设置 HeightRatioToChart 时，IsInnerMode 属性将自动设置为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setInnerHeight(int value) {#setInnerHeight-int-}
```
public void setInnerHeight(int value)
```


设置绘图区域的高度，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 PlotArea.InnerHeightRatioToChart 属性。InnerHeight = InnerHeightRatioToChart \* 4000; 此属性将在自 2025 年 2 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setInnerHeightRatioToChart(double value) {#setInnerHeightRatioToChart-double-}
```
public void setInnerHeightRatioToChart(double value)
```


设置绘图区域的高度，单位为图表区域的比例。

**Remarks**

绘图区域边界框包括绘图区域、刻度线（刻度标签）以及刻度线周围的一小段边框。如果该值不是由 MS Excel 创建的，请在调用此方法之前调用 Chart.Calculate() 方法。

**PlotArea** 的 **XRatioToChart**、**YRatioToChart**、**WidthRatioToChart** 和 **HeightRatioToChart** 表示包括绘图区域、刻度线（刻度标签）以及刻度线周围小边框的绘图区域边界框。如果您想获取绘图区域的实际大小，应该调用 **InnerXRatioToChart**、**InnerYRatioToChart**、**InnerWidthRatioToChart** 和 **InnerHeightRatioToChart** 属性。

对于 Excel 2007 及更高版本，默认值为零。您应在调用 Chart.Calculate() 后获取该值。

InnerHeight（像素） = InnerXRatioToChart \* chart.ChartObject.Width。注意：当设置 InnerHeightRatioToChart 时，IsInnerMode 属性将自动设置为 True。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setInnerMode(boolean value) {#setInnerMode-boolean-}
```
public void setInnerMode(boolean value)
```


指示绘图区的大小是否包括刻度线和轴标签。False 表示大小应确定绘图区、刻度线和轴标签的尺寸。

**Remarks**

仅适用于 Xlsx 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setInnerWidth(int value) {#setInnerWidth-int-}
```
public void setInnerWidth(int value)
```


设置绘图区域的宽度，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 PlotArea.InnerWidthRatioToChart 属性。InnerWidth = InnerWidthRatioToChart \* 4000; 此属性将在自 2025 年 2 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setInnerWidthRatioToChart(double value) {#setInnerWidthRatioToChart-double-}
```
public void setInnerWidthRatioToChart(double value)
```


设置绘图区域的宽度，单位为图表区域的比例。

**Remarks**

绘图区域边界框包括绘图区域、刻度线（刻度标签）以及刻度线周围的一小段边框。如果该值不是由 MS Excel 创建的，请在调用此方法之前调用 Chart.Calculate() 方法。

**PlotArea** 的 **XRatioToChart**、**YRatioToChart**、**WidthRatioToChart** 和 **HeightRatioToChart** 表示包括绘图区域、刻度线（刻度标签）以及刻度线周围小边框的绘图区域边界框。如果您想获取绘图区域的实际大小，应该调用 **InnerXRatioToChart**、**InnerYRatioToChart**、**InnerWidthRatioToChart** 和 **InnerHeightRatioToChart** 属性。

对于 Excel 2007 及更高版本，默认值为零。您应在调用 Chart.Calculate() 后获取该值。

InnerWidth（像素） = InnerXRatioToChart \* chart.ChartObject.Width。注意：当设置 InnerWidthRatioToChart 时，IsInnerMode 属性将自动设置为 True。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setInnerX(int value) {#setInnerX-int-}
```
public void setInnerX(int value)
```


设置绘图区域左上角的 x 坐标，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 PlotArea.InnerXRatioToChart 属性。InnerX = InnerXRatioToChart \* 4000. 此属性将在自 2025 年 2 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setInnerXRatioToChart(double value) {#setInnerXRatioToChart-double-}
```
public void setInnerXRatioToChart(double value)
```


获取绘图区左上角的 x 坐标，单位为图表区域的比例。

**Remarks**

绘图区域边界框包括绘图区域、刻度线（刻度标签）以及刻度线周围的一小段边框。如果该值不是由 MS Excel 创建的，请在调用此方法之前调用 Chart.Calculate() 方法。

**PlotArea** 的 **XRatioToChart**、**YRatioToChart**、**WidthRatioToChart** 和 **HeightRatioToChart** 表示包括绘图区域、刻度线（刻度标签）以及刻度线周围小边框的绘图区域边界框。如果您想获取绘图区域的实际大小，应该调用 **InnerXRatioToChart**、**InnerYRatioToChart**、**InnerWidthRatioToChart** 和 **InnerHeightRatioToChart** 属性。

对于 Excel 2007 及更高版本，默认值为零。您应在调用 Chart.Calculate() 后获取该值。

InnerX（像素） = InnerXRatioToChart \* chart.ChartObject.Width。注意：当设置 InnerXRatioToChart 时，IsInnerMode 属性将自动设置为 True。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setInnerY(int value) {#setInnerY-int-}
```
public void setInnerY(int value)
```


设置绘图区域左上角的 x 坐标，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 PlotArea.InnerYRatioToChart 属性。InnerY = InnerYRatioToChart \* 4000。此属性将在自 2025 年 2 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setInnerYRatioToChart(double value) {#setInnerYRatioToChart-double-}
```
public void setInnerYRatioToChart(double value)
```


获取绘图区左上角的 x 坐标，单位为图表区域的比例。

**Remarks**

绘图区域边界框包括绘图区域、刻度线（刻度标签）以及刻度线周围的一小段边框。如果该值不是由 MS Excel 创建的，请在调用此方法之前调用 Chart.Calculate() 方法。

**PlotArea** 的 **XRatioToChart**、**YRatioToChart**、**WidthRatioToChart** 和 **HeightRatioToChart** 表示包括绘图区域、刻度线（刻度标签）以及刻度线周围小边框的绘图区域边界框。如果您想获取绘图区域的实际大小，应该调用 **InnerXRatioToChart**、**InnerYRatioToChart**、**InnerWidthRatioToChart** 和 **InnerHeightRatioToChart** 属性。

对于 Excel 2007 及更高版本，默认值为零。您应在调用 Chart.Calculate() 后获取该值。

InnerY in Pixel = InnerYRatioToChart \* chart.ChartObject.Width。注意：当设置 InnerYRatioToChart 时，IsInnerMode 属性将自动设置为 True。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setPositionAuto() {#setPositionAuto--}
```
public void setPositionAuto()
```


将绘图区域的位置设置为自动

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


如果框架有阴影，则为 true。

**Remarks**

仅适用于 xls 文件中的图表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


设置绘图区域边界框的宽度，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 PlotArea.WidthRatioToChart 属性。Width = WidthRatioToChart \* 4000。此属性将在自 2025 年 2 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


以像素为单位设置框架的宽度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setWidthRatioToChart(double value) {#setWidthRatioToChart-double-}
```
public void setWidthRatioToChart(double value)
```


设置绘图区域边界框的宽度，单位为图表区域的比例。

**Remarks**

绘图区域边界框包括绘图区域、刻度线（刻度标签）以及刻度线周围的一小段边框。如果该值不是由 MS Excel 创建的，请在调用此方法之前调用 Chart.Calculate() 方法。

**PlotArea** 的 **XRatioToChart**、**YRatioToChart**、**WidthRatioToChart** 和 **HeightRatioToChart** 表示包括绘图区域、刻度线（刻度标签）以及刻度线周围小边框的绘图区域边界框。如果您想获取绘图区域的实际大小，应该调用 **InnerXRatioToChart**、**InnerYRatioToChart**、**InnerWidthRatioToChart** 和 **InnerHeightRatioToChart** 属性。

对于 Excel 2007 及更高版本，默认值为零。您应在调用 Chart.Calculate() 后获取该值。

WidthPixel = WidthRatioToChart \* chart.ChartObject.Width。注意：当设置 WidthRatioToChart 时，IsInnerMode 属性将自动设置为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


设置绘图区域边界框左上角的 x 坐标，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 PlotArea.XRatioToChart 属性。X = XRatioToChart \* 4000。此属性将在自 2025 年 2 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setXPixel(int value) {#setXPixel-int-}
```
public void setXPixel(int value)
```


以像素为单位设置左上角的 x 坐标。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setXRatioToChart(double value) {#setXRatioToChart-double-}
```
public void setXRatioToChart(double value)
```


设置绘图区域边界框左上角的 x 坐标，作为图表区域的比例。

**Remarks**

绘图区域边界框包括绘图区域、刻度线（刻度标签）以及刻度线周围的一小段边框。如果该值不是由 MS Excel 创建的，请在调用此方法之前调用 Chart.Calculate() 方法。

**PlotArea** 的 **XRatioToChart**、**YRatioToChart**、**WidthRatioToChart** 和 **HeightRatioToChart** 表示包括绘图区域、刻度线（刻度标签）以及刻度线周围小边框的绘图区域边界框。如果您想获取绘图区域的实际大小，应该调用 **InnerXRatioToChart**、**InnerYRatioToChart**、**InnerWidthRatioToChart** 和 **InnerHeightRatioToChart** 属性。

对于 Excel 2007 及更高版本，默认值为零。您应在调用 Chart.Calculate() 后获取该值。

XPixel = XRatioToChart \* chart.ChartObject.Width。注意：当设置 XRatioToChart 时，IsInnerMode 属性将自动设置为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


设置绘图区域边界框左上角的 y 坐标，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 PlotArea.YRatioToChart 属性。Y = YRatioToChart \* 4000。此属性将在自 2025 年 2 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setYPixel(int value) {#setYPixel-int-}
```
public void setYPixel(int value)
```


以像素为单位设置左上角的 y 坐标。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setYRatioToChart(double value) {#setYRatioToChart-double-}
```
public void setYRatioToChart(double value)
```


设置绘图区域边界框左上角的 y 坐标，作为图表区域的比例。

**Remarks**

绘图区域边界框包括绘图区域、刻度线（刻度标签）以及刻度线周围的一小段边框。如果该值不是由 MS Excel 创建的，请在调用此方法之前调用 Chart.Calculate() 方法。

**PlotArea** 的 **XRatioToChart**、**YRatioToChart**、**WidthRatioToChart** 和 **HeightRatioToChart** 表示包括绘图区域、刻度线（刻度标签）以及刻度线周围小边框的绘图区域边界框。如果您想获取绘图区域的实际大小，应该调用 **InnerXRatioToChart**、**InnerYRatioToChart**、**InnerWidthRatioToChart** 和 **InnerHeightRatioToChart** 属性。

对于 Excel 2007 及更高版本，默认值为零。您应在调用 Chart.Calculate() 后获取该值。

YPixel = YRatioToChart \* chart.ChartObject.Width。注意：当设置 YRatioToChart 时，IsInnerMode 属性将自动设置为 false。

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

