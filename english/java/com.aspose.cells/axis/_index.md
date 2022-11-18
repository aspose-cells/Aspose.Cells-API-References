---
title: Axis
second_title: Aspose.Cells for Java API Reference
description: Encapsulates the object that represents a charts axis.
type: docs
weight: 30
url: /java/com.aspose.cells/axis/
---

**Inheritance:**
java.lang.Object
```
public class Axis
```

Encapsulates the object that represents a chart's axis.

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
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Gets the [Area](../../com.aspose.cells/area). |
| [getAxisBetweenCategories()](#getAxisBetweenCategories--) | Represents if the value axis crosses the category axis between categories. |
| [getAxisLabels()](#getAxisLabels--) | Gets the labels of the axis after call Chart.Calculate() method. |
| [getAxisLine()](#getAxisLine--) | Gets the appearance of an Axis. |
| [getBaseUnitScale()](#getBaseUnitScale--) | Represents the base unit scale for the category axis. |
| [getBins()](#getBins--) | Represents bins on a chart(Histogram/Pareto) axis |
| [getCategoryType()](#getCategoryType--) | Represents the category axis type. |
| [getClass()](#getClass--) |  |
| [getCrossAt()](#getCrossAt--) | Represents the point on the value axis where the category axis crosses it. |
| [getCrossType()](#getCrossType--) | Represents the [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) on the specified axis where the other axis crosses. |
| [getCustUnit()](#getCustUnit--) | Specifies a custom value for the display unit. |
| [getDisplayUnit()](#getDisplayUnit--) | Represents the unit label for the specified axis. |
| [getDisplayUnitLabel()](#getDisplayUnitLabel--) | Represents a unit label on an axis in the specified chart. |
| [getLogBase()](#getLogBase--) | Represents the logarithmic base. |
| [getMajorGridLines()](#getMajorGridLines--) | Represents major gridlines on a chart axis. |
| [getMajorTickMark()](#getMajorTickMark--) | Represents the type of major tick mark for the specified axis. |
| [getMajorUnit()](#getMajorUnit--) | Represents the major units for the axis. |
| [getMajorUnitScale()](#getMajorUnitScale--) | Represents the major unit scale for the category axis. |
| [getMaxValue()](#getMaxValue--) | Represents the maximum value on the value axis. |
| [getMinValue()](#getMinValue--) | Represents the minimum value on the value axis. |
| [getMinorGridLines()](#getMinorGridLines--) | Represents minor gridlines on a chart axis. |
| [getMinorTickMark()](#getMinorTickMark--) | Represents the type of minor tick mark for the specified axis. |
| [getMinorUnit()](#getMinorUnit--) | Represents the minor units for the axis. |
| [getMinorUnitScale()](#getMinorUnitScale--) | Represents the major unit scale for the category axis. |
| [getTickLabelPosition()](#getTickLabelPosition--) | Represents the position of tick-mark labels on the specified axis. |
| [getTickLabelSpacing()](#getTickLabelSpacing--) | Represents the number of categories or series between tick-mark labels. |
| [getTickLabels()](#getTickLabels--) | Returns a [getTickLabels()](../../com.aspose.cells/axis\#getTickLabels--) object that represents the tick-mark labels for the specified axis. |
| [getTickMarkSpacing()](#getTickMarkSpacing--) | Returns or sets the number of categories or series between tick marks. |
| [getTitle()](#getTitle--) | Gets the axis' title. |
| [hasMultiLevelLabels()](#hasMultiLevelLabels--) | Indicates whether the labels shall be shown as multi level. |
| [hashCode()](#hashCode--) |  |
| [isAutoCross()](#isAutoCross--) | Indicates whether Microsoft Workbook automatically sets the axis crossing point. |
| [isAutoTickLabelSpacing()](#isAutoTickLabelSpacing--) | Indicates whether the spacing of tick label is automatic |
| [isAutomaticMajorUnit()](#isAutomaticMajorUnit--) | Indicates whether the major unit of the axis is automatically assigned. |
| [isAutomaticMaxValue()](#isAutomaticMaxValue--) | Indicates whether the max value is automatically assigned. |
| [isAutomaticMinValue()](#isAutomaticMinValue--) | Indicates whether the min value is automatically assigned. |
| [isAutomaticMinorUnit()](#isAutomaticMinorUnit--) | Indicates whether the minor unit of the axis is automatically assigned. |
| [isBaseUnitAuto()](#isBaseUnitAuto--) | Represents whether the base unit is automatic. |
| [isCrossAtMax()](#isCrossAtMax--) | Indicates whether Microsoft Workbook automatically sets the axis crossing point. |
| [isDisplayUnitLabelShown()](#isDisplayUnitLabelShown--) | Represents if the display unit label is shown on the specified axis. |
| [isLogarithmic()](#isLogarithmic--) | Represents if the value axis scale type is logarithmic or not. |
| [isPlotOrderReversed()](#isPlotOrderReversed--) | Represents if Microsoft Excel plots data points from last to first. |
| [isVisible()](#isVisible--) | Represents if the axis is visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoCross()](#setAutoCross--) | Sets the axis crossing point as automatic. |
| [setAutoTickLabelSpacing(boolean value)](#setAutoTickLabelSpacing-boolean-) | Please see the getter of this property: [isAutoTickLabelSpacing()](../../com.aspose.cells/axis\#isAutoTickLabelSpacing--) |
| [setAutomaticMajorUnit(boolean value)](#setAutomaticMajorUnit-boolean-) | Please see the getter of this property: [isAutomaticMajorUnit()](../../com.aspose.cells/axis\#isAutomaticMajorUnit--) |
| [setAutomaticMaxValue(boolean value)](#setAutomaticMaxValue-boolean-) | Please see the getter of this property: [isAutomaticMaxValue()](../../com.aspose.cells/axis\#isAutomaticMaxValue--) |
| [setAutomaticMinValue(boolean value)](#setAutomaticMinValue-boolean-) | Please see the getter of this property: [isAutomaticMinValue()](../../com.aspose.cells/axis\#isAutomaticMinValue--) |
| [setAutomaticMinorUnit(boolean value)](#setAutomaticMinorUnit-boolean-) | Please see the getter of this property: [isAutomaticMinorUnit()](../../com.aspose.cells/axis\#isAutomaticMinorUnit--) |
| [setAxisBetweenCategories(boolean value)](#setAxisBetweenCategories-boolean-) | Please see the getter of this property: [getAxisBetweenCategories()](../../com.aspose.cells/axis\#getAxisBetweenCategories--) |
| [setBaseUnitAuto(boolean value)](#setBaseUnitAuto-boolean-) | Please see the getter of this property: [isBaseUnitAuto()](../../com.aspose.cells/axis\#isBaseUnitAuto--) |
| [setBaseUnitScale(int value)](#setBaseUnitScale-int-) | Please see the getter of this property: [getBaseUnitScale()](../../com.aspose.cells/axis\#getBaseUnitScale--) |
| [setCategoryType(int value)](#setCategoryType-int-) | Please see the getter of this property: [getCategoryType()](../../com.aspose.cells/axis\#getCategoryType--) |
| [setCrossAt(double value)](#setCrossAt-double-) | Please see the getter of this property: [getCrossAt()](../../com.aspose.cells/axis\#getCrossAt--) |
| [setCrossAtMax(boolean isCrossAtMax)](#setCrossAtMax-boolean-) | Sets whether the axis crosses at the maximum value. |
| [setCrossType(int value)](#setCrossType-int-) | Please see the getter of this property: [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) |
| [setCustUnit(int value)](#setCustUnit-int-) | Please see the getter of this property: [getCustUnit()](../../com.aspose.cells/axis\#getCustUnit--) |
| [setDisplayUnit(int value)](#setDisplayUnit-int-) | Please see the getter of this property: [getDisplayUnit()](../../com.aspose.cells/axis\#getDisplayUnit--) |
| [setDisplayUnitLabelShown(boolean value)](#setDisplayUnitLabelShown-boolean-) | Please see the getter of this property: [isDisplayUnitLabelShown()](../../com.aspose.cells/axis\#isDisplayUnitLabelShown--) |
| [setHasMultiLevelLabels(boolean value)](#setHasMultiLevelLabels-boolean-) | Please see the getter of this property: [hasMultiLevelLabels()](../../com.aspose.cells/axis\#hasMultiLevelLabels--) |
| [setLogBase(double value)](#setLogBase-double-) | Please see the getter of this property: [getLogBase()](../../com.aspose.cells/axis\#getLogBase--) |
| [setLogarithmic(boolean value)](#setLogarithmic-boolean-) | Please see the getter of this property: [isLogarithmic()](../../com.aspose.cells/axis\#isLogarithmic--) |
| [setMajorTickMark(int value)](#setMajorTickMark-int-) | Please see the getter of this property: [getMajorTickMark()](../../com.aspose.cells/axis\#getMajorTickMark--) |
| [setMajorUnit(double value)](#setMajorUnit-double-) | Please see the getter of this property: [getMajorUnit()](../../com.aspose.cells/axis\#getMajorUnit--) |
| [setMajorUnitScale(int value)](#setMajorUnitScale-int-) | Please see the getter of this property: [getMajorUnitScale()](../../com.aspose.cells/axis\#getMajorUnitScale--) |
| [setMaxValue(Object value)](#setMaxValue-java.lang.Object-) | Please see the getter of this property: [getMaxValue()](../../com.aspose.cells/axis\#getMaxValue--) |
| [setMinValue(Object value)](#setMinValue-java.lang.Object-) | Please see the getter of this property: [getMinValue()](../../com.aspose.cells/axis\#getMinValue--) |
| [setMinorTickMark(int value)](#setMinorTickMark-int-) | Please see the getter of this property: [getMinorTickMark()](../../com.aspose.cells/axis\#getMinorTickMark--) |
| [setMinorUnit(double value)](#setMinorUnit-double-) | Please see the getter of this property: [getMinorUnit()](../../com.aspose.cells/axis\#getMinorUnit--) |
| [setMinorUnitScale(int value)](#setMinorUnitScale-int-) | Please see the getter of this property: [getMinorUnitScale()](../../com.aspose.cells/axis\#getMinorUnitScale--) |
| [setPlotOrderReversed(boolean value)](#setPlotOrderReversed-boolean-) | Please see the getter of this property: [isPlotOrderReversed()](../../com.aspose.cells/axis\#isPlotOrderReversed--) |
| [setTickLabelPosition(int value)](#setTickLabelPosition-int-) | Please see the getter of this property: [getTickLabelPosition()](../../com.aspose.cells/axis\#getTickLabelPosition--) |
| [setTickLabelSpacing(int value)](#setTickLabelSpacing-int-) | Please see the getter of this property: [getTickLabelSpacing()](../../com.aspose.cells/axis\#getTickLabelSpacing--) |
| [setTickMarkSpacing(int value)](#setTickMarkSpacing-int-) | Please see the getter of this property: [getTickMarkSpacing()](../../com.aspose.cells/axis\#getTickMarkSpacing--) |
| [setVisible(boolean value)](#setVisible-boolean-) | Please see the getter of this property: [isVisible()](../../com.aspose.cells/axis\#isVisible--) |
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
### getArea() {#getArea--}
```
public Area getArea()
```


Gets the [Area](../../com.aspose.cells/area).

**Returns:**
[Area](../../com.aspose.cells/area)
### getAxisBetweenCategories() {#getAxisBetweenCategories--}
```
public boolean getAxisBetweenCategories()
```


Represents if the value axis crosses the category axis between categories. This property applies only to category axes, and it doesn't apply to 3-D charts.

**Returns:**
boolean
### getAxisLabels() {#getAxisLabels--}
```
public ArrayList getAxisLabels()
```


Gets the labels of the axis after call Chart.Calculate() method.

**Returns:**
java.util.ArrayList
### getAxisLine() {#getAxisLine--}
```
public Line getAxisLine()
```


Gets the appearance of an Axis.

**Returns:**
[Line](../../com.aspose.cells/line)
### getBaseUnitScale() {#getBaseUnitScale--}
```
public int getBaseUnitScale()
```


Represents the base unit scale for the category axis. Setting this property only takes effect when the CategoryType property is set to TimeScale.

**Returns:**
int
### getBins() {#getBins--}
```
public AxisBins getBins()
```


Represents bins on a chart(Histogram/Pareto) axis

**Returns:**
[AxisBins](../../com.aspose.cells/axisbins)
### getCategoryType() {#getCategoryType--}
```
public int getCategoryType()
```


Represents the category axis type.

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


Represents the point on the value axis where the category axis crosses it. The number should be a integer when it applies to category axis. And the value must be between 1 and 31999.

**Returns:**
double
### getCrossType() {#getCrossType--}
```
public int getCrossType()
```


Represents the [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) on the specified axis where the other axis crosses.

**Returns:**
int
### getCustUnit() {#getCustUnit--}
```
public int getCustUnit()
```


Specifies a custom value for the display unit.

**Returns:**
int
### getDisplayUnit() {#getDisplayUnit--}
```
public int getDisplayUnit()
```


Represents the unit label for the specified axis.

**Returns:**
int
### getDisplayUnitLabel() {#getDisplayUnitLabel--}
```
public DisplayUnitLabel getDisplayUnitLabel()
```


Represents a unit label on an axis in the specified chart. Unit labels are useful for charting large values\\u9225?for example, in the millions or billions.

**Returns:**
[DisplayUnitLabel](../../com.aspose.cells/displayunitlabel)
### getLogBase() {#getLogBase--}
```
public double getLogBase()
```


Represents the logarithmic base. Default value is 10.Only applies for Excel2007.

**Returns:**
double
### getMajorGridLines() {#getMajorGridLines--}
```
public Line getMajorGridLines()
```


Represents major gridlines on a chart axis.

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


Represents the type of major tick mark for the specified axis.

**Returns:**
int
### getMajorUnit() {#getMajorUnit--}
```
public double getMajorUnit()
```


Represents the major units for the axis. The major units must be greater than zero.

**Returns:**
double
### getMajorUnitScale() {#getMajorUnitScale--}
```
public int getMajorUnitScale()
```


Represents the major unit scale for the category axis.

```
chart.getCategoryAxis().setCategoryType(CategoryType.TIME_SCALE);
         chart.getCategoryAxis().setMajorUnitScale(TimeUnit.MONTHS);
         chart.getCategoryAxis().setMajorUnit(2);
```

**Returns:**
int
### getMaxValue() {#getMaxValue--}
```
public Object getMaxValue()
```


Represents the maximum value on the value axis. The maxValue type only can be double or DateTime

**Returns:**
java.lang.Object
### getMinValue() {#getMinValue--}
```
public Object getMinValue()
```


Represents the minimum value on the value axis. The minValue type only can be double or DateTime

**Returns:**
java.lang.Object
### getMinorGridLines() {#getMinorGridLines--}
```
public Line getMinorGridLines()
```


Represents minor gridlines on a chart axis.

**Returns:**
[Line](../../com.aspose.cells/line)
### getMinorTickMark() {#getMinorTickMark--}
```
public int getMinorTickMark()
```


Represents the type of minor tick mark for the specified axis.

**Returns:**
int
### getMinorUnit() {#getMinorUnit--}
```
public double getMinorUnit()
```


Represents the minor units for the axis. The minor units must be greater than zero.

**Returns:**
double
### getMinorUnitScale() {#getMinorUnitScale--}
```
public int getMinorUnitScale()
```


Represents the major unit scale for the category axis.

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


Represents the position of tick-mark labels on the specified axis.

**Returns:**
int
### getTickLabelSpacing() {#getTickLabelSpacing--}
```
public int getTickLabelSpacing()
```


Represents the number of categories or series between tick-mark labels. Applies only to category and series axes. The number must be between 1 and 31999.

**Returns:**
int
### getTickLabels() {#getTickLabels--}
```
public TickLabels getTickLabels()
```


Returns a [getTickLabels()](../../com.aspose.cells/axis\#getTickLabels--) object that represents the tick-mark labels for the specified axis.

**Returns:**
[TickLabels](../../com.aspose.cells/ticklabels)
### getTickMarkSpacing() {#getTickMarkSpacing--}
```
public int getTickMarkSpacing()
```


Returns or sets the number of categories or series between tick marks. Applies only to category and series axes. The number must be between 1 and 31999.

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Gets the axis' title.

**Returns:**
[Title](../../com.aspose.cells/title)
### hasMultiLevelLabels() {#hasMultiLevelLabels--}
```
public boolean hasMultiLevelLabels()
```


Indicates whether the labels shall be shown as multi level. Only valid for category axis.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoCross() {#isAutoCross--}
```
public boolean isAutoCross()
```


Indicates whether Microsoft Workbook automatically sets the axis crossing point. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Charts.Axis.CrossType property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isAutoTickLabelSpacing() {#isAutoTickLabelSpacing--}
```
public boolean isAutoTickLabelSpacing()
```


Indicates whether the spacing of tick label is automatic

**Returns:**
boolean
### isAutomaticMajorUnit() {#isAutomaticMajorUnit--}
```
public boolean isAutomaticMajorUnit()
```


Indicates whether the major unit of the axis is automatically assigned.

**Returns:**
boolean
### isAutomaticMaxValue() {#isAutomaticMaxValue--}
```
public boolean isAutomaticMaxValue()
```


Indicates whether the max value is automatically assigned.

**Returns:**
boolean
### isAutomaticMinValue() {#isAutomaticMinValue--}
```
public boolean isAutomaticMinValue()
```


Indicates whether the min value is automatically assigned.

**Returns:**
boolean
### isAutomaticMinorUnit() {#isAutomaticMinorUnit--}
```
public boolean isAutomaticMinorUnit()
```


Indicates whether the minor unit of the axis is automatically assigned.

**Returns:**
boolean
### isBaseUnitAuto() {#isBaseUnitAuto--}
```
public boolean isBaseUnitAuto()
```


Represents whether the base unit is automatic.

**Returns:**
boolean
### isCrossAtMax() {#isCrossAtMax--}
```
public boolean isCrossAtMax()
```


Indicates whether Microsoft Workbook automatically sets the axis crossing point. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Charts.Axis.CrossType property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isDisplayUnitLabelShown() {#isDisplayUnitLabelShown--}
```
public boolean isDisplayUnitLabelShown()
```


Represents if the display unit label is shown on the specified axis. The default value is True.

**Returns:**
boolean
### isLogarithmic() {#isLogarithmic--}
```
public boolean isLogarithmic()
```


Represents if the value axis scale type is logarithmic or not.

**Returns:**
boolean
### isPlotOrderReversed() {#isPlotOrderReversed--}
```
public boolean isPlotOrderReversed()
```


Represents if Microsoft Excel plots data points from last to first.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Represents if the axis is visible.

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




### setAutoCross() {#setAutoCross--}
```
public void setAutoCross()
```


Sets the axis crossing point as automatic. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Charts.Axis.CrossType property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

### setAutoTickLabelSpacing(boolean value) {#setAutoTickLabelSpacing-boolean-}
```
public void setAutoTickLabelSpacing(boolean value)
```


Please see the getter of this property: [isAutoTickLabelSpacing()](../../com.aspose.cells/axis\#isAutoTickLabelSpacing--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutomaticMajorUnit(boolean value) {#setAutomaticMajorUnit-boolean-}
```
public void setAutomaticMajorUnit(boolean value)
```


Please see the getter of this property: [isAutomaticMajorUnit()](../../com.aspose.cells/axis\#isAutomaticMajorUnit--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutomaticMaxValue(boolean value) {#setAutomaticMaxValue-boolean-}
```
public void setAutomaticMaxValue(boolean value)
```


Please see the getter of this property: [isAutomaticMaxValue()](../../com.aspose.cells/axis\#isAutomaticMaxValue--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutomaticMinValue(boolean value) {#setAutomaticMinValue-boolean-}
```
public void setAutomaticMinValue(boolean value)
```


Please see the getter of this property: [isAutomaticMinValue()](../../com.aspose.cells/axis\#isAutomaticMinValue--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutomaticMinorUnit(boolean value) {#setAutomaticMinorUnit-boolean-}
```
public void setAutomaticMinorUnit(boolean value)
```


Please see the getter of this property: [isAutomaticMinorUnit()](../../com.aspose.cells/axis\#isAutomaticMinorUnit--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAxisBetweenCategories(boolean value) {#setAxisBetweenCategories-boolean-}
```
public void setAxisBetweenCategories(boolean value)
```


Please see the getter of this property: [getAxisBetweenCategories()](../../com.aspose.cells/axis\#getAxisBetweenCategories--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setBaseUnitAuto(boolean value) {#setBaseUnitAuto-boolean-}
```
public void setBaseUnitAuto(boolean value)
```


Please see the getter of this property: [isBaseUnitAuto()](../../com.aspose.cells/axis\#isBaseUnitAuto--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setBaseUnitScale(int value) {#setBaseUnitScale-int-}
```
public void setBaseUnitScale(int value)
```


Please see the getter of this property: [getBaseUnitScale()](../../com.aspose.cells/axis\#getBaseUnitScale--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCategoryType(int value) {#setCategoryType-int-}
```
public void setCategoryType(int value)
```


Please see the getter of this property: [getCategoryType()](../../com.aspose.cells/axis\#getCategoryType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCrossAt(double value) {#setCrossAt-double-}
```
public void setCrossAt(double value)
```


Please see the getter of this property: [getCrossAt()](../../com.aspose.cells/axis\#getCrossAt--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setCrossAtMax(boolean isCrossAtMax) {#setCrossAtMax-boolean-}
```
public void setCrossAtMax(boolean isCrossAtMax)
```


Sets whether the axis crosses at the maximum value. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Charts.Axis.CrossType property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isCrossAtMax | boolean |  |

### setCrossType(int value) {#setCrossType-int-}
```
public void setCrossType(int value)
```


Please see the getter of this property: [getCrossType()](../../com.aspose.cells/axis\#getCrossType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCustUnit(int value) {#setCustUnit-int-}
```
public void setCustUnit(int value)
```


Please see the getter of this property: [getCustUnit()](../../com.aspose.cells/axis\#getCustUnit--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDisplayUnit(int value) {#setDisplayUnit-int-}
```
public void setDisplayUnit(int value)
```


Please see the getter of this property: [getDisplayUnit()](../../com.aspose.cells/axis\#getDisplayUnit--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDisplayUnitLabelShown(boolean value) {#setDisplayUnitLabelShown-boolean-}
```
public void setDisplayUnitLabelShown(boolean value)
```


Please see the getter of this property: [isDisplayUnitLabelShown()](../../com.aspose.cells/axis\#isDisplayUnitLabelShown--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHasMultiLevelLabels(boolean value) {#setHasMultiLevelLabels-boolean-}
```
public void setHasMultiLevelLabels(boolean value)
```


Please see the getter of this property: [hasMultiLevelLabels()](../../com.aspose.cells/axis\#hasMultiLevelLabels--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLogBase(double value) {#setLogBase-double-}
```
public void setLogBase(double value)
```


Please see the getter of this property: [getLogBase()](../../com.aspose.cells/axis\#getLogBase--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setLogarithmic(boolean value) {#setLogarithmic-boolean-}
```
public void setLogarithmic(boolean value)
```


Please see the getter of this property: [isLogarithmic()](../../com.aspose.cells/axis\#isLogarithmic--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setMajorTickMark(int value) {#setMajorTickMark-int-}
```
public void setMajorTickMark(int value)
```


Please see the getter of this property: [getMajorTickMark()](../../com.aspose.cells/axis\#getMajorTickMark--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMajorUnit(double value) {#setMajorUnit-double-}
```
public void setMajorUnit(double value)
```


Please see the getter of this property: [getMajorUnit()](../../com.aspose.cells/axis\#getMajorUnit--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setMajorUnitScale(int value) {#setMajorUnitScale-int-}
```
public void setMajorUnitScale(int value)
```


Please see the getter of this property: [getMajorUnitScale()](../../com.aspose.cells/axis\#getMajorUnitScale--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMaxValue(Object value) {#setMaxValue-java.lang.Object-}
```
public void setMaxValue(Object value)
```


Please see the getter of this property: [getMaxValue()](../../com.aspose.cells/axis\#getMaxValue--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object |  |

### setMinValue(Object value) {#setMinValue-java.lang.Object-}
```
public void setMinValue(Object value)
```


Please see the getter of this property: [getMinValue()](../../com.aspose.cells/axis\#getMinValue--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object |  |

### setMinorTickMark(int value) {#setMinorTickMark-int-}
```
public void setMinorTickMark(int value)
```


Please see the getter of this property: [getMinorTickMark()](../../com.aspose.cells/axis\#getMinorTickMark--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMinorUnit(double value) {#setMinorUnit-double-}
```
public void setMinorUnit(double value)
```


Please see the getter of this property: [getMinorUnit()](../../com.aspose.cells/axis\#getMinorUnit--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setMinorUnitScale(int value) {#setMinorUnitScale-int-}
```
public void setMinorUnitScale(int value)
```


Please see the getter of this property: [getMinorUnitScale()](../../com.aspose.cells/axis\#getMinorUnitScale--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPlotOrderReversed(boolean value) {#setPlotOrderReversed-boolean-}
```
public void setPlotOrderReversed(boolean value)
```


Please see the getter of this property: [isPlotOrderReversed()](../../com.aspose.cells/axis\#isPlotOrderReversed--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setTickLabelPosition(int value) {#setTickLabelPosition-int-}
```
public void setTickLabelPosition(int value)
```


Please see the getter of this property: [getTickLabelPosition()](../../com.aspose.cells/axis\#getTickLabelPosition--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTickLabelSpacing(int value) {#setTickLabelSpacing-int-}
```
public void setTickLabelSpacing(int value)
```


Please see the getter of this property: [getTickLabelSpacing()](../../com.aspose.cells/axis\#getTickLabelSpacing--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTickMarkSpacing(int value) {#setTickMarkSpacing-int-}
```
public void setTickMarkSpacing(int value)
```


Please see the getter of this property: [getTickMarkSpacing()](../../com.aspose.cells/axis\#getTickMarkSpacing--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Please see the getter of this property: [isVisible()](../../com.aspose.cells/axis\#isVisible--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

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

