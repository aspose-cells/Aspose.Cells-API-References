---
title: "Axis"
second_title: "Aspose.Cells for Java API 参考"
description: "封装表示图表坐标轴的对象。"
type: docs
url: /zh/java/com.aspose.cells/axis/
---

**Inheritance:**
java.lang.Object
```
public class Axis
```

封装表示图表坐标轴的对象。

**Example**

通过以下代码，您可以学习如何设置轴的单位、最大值和最小值。

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
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(4);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(20);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 25, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
         //Set the max value of value axis
         chart.getValueAxis().setMaxValue(200);
         //Set the min value of value axis
         chart.getValueAxis().setMinValue(0);
         //Set the major unit
         chart.getValueAxis().setMajorUnit(25);
         //Category(X) axis crosses at the maxinum value.
         chart.getValueAxis().setCrossType(CrossType.MAXIMUM);
         //Set he number of categories or series between tick-mark labels. 
         chart.getCategoryAxis().setTickLabelSpacing(2);
 
         //do your business
 
         //Saving the Excel file
         workbook.save("book1.xlsx");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | 获取 [getArea()](../../com.aspose.cells/axis\#getArea--)。 |
| [getAxisBetweenCategories()](#getAxisBetweenCategories--) | 表示数值轴是否在类别之间穿过类别轴。 |
| [getAxisLabels()](#getAxisLabels--) | 在调用 Chart.Calculate() 方法后获取轴的标签。 |
| [getAxisLine()](#getAxisLine--) | 获取轴的外观。 |
| [getAxisTexts()](#getAxisTexts--) | 在调用 Chart.Calculate() 方法后获取轴的标签。 |
| [getBaseUnitScale()](#getBaseUnitScale--) | 表示类别轴的基准单位刻度。 |
| [getBins()](#getBins--) | 表示图表（直方图/帕累托）轴上的箱体。 |
| [getCategoryType()](#getCategoryType--) | 表示类别轴的类型。 |
| [getClass()](#getClass--) |  |
| [getCrossAt()](#getCrossAt--) | 表示数值轴上类别轴交叉的点。 |
| [getCrossType()](#getCrossType--) | 表示在指定轴上另一轴交叉处的 [getCrossType()](../../com.aspose.cells/axis\#getCrossType--)。 |
| [getCustUnit()](#getCustUnit--) | 指定显示单位的自定义值。 |
| [getCustomDisplayUnit()](#getCustomDisplayUnit--) | 指定显示单位的自定义值。 |
| [getCustomUnit()](#getCustomUnit--) | 指定显示单位的自定义值。 |
| [getDisplayUnit()](#getDisplayUnit--) | 表示指定轴的单位标签。 |
| [getDisplayUnitLabel()](#getDisplayUnitLabel--) | 表示指定图表中轴上的单位标签。 |
| [getLogBase()](#getLogBase--) | 表示对数基数。 |
| [getMajorGridLines()](#getMajorGridLines--) | 表示图表轴上的主网格线。 |
| [getMajorTickMark()](#getMajorTickMark--) | 表示指定轴的主刻度标记类型。 |
| [getMajorUnit()](#getMajorUnit--) | 表示轴的主单位。 |
| [getMajorUnitScale()](#getMajorUnitScale--) | 表示类目轴的主单位刻度。 |
| [getMaxValue()](#getMaxValue--) | 表示值轴的最大值。 |
| [getMinValue()](#getMinValue--) | 表示值轴的最小值。 |
| [getMinorGridLines()](#getMinorGridLines--) | 表示图表轴上的次网格线。 |
| [getMinorTickMark()](#getMinorTickMark--) | 表示指定轴的次刻度标记类型。 |
| [getMinorUnit()](#getMinorUnit--) | 表示轴的次单位。 |
| [getMinorUnitScale()](#getMinorUnitScale--) | 表示类目轴的主单位刻度。 |
| [getTickLabelPosition()](#getTickLabelPosition--) | 表示指定轴上刻度标签的位置。 |
| [getTickLabelSpacing()](#getTickLabelSpacing--) | 表示刻度标签之间的类目或系列数量。 |
| [getTickLabels()](#getTickLabels--) | 返回一个 [getTickLabels()](../../com.aspose.cells/axis\#getTickLabels--) 对象，表示指定轴的刻度标签。 |
| [getTickMarkSpacing()](#getTickMarkSpacing--) | 返回或设置刻度之间的类目或系列数量。 |
| [getTitle()](#getTitle--) | 获取此轴在图表中的标题。 |
| [hasMultiLevelLabels()](#hasMultiLevelLabels--) | 指示标签是否应显示为多级。 |
| [hashCode()](#hashCode--) |  |
| [isAutoTickLabelSpacing()](#isAutoTickLabelSpacing--) | 指示刻度标签的间距是否自动 |
| [isAutomaticMajorUnit()](#isAutomaticMajorUnit--) | 指示轴的主单位是否自动分配。 |
| [isAutomaticMaxValue()](#isAutomaticMaxValue--) | 指示最大值是否自动分配。 |
| [isAutomaticMinValue()](#isAutomaticMinValue--) | 指示最小值是否自动分配。 |
| [isAutomaticMinorUnit()](#isAutomaticMinorUnit--) | 指示轴的次单位是否自动分配。 |
| [isBaseUnitAuto()](#isBaseUnitAuto--) | 表示基准单位是否自动。 |
| [isDisplayUnitLabelShown()](#isDisplayUnitLabelShown--) | 表示是否在指定轴上显示单位标签。 |
| [isLogarithmic()](#isLogarithmic--) | 表示值轴的刻度类型是否为对数。 |
| [isPlotOrderReversed()](#isPlotOrderReversed--) | 表示 Microsoft Excel 是否从最后到最先绘制数据点。 |
| [isVisible()](#isVisible--) | 表示轴是否可见。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoTickLabelSpacing(boolean value)](#setAutoTickLabelSpacing-boolean-) | 指示刻度标签的间距是否自动 |
| [setAutomaticMajorUnit(boolean value)](#setAutomaticMajorUnit-boolean-) | 指示轴的主单位是否自动分配。 |
| [setAutomaticMaxValue(boolean value)](#setAutomaticMaxValue-boolean-) | 指示最大值是否自动分配。 |
| [setAutomaticMinValue(boolean value)](#setAutomaticMinValue-boolean-) | 指示最小值是否自动分配。 |
| [setAutomaticMinorUnit(boolean value)](#setAutomaticMinorUnit-boolean-) | 指示轴的次单位是否自动分配。 |
| [setAxisBetweenCategories(boolean value)](#setAxisBetweenCategories-boolean-) | 表示数值轴是否在类别之间穿过类别轴。 |
| [setBaseUnitAuto(boolean value)](#setBaseUnitAuto-boolean-) | 表示基准单位是否自动。 |
| [setBaseUnitScale(int value)](#setBaseUnitScale-int-) | 表示类别轴的基准单位刻度。 |
| [setCategoryType(int value)](#setCategoryType-int-) | 表示类别轴的类型。 |
| [setCrossAt(double value)](#setCrossAt-double-) | 表示数值轴上类别轴交叉的点。 |
| [setCrossType(int value)](#setCrossType-int-) | 表示在指定轴上另一轴交叉处的 [getCrossType()](../../com.aspose.cells/axis\#getCrossType--)。 |
| [setCustUnit(int value)](#setCustUnit-int-) | 指定显示单位的自定义值。 |
| [setCustomDisplayUnit(double value)](#setCustomDisplayUnit-double-) | 指定显示单位的自定义值。 |
| [setCustomUnit(int value)](#setCustomUnit-int-) | 指定显示单位的自定义值。 |
| [setDisplayUnit(int value)](#setDisplayUnit-int-) | 表示指定轴的单位标签。 |
| [setDisplayUnitLabelShown(boolean value)](#setDisplayUnitLabelShown-boolean-) | 表示是否在指定轴上显示单位标签。 |
| [setHasMultiLevelLabels(boolean value)](#setHasMultiLevelLabels-boolean-) | 指示标签是否应显示为多级。 |
| [setLogBase(double value)](#setLogBase-double-) | 表示对数基数。 |
| [setLogarithmic(boolean value)](#setLogarithmic-boolean-) | 表示值轴的刻度类型是否为对数。 |
| [setMajorTickMark(int value)](#setMajorTickMark-int-) | 表示指定轴的主刻度标记类型。 |
| [setMajorUnit(double value)](#setMajorUnit-double-) | 表示轴的主单位。 |
| [setMajorUnitScale(int value)](#setMajorUnitScale-int-) | 表示类目轴的主单位刻度。 |
| [setMaxValue(Object value)](#setMaxValue-java.lang.Object-) | 表示值轴的最大值。 |
| [setMinValue(Object value)](#setMinValue-java.lang.Object-) | 表示值轴的最小值。 |
| [setMinorTickMark(int value)](#setMinorTickMark-int-) | 表示指定轴的次刻度标记类型。 |
| [setMinorUnit(double value)](#setMinorUnit-double-) | 表示轴的次单位。 |
| [setMinorUnitScale(int value)](#setMinorUnitScale-int-) | 表示类目轴的主单位刻度。 |
| [setPlotOrderReversed(boolean value)](#setPlotOrderReversed-boolean-) | 表示 Microsoft Excel 是否从最后到最先绘制数据点。 |
| [setTickLabelPosition(int value)](#setTickLabelPosition-int-) | 表示指定轴上刻度标签的位置。 |
| [setTickLabelSpacing(int value)](#setTickLabelSpacing-int-) | 表示刻度标签之间的类目或系列数量。 |
| [setTickMarkSpacing(int value)](#setTickMarkSpacing-int-) | 返回或设置刻度之间的类目或系列数量。 |
| [setVisible(boolean value)](#setVisible-boolean-) | 表示轴是否可见。 |
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


获取 [getArea()](../../com.aspose.cells/axis\#getArea--)。

**Returns:**
[Area](../../com.aspose.cells/area)
### getAxisBetweenCategories() {#getAxisBetweenCategories--}
```
public boolean getAxisBetweenCategories()
```


表示数值轴是否在类别之间穿过类别轴。

**Remarks**

此属性仅适用于类目轴，不适用于 3-D 图表。

**Returns:**
boolean
### getAxisLabels() {#getAxisLabels--}
```
public ArrayList getAxisLabels()
```


在调用 Chart.Calculate() 方法后获取轴的标签。

**Remarks**

注意：此成员现已过时。请改用 Axis.GetAxisTexts 方法。此属性将在自 2023 年 11 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
java.util.ArrayList
### getAxisLine() {#getAxisLine--}
```
public Line getAxisLine()
```


获取轴的外观。

**Returns:**
[Line](../../com.aspose.cells/line)
### getAxisTexts() {#getAxisTexts--}
```
public String[] getAxisTexts()
```


在调用 Chart.Calculate() 方法后获取轴的标签。

**Returns:**
java.lang.String[]
### getBaseUnitScale() {#getBaseUnitScale--}
```
public int getBaseUnitScale()
```


表示类别轴的基准单位刻度。

参见 [TimeUnit](../../com.aspose.cells/timeunit)。

**Remarks**

仅在 CategoryType 属性设置为 TimeScale 时生效。

**Returns:**
int
### getBins() {#getBins--}
```
public AxisBins getBins()
```


表示图表（直方图/帕累托）轴上的箱体。

**Remarks**

仅适用于直方图或帕累托图。

**Returns:**
[AxisBins](../../com.aspose.cells/axisbins)
### getCategoryType() {#getCategoryType--}
```
public int getCategoryType()
```


表示类别轴的类型。

参见 [CategoryType](../../com.aspose.cells/categorytype)。

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCrossAt() {#getCrossAt--}
```
public double getCrossAt()
```


表示数值轴上类别轴交叉的点。

**Remarks**

当适用于分类轴时，该数字应为整数，并且值必须在 1 到 31999 之间。

**Returns:**
double
### getCrossType() {#getCrossType--}
```
public int getCrossType()
```


表示在指定轴上另一轴交叉处的 [getCrossType()](../../com.aspose.cells/axis\#getCrossType--)。

参见 [CrossType](../../com.aspose.cells/crosstype)。

**Returns:**
int
### getCustUnit() {#getCustUnit--}
```
public int getCustUnit()
```


指定显示单位的自定义值。

**Remarks**

注意：此属性现已过时。请改用 Axis.CustomUnit 属性。此属性将在自 2023 年 1 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getCustomDisplayUnit() {#getCustomDisplayUnit--}
```
public double getCustomDisplayUnit()
```


指定显示单位的自定义值。

**Returns:**
double
### getCustomUnit() {#getCustomUnit--}
```
public int getCustomUnit()
```


指定显示单位的自定义值。

**Remarks**

注意：此属性现已过时。请改用 Axis.CustomDisplayUnit 属性。此属性将在自 2025 年 2 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getDisplayUnit() {#getDisplayUnit--}
```
public int getDisplayUnit()
```


表示指定轴的单位标签。

参见 [DisplayUnitType](../../com.aspose.cells/displayunittype)。

**Returns:**
int
### getDisplayUnitLabel() {#getDisplayUnitLabel--}
```
public DisplayUnitLabel getDisplayUnitLabel()
```


表示指定图表中坐标轴上的单位标签。单位标签对于绘制大数值（例如百万或十亿）很有用。

**Returns:**
[DisplayUnitLabel](../../com.aspose.cells/displayunitlabel)
### getLogBase() {#getLogBase--}
```
public double getLogBase()
```


表示对数基数。默认值为 10。

**Returns:**
double
### getMajorGridLines() {#getMajorGridLines--}
```
public Line getMajorGridLines()
```


表示图表轴上的主网格线。

**Example**

```
         chart.getValueAxis().getMajorGridLines().setVisible(false);
         chart.getCategoryAxis().getMajorGridLines().setVisible(true);
```

**Returns:**
[Line](../../com.aspose.cells/line)
### getMajorTickMark() {#getMajorTickMark--}
```
public int getMajorTickMark()
```


表示指定轴的主刻度标记类型。

参见 [TickMarkType](../../com.aspose.cells/tickmarktype)。

**Returns:**
int
### getMajorUnit() {#getMajorUnit--}
```
public double getMajorUnit()
```


表示轴的主单位。

**Remarks**

主单位必须大于零。

**Returns:**
double
### getMajorUnitScale() {#getMajorUnitScale--}
```
public int getMajorUnitScale()
```


表示类目轴的主单位刻度。

参见 [TimeUnit](../../com.aspose.cells/timeunit)。

**Example**

```
         chart.getCategoryAxis().setCategoryType(CategoryType.TIME_SCALE);
         /*TimeUnit*/int majorUnitScale = chart.getCategoryAxis().getMajorUnitScale(); //get
         chart.getCategoryAxis().setMajorUnitScale(majorUnitScale); //set
         chart.getCategoryAxis().setMajorUnit(2);
```

**Returns:**
int
### getMaxValue() {#getMaxValue--}
```
public Object getMaxValue()
```


表示值轴的最大值。

**Remarks**

maxValue 类型只能是 double 或 DateTime。

**Returns:**
java.lang.Object
### getMinValue() {#getMinValue--}
```
public Object getMinValue()
```


表示值轴的最小值。

**Remarks**

minValue 类型只能是 double 或 DateTime。

**Returns:**
java.lang.Object
### getMinorGridLines() {#getMinorGridLines--}
```
public Line getMinorGridLines()
```


表示图表轴上的次网格线。

**Returns:**
[Line](../../com.aspose.cells/line)
### getMinorTickMark() {#getMinorTickMark--}
```
public int getMinorTickMark()
```


表示指定轴的次刻度标记类型。

参见 [TickMarkType](../../com.aspose.cells/tickmarktype)。

**Returns:**
int
### getMinorUnit() {#getMinorUnit--}
```
public double getMinorUnit()
```


表示轴的次单位。

**Remarks**

次单位必须大于零。

**Returns:**
double
### getMinorUnitScale() {#getMinorUnitScale--}
```
public int getMinorUnitScale()
```


表示类目轴的主单位刻度。

参见 [TimeUnit](../../com.aspose.cells/timeunit)。

**Example**

```
         chart.getCategoryAxis().setCategoryType(CategoryType.TIME_SCALE);
         chart.getCategoryAxis().setMinorUnitScale(TimeUnit.MONTHS);
         chart.getCategoryAxis().setMinorUnit(2);
```

**Returns:**
int
### getTickLabelPosition() {#getTickLabelPosition--}
```
public int getTickLabelPosition()
```


表示指定轴上刻度标签的位置。

参见 [TickLabelPositionType](../../com.aspose.cells/ticklabelpositiontype)。

**Returns:**
int
### getTickLabelSpacing() {#getTickLabelSpacing--}
```
public int getTickLabelSpacing()
```


表示刻度标签之间的分类或系列数量。仅适用于分类轴和系列轴。

**Remarks**

该数字必须在 1 到 31999 之间。

**Returns:**
int
### getTickLabels() {#getTickLabels--}
```
public TickLabels getTickLabels()
```


返回一个 [getTickLabels()](../../com.aspose.cells/axis\#getTickLabels--) 对象，表示指定轴的刻度标签。

**Returns:**
[TickLabels](../../com.aspose.cells/ticklabels)
### getTickMarkSpacing() {#getTickMarkSpacing--}
```
public int getTickMarkSpacing()
```


返回或设置刻度之间的分类或系列数量。仅适用于分类轴和系列轴。

**Remarks**

该数字必须在 1 到 31999 之间。

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


获取此轴在图表中的标题。

**Returns:**
[Title](../../com.aspose.cells/title)
### hasMultiLevelLabels() {#hasMultiLevelLabels--}
```
public boolean hasMultiLevelLabels()
```


指示标签是否应显示为多级。

**Remarks**

仅对分类轴有效。

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoTickLabelSpacing() {#isAutoTickLabelSpacing--}
```
public boolean isAutoTickLabelSpacing()
```


指示刻度标签的间距是否自动

**Returns:**
boolean
### isAutomaticMajorUnit() {#isAutomaticMajorUnit--}
```
public boolean isAutomaticMajorUnit()
```


指示轴的主单位是否自动分配。

**Returns:**
boolean
### isAutomaticMaxValue() {#isAutomaticMaxValue--}
```
public boolean isAutomaticMaxValue()
```


指示最大值是否自动分配。

**Returns:**
boolean
### isAutomaticMinValue() {#isAutomaticMinValue--}
```
public boolean isAutomaticMinValue()
```


指示最小值是否自动分配。

**Returns:**
boolean
### isAutomaticMinorUnit() {#isAutomaticMinorUnit--}
```
public boolean isAutomaticMinorUnit()
```


指示轴的次单位是否自动分配。

**Returns:**
boolean
### isBaseUnitAuto() {#isBaseUnitAuto--}
```
public boolean isBaseUnitAuto()
```


表示基准单位是否自动。

**Returns:**
boolean
### isDisplayUnitLabelShown() {#isDisplayUnitLabelShown--}
```
public boolean isDisplayUnitLabelShown()
```


表示是否在指定轴上显示单位标签。

**Remarks**

默认值为 True。仅在 [getDisplayUnit()](../../com.aspose.cells/axis\#getDisplayUnit--) 不为 [DisplayUnitType.NONE](../../com.aspose.cells/displayunittype\#NONE) 时有效。

**Returns:**
boolean
### isLogarithmic() {#isLogarithmic--}
```
public boolean isLogarithmic()
```


表示值轴的刻度类型是否为对数。

**Returns:**
boolean
### isPlotOrderReversed() {#isPlotOrderReversed--}
```
public boolean isPlotOrderReversed()
```


表示 Microsoft Excel 是否从最后到最先绘制数据点。

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


表示轴是否可见。

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




### setAutoTickLabelSpacing(boolean value) {#setAutoTickLabelSpacing-boolean-}
```
public void setAutoTickLabelSpacing(boolean value)
```


指示刻度标签的间距是否自动

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutomaticMajorUnit(boolean value) {#setAutomaticMajorUnit-boolean-}
```
public void setAutomaticMajorUnit(boolean value)
```


指示轴的主单位是否自动分配。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutomaticMaxValue(boolean value) {#setAutomaticMaxValue-boolean-}
```
public void setAutomaticMaxValue(boolean value)
```


指示最大值是否自动分配。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutomaticMinValue(boolean value) {#setAutomaticMinValue-boolean-}
```
public void setAutomaticMinValue(boolean value)
```


指示最小值是否自动分配。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutomaticMinorUnit(boolean value) {#setAutomaticMinorUnit-boolean-}
```
public void setAutomaticMinorUnit(boolean value)
```


指示轴的次单位是否自动分配。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAxisBetweenCategories(boolean value) {#setAxisBetweenCategories-boolean-}
```
public void setAxisBetweenCategories(boolean value)
```


表示数值轴是否在类别之间穿过类别轴。

**Remarks**

此属性仅适用于类目轴，不适用于 3-D 图表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setBaseUnitAuto(boolean value) {#setBaseUnitAuto-boolean-}
```
public void setBaseUnitAuto(boolean value)
```


表示基准单位是否自动。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setBaseUnitScale(int value) {#setBaseUnitScale-int-}
```
public void setBaseUnitScale(int value)
```


表示类别轴的基准单位刻度。

参见 [TimeUnit](../../com.aspose.cells/timeunit)。

**Remarks**

仅在 CategoryType 属性设置为 TimeScale 时生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setCategoryType(int value) {#setCategoryType-int-}
```
public void setCategoryType(int value)
```


表示类别轴的类型。

参见 [CategoryType](../../com.aspose.cells/categorytype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setCrossAt(double value) {#setCrossAt-double-}
```
public void setCrossAt(double value)
```


表示数值轴上类别轴交叉的点。

**Remarks**

当适用于分类轴时，该数字应为整数，并且值必须在 1 到 31999 之间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setCrossType(int value) {#setCrossType-int-}
```
public void setCrossType(int value)
```


表示在指定轴上另一轴交叉处的 [getCrossType()](../../com.aspose.cells/axis\#getCrossType--)。

参见 [CrossType](../../com.aspose.cells/crosstype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setCustUnit(int value) {#setCustUnit-int-}
```
public void setCustUnit(int value)
```


指定显示单位的自定义值。

**Remarks**

注意：此属性现已过时。请改用 Axis.CustomUnit 属性。此属性将在自 2023 年 1 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setCustomDisplayUnit(double value) {#setCustomDisplayUnit-double-}
```
public void setCustomDisplayUnit(double value)
```


指定显示单位的自定义值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setCustomUnit(int value) {#setCustomUnit-int-}
```
public void setCustomUnit(int value)
```


指定显示单位的自定义值。

**Remarks**

注意：此属性现已过时。请改用 Axis.CustomDisplayUnit 属性。此属性将在自 2025 年 2 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setDisplayUnit(int value) {#setDisplayUnit-int-}
```
public void setDisplayUnit(int value)
```


表示指定轴的单位标签。

参见 [DisplayUnitType](../../com.aspose.cells/displayunittype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setDisplayUnitLabelShown(boolean value) {#setDisplayUnitLabelShown-boolean-}
```
public void setDisplayUnitLabelShown(boolean value)
```


表示是否在指定轴上显示单位标签。

**Remarks**

默认值为 True。仅在 [getDisplayUnit()](../../com.aspose.cells/axis\#getDisplayUnit--) 不为 [DisplayUnitType.NONE](../../com.aspose.cells/displayunittype\#NONE) 时有效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHasMultiLevelLabels(boolean value) {#setHasMultiLevelLabels-boolean-}
```
public void setHasMultiLevelLabels(boolean value)
```


指示标签是否应显示为多级。

**Remarks**

仅对分类轴有效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setLogBase(double value) {#setLogBase-double-}
```
public void setLogBase(double value)
```


表示对数基数。默认值为 10。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setLogarithmic(boolean value) {#setLogarithmic-boolean-}
```
public void setLogarithmic(boolean value)
```


表示值轴的刻度类型是否为对数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setMajorTickMark(int value) {#setMajorTickMark-int-}
```
public void setMajorTickMark(int value)
```


表示指定轴的主刻度标记类型。

参见 [TickMarkType](../../com.aspose.cells/tickmarktype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMajorUnit(double value) {#setMajorUnit-double-}
```
public void setMajorUnit(double value)
```


表示轴的主单位。

**Remarks**

主单位必须大于零。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setMajorUnitScale(int value) {#setMajorUnitScale-int-}
```
public void setMajorUnitScale(int value)
```


表示类目轴的主单位刻度。

参见 [TimeUnit](../../com.aspose.cells/timeunit)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMaxValue(Object value) {#setMaxValue-java.lang.Object-}
```
public void setMaxValue(Object value)
```


表示值轴的最大值。

**Remarks**

maxValue 类型只能是 double 或 DateTime。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object |  |

### setMinValue(Object value) {#setMinValue-java.lang.Object-}
```
public void setMinValue(Object value)
```


表示值轴的最小值。

**Remarks**

minValue 类型只能是 double 或 DateTime。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object |  |

### setMinorTickMark(int value) {#setMinorTickMark-int-}
```
public void setMinorTickMark(int value)
```


表示指定轴的次刻度标记类型。

参见 [TickMarkType](../../com.aspose.cells/tickmarktype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMinorUnit(double value) {#setMinorUnit-double-}
```
public void setMinorUnit(double value)
```


表示轴的次单位。

**Remarks**

次单位必须大于零。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setMinorUnitScale(int value) {#setMinorUnitScale-int-}
```
public void setMinorUnitScale(int value)
```


表示类目轴的主单位刻度。

参见 [TimeUnit](../../com.aspose.cells/timeunit)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPlotOrderReversed(boolean value) {#setPlotOrderReversed-boolean-}
```
public void setPlotOrderReversed(boolean value)
```


表示 Microsoft Excel 是否从最后到最先绘制数据点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setTickLabelPosition(int value) {#setTickLabelPosition-int-}
```
public void setTickLabelPosition(int value)
```


表示指定轴上刻度标签的位置。

参见 [TickLabelPositionType](../../com.aspose.cells/ticklabelpositiontype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTickLabelSpacing(int value) {#setTickLabelSpacing-int-}
```
public void setTickLabelSpacing(int value)
```


表示刻度标签之间的分类或系列数量。仅适用于分类轴和系列轴。

**Remarks**

该数字必须在 1 到 31999 之间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTickMarkSpacing(int value) {#setTickMarkSpacing-int-}
```
public void setTickMarkSpacing(int value)
```


返回或设置刻度之间的分类或系列数量。仅适用于分类轴和系列轴。

**Remarks**

该数字必须在 1 到 31999 之间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


表示轴是否可见。

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

