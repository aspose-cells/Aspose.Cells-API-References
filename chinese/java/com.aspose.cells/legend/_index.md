---
title: "图例"
second_title: "Aspose.Cells for Java API 参考"
description: "封装表示图表图例的对象。"
type: docs
url: /zh/java/com.aspose.cells/legend/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe), [com.aspose.cells.ChartTextFrame](../../com.aspose.cells/charttextframe)
```
public class Legend extends ChartTextFrame
```

封装表示图表图例的对象。

**Example**

```
         Workbook workbook = new Workbook();
         	Worksheet sheet = workbook.getWorksheets().get(0);
 
         	Cells cells = sheet.getCells();
         	cells.get(0,1).putValue("Income");
         	cells.get(1,0).putValue("Company A");
         	cells.get(2,0).putValue("Company B");
         	cells.get(3,0).putValue("Company C");
         	cells.get(1,1).putValue(10000);
         	cells.get(2,1).putValue(20000);
         	cells.get(3,1).putValue(30000);
 
         	int chartIndex = sheet.getCharts().add(ChartType.COLUMN, 9, 9, 21, 15);
         	Chart chart = sheet.getCharts().get(chartIndex);
         	chart.setChartDataRange("A1:B4", true);
         //Set Legend's width and height
         Legend legend = chart.getLegend();
 
         //Legend is at right side of chart by default.
         //If the legend is at left or right side of the chart, setting Legend.X property will not take effect.
         //If the legend is at top or bottom side of the chart, setting Legend.Y property will not take effect.
         legend.setY(1500);
         legend.setWidth(50);
         legend.setHeight(50); 
         //Set legend's position
         legend.setPosition(LegendPositionType.LEFT);
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [characters(int startIndex, int length)](#characters-int-int-) | 返回一个 Characters 对象，表示文本中的字符范围。 |
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
| [getDirectionType()](#getDirectionType--) | 获取文本的方向。 |
| [getFont()](#getFont--) | 获取指定 ChartFrame 对象的 [getFont()](../../com.aspose.cells/chartframe\#getFont--) 对象。 |
| [getHeight()](#getHeight--) | 获取框架的高度，单位为图表区域的 1/4000。 |
| [getHeightPixel()](#getHeightPixel--) | 获取框架的高度，单位为像素。 |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | 获取框架的高度，单位为图表区域的比例。 |
| [getLegendEntries()](#getLegendEntries--) | 获取指定图表图例中所有 LegendEntry 对象的集合。 |
| [getLegendEntriesLabels()](#getLegendEntriesLabels--) | 在调用 Chart.Calculate() 方法后获取图例条目的标签。 |
| [getLegendLabels()](#getLegendLabels--) | 在调用 Chart.Calculate() 方法后获取图例条目的标签。 |
| [getLinkedSource()](#getLinkedSource--) | 获取对工作表的引用。 |
| [getPosition()](#getPosition--) | 获取图例位置类型。 |
| [getReadingOrder()](#getReadingOrder--) | 表示文本阅读顺序。 |
| [getRotationAngle()](#getRotationAngle--) | 表示文本旋转角度。 |
| [getShadow()](#getShadow--) | 如果框架有阴影，则为 true。 |
| [getShapeProperties()](#getShapeProperties--) | 获取 [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--) 对象。 |
| [getText()](#getText--) | 获取框架标题的文本。 |
| [getTextDirection()](#getTextDirection--) | 表示文本阅读顺序。 |
| [getTextFont()](#getTextFont--) | 获取指定 ChartFrame 对象的 [getFont()](../../com.aspose.cells/chartframe\#getFont--) 对象。 |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | 获取文本的水平对齐方式。 |
| [getTextOptions()](#getTextOptions--) | 获取文本的选项。 |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | 获取文本的垂直对齐方式。 |
| [getWidth()](#getWidth--) | 获取框架的宽度，单位为图表区域的 1/4000。 |
| [getWidthPixel()](#getWidthPixel--) | 获取框架的宽度，单位为像素。 |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | 获取框架的宽度，单位为图表区域的比例。 |
| [getX()](#getX--) | 获取左上角的 x 坐标，单位为图表区域的 1/4000。 |
| [getXPixel()](#getXPixel--) | 获取左上角的 X 坐标，单位为像素。 |
| [getXRatioToChart()](#getXRatioToChart--) | 获取左上角的 x 坐标，单位为图表区域的比例。 |
| [getY()](#getY--) | 获取左上角的 Y 坐标，单位为图表区域的 1/4000。 |
| [getYPixel()](#getYPixel--) | 获取左上角的 Y 坐标，单位为像素。 |
| [getYRatioToChart()](#getYRatioToChart--) | 获取左上角的 y 坐标，单位为图表区域的比例。 |
| [hashCode()](#hashCode--) |  |
| [isAutoText()](#isAutoText--) | 指示文本是自动生成的。 |
| [isAutomaticRotation()](#isAutomaticRotation--) | 指示图表的文本是否自动旋转。 |
| [isAutomaticSize()](#isAutomaticSize--) | 指示图表框架是否自动大小。 |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | 指示是否已设置默认位置（DefaultX、DefaultY、DefaultWidth 和 DefaultHeight）。 |
| [isDeleted()](#isDeleted--) | 指示此数据标签是否已删除。 |
| [isInnerMode()](#isInnerMode--) | 指示绘图区的大小是否包括刻度线和轴标签。 |
| [isOverLay()](#isOverLay--) | 获取是否在不覆盖图表的情况下显示图例。 |
| [isResizeShapeToFitText()](#isResizeShapeToFitText--) | 获取形状是否应自动适配以完整容纳其中描述的文本。 |
| [isTextWrapped()](#isTextWrapped--) | 获取指示文本是否换行的值。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | 如果对象中的文本在对象大小变化时会更改字体大小，则为 True。 |
| [setAutoText(boolean value)](#setAutoText-boolean-) | 指示文本是自动生成的。 |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | 指示图表框架是否自动大小。 |
| [setBackground(int value)](#setBackground-int-) | 设置背景的显示模式。 |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | 设置背景的显示模式。 |
| [setDeleted(boolean value)](#setDeleted-boolean-) | 指示此数据标签是否已删除。 |
| [setDirectionType(int value)](#setDirectionType-int-) | 设置文本的方向。 |
| [setHeight(int value)](#setHeight-int-) | 以图表区域的 1/4000 为单位设置框架的高度。 |
| [setHeightPixel(int value)](#setHeightPixel-int-) | 以像素为单位设置框架的高度。 |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | 以图表区域的比例为单位设置框架的高度。 |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | 指示绘图区的大小是否包括刻度线和轴标签。 |
| [setLinkedSource(String value)](#setLinkedSource-java.lang.String-) | 设置对工作表的引用。 |
| [setOverLay(boolean value)](#setOverLay-boolean-) | 设置是否在不覆盖图表的情况下显示图例。 |
| [setPosition(int value)](#setPosition-int-) | 设置图例位置类型。 |
| [setPositionAuto()](#setPositionAuto--) | 将框架位置设置为自动 |
| [setReadingOrder(int value)](#setReadingOrder-int-) | 表示文本阅读顺序。 |
| [setResizeShapeToFitText(boolean value)](#setResizeShapeToFitText-boolean-) | 设置形状是否应自动适配以完整容纳其中描述的文本。 |
| [setRotationAngle(int value)](#setRotationAngle-int-) | 表示文本旋转角度。 |
| [setShadow(boolean value)](#setShadow-boolean-) | 如果框架有阴影，则为 true。 |
| [setText(String value)](#setText-java.lang.String-) | 设置框架标题的文本。 |
| [setTextDirection(int value)](#setTextDirection-int-) | 表示文本阅读顺序。 |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | 设置文本的水平对齐方式。 |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | 设置文本的垂直对齐方式。 |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | 设置指示文本是否换行的值。 |
| [setWidth(int value)](#setWidth-int-) | 以图表区域的 1/4000 为单位设置框架的宽度。 |
| [setWidthPixel(int value)](#setWidthPixel-int-) | 以像素为单位设置框架的宽度。 |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | 以图表区域的比例为单位设置框架的宽度。 |
| [setX(int value)](#setX-int-) | 设置左上角的 x 坐标，单位为图表区域的 1/4000。 |
| [setXPixel(int value)](#setXPixel-int-) | 以像素为单位设置左上角的 x 坐标。 |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | 设置左上角的 x 坐标，单位为图表区域的比例。 |
| [setY(int value)](#setY-int-) | 以图表区域的 1/4000 为单位设置左上角的 y 坐标。 |
| [setYPixel(int value)](#setYPixel-int-) | 以像素为单位设置左上角的 y 坐标。 |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | 设置左上角的 y 坐标，单位为图表区域的比例。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


返回一个 Characters 对象，表示文本中的字符范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startIndex | int | 字符起始位置的索引。 |
| length | int | 字符数。 |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
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
### getDirectionType() {#getDirectionType--}
```
public int getDirectionType()
```


获取文本的方向。

参见 [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype)。

**Returns:**
int
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


获取框架的高度，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 ChartFrame.HeightRatioToChart 属性。Height = HeightRatioToChart \* 4000。此属性将在自 2025 年 2 月起 12 个月后移除。Aspose 对给您带来的不便表示歉意。

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


获取框架的高度，单位为图表区域的比例。

**Remarks**

这是一个分数值，其有效范围为 0-1。如何将比例单位转换为像素？HeightPixel = HeightRatioToChart \* Chart.ChartObject.Height;

**Returns:**
double
### getLegendEntries() {#getLegendEntries--}
```
public LegendEntryCollection getLegendEntries()
```


获取指定图表图例中所有 LegendEntry 对象的集合。不支持设置曲面图的图例条目。因此，如果图表类型为曲面图，则返回 null。

**Returns:**
[LegendEntryCollection](../../com.aspose.cells/legendentrycollection)
### getLegendEntriesLabels() {#getLegendEntriesLabels--}
```
public ArrayList getLegendEntriesLabels()
```


在调用 Chart.Calculate() 方法后获取图例条目的标签。

**Remarks**

注意：此成员现已过时。请改用 Legend.GetLegendLabels 方法。此属性将在自 2023 年 11 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
java.util.ArrayList
### getLegendLabels() {#getLegendLabels--}
```
public String[] getLegendLabels()
```


在调用 Chart.Calculate() 方法后获取图例条目的标签。

**Returns:**
java.lang.String[]
### getLinkedSource() {#getLinkedSource--}
```
public String getLinkedSource()
```


获取对工作表的引用。

**Returns:**
java.lang.String
### getPosition() {#getPosition--}
```
public int getPosition()
```


获取图例位置类型。

参见 [LegendPositionType](../../com.aspose.cells/legendpositiontype)。

**Remarks**


默认位置在右侧。

如果图例位于图表的左侧或右侧，设置 Legend.X 属性将不起作用。

如果图例位于图表的顶部或底部，设置 Legend.Y 属性将不起作用。


**Returns:**
int
### getReadingOrder() {#getReadingOrder--}
```
public int getReadingOrder()
```


表示文本阅读顺序。

参见 [TextDirectionType](../../com.aspose.cells/textdirectiontype)。

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


表示文本旋转角度。

**Remarks**


0：未旋转。

255：从上到下。

\-90：向下。

90：向上。


**Returns:**
int
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
### getText() {#getText--}
```
public String getText()
```


获取框架标题的文本。

**Returns:**
java.lang.String
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


表示文本阅读顺序。

参见 [TextDirectionType](../../com.aspose.cells/textdirectiontype)。

**Remarks**

注意：此成员已过时。请改用 ChartTextFrame.ReadingOrder 属性。此属性将在自 2020 年 3 月起 12 个月后移除。Aspose 对给您带来的不便表示歉意。

**Returns:**
int
### getTextFont() {#getTextFont--}
```
public Font getTextFont()
```


获取指定 ChartFrame 对象的 [getFont()](../../com.aspose.cells/chartframe\#getFont--) 对象。

**Remarks**

注意：此成员已过时。请改用 ChartFrame.Font 属性。此属性将在自 2012 年 1 月起 12 个月后移除。Aspose 对给您带来的不便表示歉意。

**Returns:**
[Font](../../com.aspose.cells/font)
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```
public int getTextHorizontalAlignment()
```


获取文本的水平对齐方式。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


获取文本的选项。

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getTextVerticalAlignment() {#getTextVerticalAlignment--}
```
public int getTextVerticalAlignment()
```


获取文本的垂直对齐方式。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


获取框架的宽度，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 ChartFrame.WidthRatioToChart 属性。Width = WidthRatioToChart \* 4000; 此属性将在自 2025 年 2 月起 12 个月后移除。Aspose 对给您带来的不便表示歉意。

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


获取框架的宽度，单位为图表区域的比例。

**Remarks**

这是一个分数值，其有效范围为 0-1。如何将比例单位转换为像素？WidthPixel = WidthRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### getX() {#getX--}
```
public int getX()
```


获取左上角的 x 坐标，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 ChartFrame.XRatioToChart 属性。X = XRatioToChart \* 4000。该属性将在自 2025 年 2 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

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


获取左上角的 x 坐标，单位为图表区域的比例。

**Remarks**

这是一个分数值，有效范围为 0-1。如何将比例单位转换为像素？XPixel = XRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


获取左上角的 Y 坐标，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 ChartFrame.YRatioToChart 属性。Y = YRatioToChart \* 4000。该属性将在自 2025 年 2 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

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


获取左上角的 y 坐标，单位为图表区域的比例。

**Remarks**

这是一个分数值，有效范围为 0-1。如何将比例单位转换为像素？YPixel = YRatioToChart \* Chart.ChartObject.Height;

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoText() {#isAutoText--}
```
public boolean isAutoText()
```


指示文本是自动生成的。

**Returns:**
boolean
### isAutomaticRotation() {#isAutomaticRotation--}
```
public boolean isAutomaticRotation()
```


指示图表的文本是否自动旋转。

**Returns:**
boolean
### isAutomaticSize() {#isAutomaticSize--}
```
public boolean isAutomaticSize()
```


指示图表框架是否自动大小。

**Returns:**
boolean
### isDefaultPosBeSet() {#isDefaultPosBeSet--}
```
public boolean isDefaultPosBeSet()
```


指示是否已设置默认位置（DefaultX、DefaultY、DefaultWidth 和 DefaultHeight）。

**Returns:**
boolean
### isDeleted() {#isDeleted--}
```
public boolean isDeleted()
```


指示此数据标签是否已删除。

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
### isOverLay() {#isOverLay--}
```
public boolean isOverLay()
```


获取是否在不覆盖图表的情况下显示图例。

**Returns:**
boolean
### isResizeShapeToFitText() {#isResizeShapeToFitText--}
```
public boolean isResizeShapeToFitText()
```


获取形状是否应自动适配以完整容纳其中的文本。自动适配是指对形状内的文本进行缩放，以容纳所有文本。

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


获取指示文本是否换行的值。

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

### setAutoText(boolean value) {#setAutoText-boolean-}
```
public void setAutoText(boolean value)
```


指示文本是自动生成的。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutomaticSize(boolean value) {#setAutomaticSize-boolean-}
```
public void setAutomaticSize(boolean value)
```


指示图表框架是否自动大小。

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

### setDeleted(boolean value) {#setDeleted-boolean-}
```
public void setDeleted(boolean value)
```


指示此数据标签是否已删除。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDirectionType(int value) {#setDirectionType-int-}
```
public void setDirectionType(int value)
```


设置文本的方向。

参见 [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


以图表区域的 1/4000 为单位设置框架的高度。

**Remarks**

注意：此成员已过时。请改用 ChartFrame.HeightRatioToChart 属性。Height = HeightRatioToChart \* 4000。此属性将在自 2025 年 2 月起 12 个月后移除。Aspose 对给您带来的不便表示歉意。

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


以图表区域的比例为单位设置框架的高度。

**Remarks**

这是一个分数值，其有效范围为 0-1。如何将比例单位转换为像素？HeightPixel = HeightRatioToChart \* Chart.ChartObject.Height;

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

### setLinkedSource(String value) {#setLinkedSource-java.lang.String-}
```
public void setLinkedSource(String value)
```


设置对工作表的引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOverLay(boolean value) {#setOverLay-boolean-}
```
public void setOverLay(boolean value)
```


设置是否在不覆盖图表的情况下显示图例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


设置图例位置类型。

参见 [LegendPositionType](../../com.aspose.cells/legendpositiontype)。

**Remarks**


默认位置在右侧。

如果图例位于图表的左侧或右侧，设置 Legend.X 属性将不起作用。

如果图例位于图表的顶部或底部，设置 Legend.Y 属性将不起作用。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPositionAuto() {#setPositionAuto--}
```
public void setPositionAuto()
```


将框架位置设置为自动

### setReadingOrder(int value) {#setReadingOrder-int-}
```
public void setReadingOrder(int value)
```


表示文本阅读顺序。

参见 [TextDirectionType](../../com.aspose.cells/textdirectiontype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setResizeShapeToFitText(boolean value) {#setResizeShapeToFitText-boolean-}
```
public void setResizeShapeToFitText(boolean value)
```


设置形状是否应自动适配以完整容纳其中的文本。自动适配是指对形状内的文本进行缩放，以容纳所有文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


表示文本旋转角度。

**Remarks**


0：未旋转。

255：从上到下。

\-90：向下。

90：向上。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

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

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


设置框架标题的文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


表示文本阅读顺序。

参见 [TextDirectionType](../../com.aspose.cells/textdirectiontype)。

**Remarks**

注意：此成员已过时。请改用 ChartTextFrame.ReadingOrder 属性。此属性将在自 2020 年 3 月起 12 个月后移除。Aspose 对给您带来的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


设置文本的水平对齐方式。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


设置文本的垂直对齐方式。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


设置指示文本是否换行的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


以图表区域的 1/4000 为单位设置框架的宽度。

**Remarks**

注意：此成员已过时。请改用 ChartFrame.WidthRatioToChart 属性。Width = WidthRatioToChart \* 4000; 此属性将在自 2025 年 2 月起 12 个月后移除。Aspose 对给您带来的不便表示歉意。

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


以图表区域的比例为单位设置框架的宽度。

**Remarks**

这是一个分数值，其有效范围为 0-1。如何将比例单位转换为像素？WidthPixel = WidthRatioToChart \* Chart.ChartObject.Width;

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


设置左上角的 x 坐标，单位为图表区域的 1/4000。

**Remarks**

注意：此成员已过时。请改用 ChartFrame.XRatioToChart 属性。X = XRatioToChart \* 4000。该属性将在自 2025 年 2 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

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


设置左上角的 x 坐标，单位为图表区域的比例。

**Remarks**

这是一个分数值，有效范围为 0-1。如何将比例单位转换为像素？XPixel = XRatioToChart \* Chart.ChartObject.Width;

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


以图表区域的 1/4000 为单位设置左上角的 y 坐标。

**Remarks**

注意：此成员已过时。请改用 ChartFrame.YRatioToChart 属性。Y = YRatioToChart \* 4000。该属性将在自 2025 年 2 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

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


设置左上角的 y 坐标，单位为图表区域的比例。

**Remarks**

这是一个分数值，有效范围为 0-1。如何将比例单位转换为像素？YPixel = YRatioToChart \* Chart.ChartObject.Height;

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

