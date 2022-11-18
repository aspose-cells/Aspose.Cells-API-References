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
| [setAutoTickLabelSpacing(boolean value)](#setAutoTickLabelSpacing-boolean-) | For the description of this property, please see \#isAutoTickLabelSpacing().isAutoTickLabelSpacing() |
| [setAutomaticMajorUnit(boolean value)](#setAutomaticMajorUnit-boolean-) | For the description of this property, please see \#isAutomaticMajorUnit().isAutomaticMajorUnit() |
| [setAutomaticMaxValue(boolean value)](#setAutomaticMaxValue-boolean-) | For the description of this property, please see \#isAutomaticMaxValue().isAutomaticMaxValue() |
| [setAutomaticMinValue(boolean value)](#setAutomaticMinValue-boolean-) | For the description of this property, please see \#isAutomaticMinValue().isAutomaticMinValue() |
| [setAutomaticMinorUnit(boolean value)](#setAutomaticMinorUnit-boolean-) | For the description of this property, please see \#isAutomaticMinorUnit().isAutomaticMinorUnit() |
| [setAxisBetweenCategories(boolean value)](#setAxisBetweenCategories-boolean-) | For the description of this property, please see \#getAxisBetweenCategories().getAxisBetweenCategories() |
| [setBaseUnitAuto(boolean value)](#setBaseUnitAuto-boolean-) | For the description of this property, please see \#isBaseUnitAuto().isBaseUnitAuto() |
| [setBaseUnitScale(int value)](#setBaseUnitScale-int-) | For the description of this property, please see \#getBaseUnitScale().getBaseUnitScale() |
| [setCategoryType(int value)](#setCategoryType-int-) | For the description of this property, please see \#getCategoryType().getCategoryType() |
| [setCrossAt(double value)](#setCrossAt-double-) | For the description of this property, please see \#getCrossAt().getCrossAt() |
| [setCrossAtMax(boolean isCrossAtMax)](#setCrossAtMax-boolean-) | Sets whether the axis crosses at the maximum value. |
| [setCrossType(int value)](#setCrossType-int-) | For the description of this property, please see \#getCrossType().getCrossType() |
| [setCustUnit(int value)](#setCustUnit-int-) | For the description of this property, please see \#getCustUnit().getCustUnit() |
| [setDisplayUnit(int value)](#setDisplayUnit-int-) | For the description of this property, please see \#getDisplayUnit().getDisplayUnit() |
| [setDisplayUnitLabelShown(boolean value)](#setDisplayUnitLabelShown-boolean-) | For the description of this property, please see \#isDisplayUnitLabelShown().isDisplayUnitLabelShown() |
| [setHasMultiLevelLabels(boolean value)](#setHasMultiLevelLabels-boolean-) | For the description of this property, please see \#hasMultiLevelLabels().hasMultiLevelLabels() |
| [setLogBase(double value)](#setLogBase-double-) | For the description of this property, please see \#getLogBase().getLogBase() |
| [setLogarithmic(boolean value)](#setLogarithmic-boolean-) | For the description of this property, please see \#isLogarithmic().isLogarithmic() |
| [setMajorTickMark(int value)](#setMajorTickMark-int-) | For the description of this property, please see \#getMajorTickMark().getMajorTickMark() |
| [setMajorUnit(double value)](#setMajorUnit-double-) | For the description of this property, please see \#getMajorUnit().getMajorUnit() |
| [setMajorUnitScale(int value)](#setMajorUnitScale-int-) | For the description of this property, please see \#getMajorUnitScale().getMajorUnitScale() |
| [setMaxValue(Object value)](#setMaxValue-java.lang.Object-) | For the description of this property, please see \#getMaxValue().getMaxValue() |
| [setMinValue(Object value)](#setMinValue-java.lang.Object-) | For the description of this property, please see \#getMinValue().getMinValue() |
| [setMinorTickMark(int value)](#setMinorTickMark-int-) | For the description of this property, please see \#getMinorTickMark().getMinorTickMark() |
| [setMinorUnit(double value)](#setMinorUnit-double-) | For the description of this property, please see \#getMinorUnit().getMinorUnit() |
| [setMinorUnitScale(int value)](#setMinorUnitScale-int-) | For the description of this property, please see \#getMinorUnitScale().getMinorUnitScale() |
| [setPlotOrderReversed(boolean value)](#setPlotOrderReversed-boolean-) | For the description of this property, please see \#isPlotOrderReversed().isPlotOrderReversed() |
| [setTickLabelPosition(int value)](#setTickLabelPosition-int-) | For the description of this property, please see \#getTickLabelPosition().getTickLabelPosition() |
| [setTickLabelSpacing(int value)](#setTickLabelSpacing-int-) | For the description of this property, please see \#getTickLabelSpacing().getTickLabelSpacing() |
| [setTickMarkSpacing(int value)](#setTickMarkSpacing-int-) | For the description of this property, please see \#getTickMarkSpacing().getTickMarkSpacing() |
| [setVisible(boolean value)](#setVisible-boolean-) | For the description of this property, please see \#isVisible().isVisible() |
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


For the description of this property, please see \#isAutoTickLabelSpacing().isAutoTickLabelSpacing()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutomaticMajorUnit(boolean value) {#setAutomaticMajorUnit-boolean-}
```
public void setAutomaticMajorUnit(boolean value)
```


For the description of this property, please see \#isAutomaticMajorUnit().isAutomaticMajorUnit()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutomaticMaxValue(boolean value) {#setAutomaticMaxValue-boolean-}
```
public void setAutomaticMaxValue(boolean value)
```


For the description of this property, please see \#isAutomaticMaxValue().isAutomaticMaxValue()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutomaticMinValue(boolean value) {#setAutomaticMinValue-boolean-}
```
public void setAutomaticMinValue(boolean value)
```


For the description of this property, please see \#isAutomaticMinValue().isAutomaticMinValue()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutomaticMinorUnit(boolean value) {#setAutomaticMinorUnit-boolean-}
```
public void setAutomaticMinorUnit(boolean value)
```


For the description of this property, please see \#isAutomaticMinorUnit().isAutomaticMinorUnit()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAxisBetweenCategories(boolean value) {#setAxisBetweenCategories-boolean-}
```
public void setAxisBetweenCategories(boolean value)
```


For the description of this property, please see \#getAxisBetweenCategories().getAxisBetweenCategories()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setBaseUnitAuto(boolean value) {#setBaseUnitAuto-boolean-}
```
public void setBaseUnitAuto(boolean value)
```


For the description of this property, please see \#isBaseUnitAuto().isBaseUnitAuto()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setBaseUnitScale(int value) {#setBaseUnitScale-int-}
```
public void setBaseUnitScale(int value)
```


For the description of this property, please see \#getBaseUnitScale().getBaseUnitScale()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCategoryType(int value) {#setCategoryType-int-}
```
public void setCategoryType(int value)
```


For the description of this property, please see \#getCategoryType().getCategoryType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCrossAt(double value) {#setCrossAt-double-}
```
public void setCrossAt(double value)
```


For the description of this property, please see \#getCrossAt().getCrossAt()

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


For the description of this property, please see \#getCrossType().getCrossType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCustUnit(int value) {#setCustUnit-int-}
```
public void setCustUnit(int value)
```


For the description of this property, please see \#getCustUnit().getCustUnit()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDisplayUnit(int value) {#setDisplayUnit-int-}
```
public void setDisplayUnit(int value)
```


For the description of this property, please see \#getDisplayUnit().getDisplayUnit()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDisplayUnitLabelShown(boolean value) {#setDisplayUnitLabelShown-boolean-}
```
public void setDisplayUnitLabelShown(boolean value)
```


For the description of this property, please see \#isDisplayUnitLabelShown().isDisplayUnitLabelShown()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHasMultiLevelLabels(boolean value) {#setHasMultiLevelLabels-boolean-}
```
public void setHasMultiLevelLabels(boolean value)
```


For the description of this property, please see \#hasMultiLevelLabels().hasMultiLevelLabels()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLogBase(double value) {#setLogBase-double-}
```
public void setLogBase(double value)
```


For the description of this property, please see \#getLogBase().getLogBase()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setLogarithmic(boolean value) {#setLogarithmic-boolean-}
```
public void setLogarithmic(boolean value)
```


For the description of this property, please see \#isLogarithmic().isLogarithmic()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setMajorTickMark(int value) {#setMajorTickMark-int-}
```
public void setMajorTickMark(int value)
```


For the description of this property, please see \#getMajorTickMark().getMajorTickMark()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMajorUnit(double value) {#setMajorUnit-double-}
```
public void setMajorUnit(double value)
```


For the description of this property, please see \#getMajorUnit().getMajorUnit()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setMajorUnitScale(int value) {#setMajorUnitScale-int-}
```
public void setMajorUnitScale(int value)
```


For the description of this property, please see \#getMajorUnitScale().getMajorUnitScale()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMaxValue(Object value) {#setMaxValue-java.lang.Object-}
```
public void setMaxValue(Object value)
```


For the description of this property, please see \#getMaxValue().getMaxValue()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object |  |

### setMinValue(Object value) {#setMinValue-java.lang.Object-}
```
public void setMinValue(Object value)
```


For the description of this property, please see \#getMinValue().getMinValue()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object |  |

### setMinorTickMark(int value) {#setMinorTickMark-int-}
```
public void setMinorTickMark(int value)
```


For the description of this property, please see \#getMinorTickMark().getMinorTickMark()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMinorUnit(double value) {#setMinorUnit-double-}
```
public void setMinorUnit(double value)
```


For the description of this property, please see \#getMinorUnit().getMinorUnit()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setMinorUnitScale(int value) {#setMinorUnitScale-int-}
```
public void setMinorUnitScale(int value)
```


For the description of this property, please see \#getMinorUnitScale().getMinorUnitScale()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPlotOrderReversed(boolean value) {#setPlotOrderReversed-boolean-}
```
public void setPlotOrderReversed(boolean value)
```


For the description of this property, please see \#isPlotOrderReversed().isPlotOrderReversed()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setTickLabelPosition(int value) {#setTickLabelPosition-int-}
```
public void setTickLabelPosition(int value)
```


For the description of this property, please see \#getTickLabelPosition().getTickLabelPosition()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTickLabelSpacing(int value) {#setTickLabelSpacing-int-}
```
public void setTickLabelSpacing(int value)
```


For the description of this property, please see \#getTickLabelSpacing().getTickLabelSpacing()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTickMarkSpacing(int value) {#setTickMarkSpacing-int-}
```
public void setTickMarkSpacing(int value)
```


For the description of this property, please see \#getTickMarkSpacing().getTickMarkSpacing()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


For the description of this property, please see \#isVisible().isVisible()

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

