---
title: DataLabels
second_title: Aspose.Cells for Java API Reference
description: Encapsulates a collection of all the DataLabel objects for the specified Series.
type: docs
url: /java/com.aspose.cells/datalabels/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe), [com.aspose.cells.ChartTextFrame](../../com.aspose.cells/charttextframe)
```
public class DataLabels extends ChartTextFrame
```

Encapsulates a collection of all the DataLabel objects for the specified Series.

**Example**

```
         //Set the DataLabels in the chart
         Workbook wb = new Workbook("chart.xlsx");
         Chart chart = wb.getWorksheets().get(0).getCharts().get(0);
         DataLabels datalabels;
         for (int i = 0; i  <chart.getNSeries().getCount(); i++)
         {
             datalabels = chart.getNSeries().get(i).getDataLabels();
             //Set the position of DataLabels
             datalabels.setPosition(LabelPositionType.INSIDE_BASE);
             //Show the category name in the DataLabels
             datalabels.setShowCategoryName(true);
             //Show the value in the DataLabels
             datalabels.setShowValue(true);
             //Not show the percentage in the DataLabels
             datalabels.setShowPercentage(false);
             //Not show the legend key.
             datalabels.setShowLegendKey(false);
         }
```
## Methods

| Method | Description |
| --- | --- |
| [applyFont()](#applyFont--) | Apply the font of the datalabels to all child nodes. |
| [characters(int startIndex, int length)](#characters-int-int-) | Returns a Characters object that represents a range of characters within the text. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Gets the [Area](../../com.aspose.cells/area). |
| [getAutoScaleFont()](#getAutoScaleFont--) | True if the text in the object changes font size when the object size changes. |
| [getBackground()](#getBackground--) | Gets the display mode of the background |
| [getBackgroundMode()](#getBackgroundMode--) | Gets the display mode of the background |
| [getBorder()](#getBorder--) | Gets the [Line](../../com.aspose.cells/line). |
| [getChart()](#getChart--) | Gets the chart to which this object belongs. |
| [getClass()](#getClass--) |  |
| [getDefaultHeight()](#getDefaultHeight--) | Represents height of default position in units of 1/4000 of the chart area. |
| [getDefaultHeightRatioToChart()](#getDefaultHeightRatioToChart--) | Represents height of default position in units of Fraction of the chart area. |
| [getDefaultWidth()](#getDefaultWidth--) | Represents width of default position in units of 1/4000 of the chart area. |
| [getDefaultWidthRatioToChart()](#getDefaultWidthRatioToChart--) | Represents width of default position in units of Fraction of the chart area. |
| [getDefaultX()](#getDefaultX--) | Represents x of default position in units of 1/4000 of the chart area. |
| [getDefaultXRatioToChart()](#getDefaultXRatioToChart--) | Represents x of default position in units of Fraction of the chart area. |
| [getDefaultY()](#getDefaultY--) | Represents y of default position in units of 1/4000 of the chart area. |
| [getDefaultYRatioToChart()](#getDefaultYRatioToChart--) | Represents y of default position in units of Fraction of the chart area. |
| [getDirectionType()](#getDirectionType--) | Gets the direction of text. |
| [getFont()](#getFont--) | Gets the font of the DataLabels; |
| [getHeight()](#getHeight--) | Gets the height of frame in units of 1/4000 of the chart area. |
| [getHeightPixel()](#getHeightPixel--) | Gets the height of frame in units of Pixel. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | Gets the height of frame in units of ratio of the chart area. |
| [getLinkedSource()](#getLinkedSource--) | Gets a reference to the worksheet. |
| [getNumber()](#getNumber--) | Gets the built-in number format. |
| [getNumberFormat()](#getNumberFormat--) | Represents the format string for the DataLabels object. |
| [getNumberFormatLinked()](#getNumberFormatLinked--) | True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells). |
| [getPosition()](#getPosition--) | Represents the position of the data label. |
| [getReadingOrder()](#getReadingOrder--) | Represents text reading order. |
| [getRotationAngle()](#getRotationAngle--) | Represents text rotation angle. |
| [getSeparatorType()](#getSeparatorType--) | Gets the separator type used for the data labels on a chart. |
| [getSeparatorValue()](#getSeparatorValue--) | Gets the separator value used for the data labels on a chart. |
| [getShadow()](#getShadow--) | True if the frame has a shadow. |
| [getShapeProperties()](#getShapeProperties--) | Gets the [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--) object. |
| [getShapeType()](#getShapeType--) | Gets shape type of data label. |
| [getShowBubbleSize()](#getShowBubbleSize--) | Represents a specified chart's data label percentage value display behavior. |
| [getShowCategoryName()](#getShowCategoryName--) | Represents a specified chart's data label category name display behavior.True to display the category name for the data labels on a chart. |
| [getShowCellRange()](#getShowCellRange--) | Indicates whether showing cell range as the data labels. |
| [getShowLegendKey()](#getShowLegendKey--) | Represents a specified chart's data label legend key display behavior. |
| [getShowPercentage()](#getShowPercentage--) | Represents a specified chart's data label percentage value display behavior. |
| [getShowSeriesName()](#getShowSeriesName--) | Indicates whether the series name displays for the data labels on a chart. |
| [getShowValue()](#getShowValue--) | Represents a specified chart's data label values display behavior. |
| [getText()](#getText--) | Gets the text of data label. |
| [getTextDirection()](#getTextDirection--) | Represents text reading order. |
| [getTextFont()](#getTextFont--) | Gets a [ChartArea.getFont()](../../com.aspose.cells/chartarea\#getFont--) object of the specified ChartFrame object. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Gets the text horizontal alignment. |
| [getTextOptions()](#getTextOptions--) | Gets the options of the text. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Gets the text vertical alignment of text. |
| [getWidth()](#getWidth--) | Gets the width of frame in units of 1/4000 of the chart area. |
| [getWidthPixel()](#getWidthPixel--) | Gets the width of frame in units of Pixel. |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | Gets the width of frame in units of ratio of the chart area. |
| [getX()](#getX--) | Gets the x coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [getXPixel()](#getXPixel--) | Gets the x coordinate of the upper left corner in units of Pixel. |
| [getXRatioToChart()](#getXRatioToChart--) | Gets the x coordinate of the upper left corner in units of ratio of the chart area. |
| [getY()](#getY--) | Gets the y coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [getYPixel()](#getYPixel--) | Gets the y coordinate of the upper left corner in units of Pixel. |
| [getYRatioToChart()](#getYRatioToChart--) | Gets the y coordinate of the upper left corner in units of ratio of the chart area. |
| [hashCode()](#hashCode--) |  |
| [isAutoText()](#isAutoText--) | Indicates the text is auto generated. |
| [isAutomaticRotation()](#isAutomaticRotation--) | Indicates whether the text of the chart is automatically rotated. |
| [isAutomaticSize()](#isAutomaticSize--) | Indicates whether the chart frame is automatic sized. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [isDeleted()](#isDeleted--) | Indicates whether this data labels is deleted. |
| [isInnerMode()](#isInnerMode--) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. |
| [isNeverOverlap()](#isNeverOverlap--) | Indicates whether the datalabels display never overlap. |
| [isResizeShapeToFitText()](#isResizeShapeToFitText--) | Gets whether a shape should be auto-fit to fully contain the text described within it. |
| [isTextWrapped()](#isTextWrapped--) | Gets a value indicating whether the text is wrapped. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | True if the text in the object changes font size when the object size changes. |
| [setAutoText(boolean value)](#setAutoText-boolean-) | Indicates the text is auto generated. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Indicates whether the chart frame is automatic sized. |
| [setBackground(int value)](#setBackground-int-) | Sets the display mode of the background |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Sets the display mode of the background |
| [setDeleted(boolean value)](#setDeleted-boolean-) | Indicates whether this data labels is deleted. |
| [setDirectionType(int value)](#setDirectionType-int-) | Sets the direction of text. |
| [setHeight(int value)](#setHeight-int-) | Sets the height of frame in units of 1/4000 of the chart area. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Sets the height of frame in units of Pixel. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | Sets the height of frame in units of ratio of the chart area. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. |
| [setLinkedSource(String value)](#setLinkedSource-java.lang.String-) | Sets a reference to the worksheet. |
| [setNeverOverlap(boolean value)](#setNeverOverlap-boolean-) | Indicates whether the datalabels display never overlap. |
| [setNumber(int value)](#setNumber-int-) | Sets the built-in number format. |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | Represents the format string for the DataLabels object. |
| [setNumberFormatLinked(boolean value)](#setNumberFormatLinked-boolean-) | True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells). |
| [setPosition(int value)](#setPosition-int-) | Represents the position of the data label. |
| [setPositionAuto()](#setPositionAuto--) | Set position of the frame to automatic |
| [setReadingOrder(int value)](#setReadingOrder-int-) | Represents text reading order. |
| [setResizeShapeToFitText(boolean value)](#setResizeShapeToFitText-boolean-) | Sets whether a shape should be auto-fit to fully contain the text described within it. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Represents text rotation angle. |
| [setSeparatorType(int value)](#setSeparatorType-int-) | Sets the separator type used for the data labels on a chart. |
| [setSeparatorValue(String value)](#setSeparatorValue-java.lang.String-) | Sets the separator value used for the data labels on a chart. |
| [setShadow(boolean value)](#setShadow-boolean-) | True if the frame has a shadow. |
| [setShapeType(int value)](#setShapeType-int-) | Sets shape type of data label. |
| [setShowBubbleSize(boolean value)](#setShowBubbleSize-boolean-) | Represents a specified chart's data label percentage value display behavior. |
| [setShowCategoryName(boolean value)](#setShowCategoryName-boolean-) | Represents a specified chart's data label category name display behavior.True to display the category name for the data labels on a chart. |
| [setShowCellRange(boolean value)](#setShowCellRange-boolean-) | Indicates whether showing cell range as the data labels. |
| [setShowLegendKey(boolean value)](#setShowLegendKey-boolean-) | Represents a specified chart's data label legend key display behavior. |
| [setShowPercentage(boolean value)](#setShowPercentage-boolean-) | Represents a specified chart's data label percentage value display behavior. |
| [setShowSeriesName(boolean value)](#setShowSeriesName-boolean-) | Indicates whether the series name displays for the data labels on a chart. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Represents a specified chart's data label values display behavior. |
| [setText(String value)](#setText-java.lang.String-) | Sets the text of data label. |
| [setTextDirection(int value)](#setTextDirection-int-) | Represents text reading order. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Sets the text horizontal alignment. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Sets the text vertical alignment of text. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Sets a value indicating whether the text is wrapped. |
| [setWidth(int value)](#setWidth-int-) | Sets the width of frame in units of 1/4000 of the chart area. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Sets the width of frame in units of Pixel. |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | Sets the width of frame in units of ratio of the chart area. |
| [setX(int value)](#setX-int-) | Sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [setXPixel(int value)](#setXPixel-int-) | Sets the x coordinate of the upper left corner in units of Pixel. |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | Sets the x coordinate of the upper left corner in units of ratio of the chart area. |
| [setY(int value)](#setY-int-) | Sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [setYPixel(int value)](#setYPixel-int-) | Sets the y coordinate of the upper left corner in units of Pixel. |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | Sets the y coordinate of the upper left corner in units of ratio of the chart area. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyFont() {#applyFont--}
```
public void applyFont()
```


Apply the font of the datalabels to all child nodes.

### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Returns a Characters object that represents a range of characters within the text.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The index of the start of the character. |
| length | int | The number of characters. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
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
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


True if the text in the object changes font size when the object size changes. The default value is True.

**Returns:**
boolean
### getBackground() {#getBackground--}
```
public int getBackground()
```


Gets the display mode of the background

See [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOTE: This member is now obsolete. Instead, please use ChartFrame.BackgroundMode property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


Gets the display mode of the background

See [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Gets the [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getChart() {#getChart--}
```
public Chart getChart()
```


Gets the chart to which this object belongs.

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


Represents height of default position in units of 1/4000 of the chart area.

**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.DefaultHeightRatioToChart property, instead. DefaultHeight = (int)(DefaultHeightRatioToChart \* 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getDefaultHeightRatioToChart() {#getDefaultHeightRatioToChart--}
```
public double getDefaultHeightRatioToChart()
```


Represents height of default position in units of Fraction of the chart area.

**Returns:**
double
### getDefaultWidth() {#getDefaultWidth--}
```
public int getDefaultWidth()
```


Represents width of default position in units of 1/4000 of the chart area.

**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.DefaultWidthRatioToChart property, instead. DefaultWidth = (int)(DefaultWidthRatioToChart \* 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getDefaultWidthRatioToChart() {#getDefaultWidthRatioToChart--}
```
public double getDefaultWidthRatioToChart()
```


Represents width of default position in units of Fraction of the chart area.

**Returns:**
double
### getDefaultX() {#getDefaultX--}
```
public int getDefaultX()
```


Represents x of default position in units of 1/4000 of the chart area.

**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.DefaultXRatioToChart property, instead. DefaultX = (int)(DefaultXRatioToChart \* 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getDefaultXRatioToChart() {#getDefaultXRatioToChart--}
```
public double getDefaultXRatioToChart()
```


Represents x of default position in units of Fraction of the chart area.

**Returns:**
double
### getDefaultY() {#getDefaultY--}
```
public int getDefaultY()
```


Represents y of default position in units of 1/4000 of the chart area.

**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.DefaultYRatioToChart property, instead. DefaultY = (int)(DefaultYRatioToChart \* 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getDefaultYRatioToChart() {#getDefaultYRatioToChart--}
```
public double getDefaultYRatioToChart()
```


Represents y of default position in units of Fraction of the chart area.

**Returns:**
double
### getDirectionType() {#getDirectionType--}
```
public int getDirectionType()
```


Gets the direction of text.

See [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).

**Returns:**
int
### getFont() {#getFont--}
```
public Font getFont()
```


Gets the font of the DataLabels;

**Returns:**
[Font](../../com.aspose.cells/font)
### getHeight() {#getHeight--}
```
public int getHeight()
```


Gets the height of frame in units of 1/4000 of the chart area.

**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.HeightRatioToChart property, instead. Height = HeightRatioToChart \* 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Gets the height of frame in units of Pixel.

**Returns:**
int
### getHeightRatioToChart() {#getHeightRatioToChart--}
```
public double getHeightRatioToChart()
```


Gets the height of frame in units of ratio of the chart area.

**Remarks**

This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? HeightPixel = HeightRatioToChart \* Chart.ChartObject.Height;

**Returns:**
double
### getLinkedSource() {#getLinkedSource--}
```
public String getLinkedSource()
```


Gets a reference to the worksheet.

**Returns:**
java.lang.String
### getNumber() {#getNumber--}
```
public int getNumber()
```


Gets the built-in number format.

**Returns:**
int
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


Represents the format string for the DataLabels object.

**Returns:**
java.lang.String
### getNumberFormatLinked() {#getNumberFormatLinked--}
```
public boolean getNumberFormatLinked()
```


True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells).

**Returns:**
boolean
### getPosition() {#getPosition--}
```
public int getPosition()
```


Represents the position of the data label.

See [LabelPositionType](../../com.aspose.cells/labelpositiontype).

**Returns:**
int
### getReadingOrder() {#getReadingOrder--}
```
public int getReadingOrder()
```


Represents text reading order.

See [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Represents text rotation angle.

**Remarks**


0: Not rotated.

255: Top to Bottom.

\-90: Downward.

90: Upward.


**Returns:**
int
### getSeparatorType() {#getSeparatorType--}
```
public int getSeparatorType()
```


Gets the separator type used for the data labels on a chart.

See [DataLabelsSeparatorType](../../com.aspose.cells/datalabelsseparatortype).

**Remarks**

To set custom separator, please set the property [getSeparatorType()](../../com.aspose.cells/datalabels\#getSeparatorType--) as [DataLabelsSeparatorType.CUSTOM](../../com.aspose.cells/datalabelsseparatortype\#CUSTOM) and then specify the expected value for [getSeparatorValue()](../../com.aspose.cells/datalabels\#getSeparatorValue--).

**Returns:**
int
### getSeparatorValue() {#getSeparatorValue--}
```
public String getSeparatorValue()
```


Gets the separator value used for the data labels on a chart.

**Returns:**
java.lang.String
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


True if the frame has a shadow.

**Returns:**
boolean
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Gets the [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--) object.

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShapeType() {#getShapeType--}
```
public int getShapeType()
```


Gets shape type of data label.

See [DataLabelShapeType](../../com.aspose.cells/datalabelshapetype).

**Returns:**
int
### getShowBubbleSize() {#getShowBubbleSize--}
```
public boolean getShowBubbleSize()
```


Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide.

**Returns:**
boolean
### getShowCategoryName() {#getShowCategoryName--}
```
public boolean getShowCategoryName()
```


Represents a specified chart's data label category name display behavior.True to display the category name for the data labels on a chart. False to hide.

**Returns:**
boolean
### getShowCellRange() {#getShowCellRange--}
```
public boolean getShowCellRange()
```


Indicates whether showing cell range as the data labels.

**Returns:**
boolean
### getShowLegendKey() {#getShowLegendKey--}
```
public boolean getShowLegendKey()
```


Represents a specified chart's data label legend key display behavior. True if the data label legend key is visible.

**Returns:**
boolean
### getShowPercentage() {#getShowPercentage--}
```
public boolean getShowPercentage()
```


Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide.

**Returns:**
boolean
### getShowSeriesName() {#getShowSeriesName--}
```
public boolean getShowSeriesName()
```


Indicates whether the series name displays for the data labels on a chart. True to show the series name. False to hide.

**Returns:**
boolean
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


Represents a specified chart's data label values display behavior. True displays the values. False to hide.

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


Gets the text of data label.

**Returns:**
java.lang.String
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Represents text reading order.

See [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Remarks**

NOTE: This member is now obsolete. Instead, please use ChartTextFrame.ReadingOrder property. This property will be removed 12 months later since March 2020. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getTextFont() {#getTextFont--}
```
public Font getTextFont()
```


Gets a [ChartArea.getFont()](../../com.aspose.cells/chartarea\#getFont--) object of the specified ChartFrame object.

**Remarks**

NOTE: This member is now obsolete. Instead, please use ChartFrame.Font property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
[Font](../../com.aspose.cells/font)
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```
public int getTextHorizontalAlignment()
```


Gets the text horizontal alignment.

See [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Gets the options of the text.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getTextVerticalAlignment() {#getTextVerticalAlignment--}
```
public int getTextVerticalAlignment()
```


Gets the text vertical alignment of text.

See [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Gets the width of frame in units of 1/4000 of the chart area.

**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.WidthRatioToChart property, instead. Width = WidthRatioToChart \* 4000; This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Gets the width of frame in units of Pixel.

**Returns:**
int
### getWidthRatioToChart() {#getWidthRatioToChart--}
```
public double getWidthRatioToChart()
```


Gets the width of frame in units of ratio of the chart area.

**Remarks**

This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? WidthPixel = WidthRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### getX() {#getX--}
```
public int getX()
```


Gets the x coordinate of the upper left corner in units of 1/4000 of the chart area.

**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.XRatioToChart property, instead. X = XRatioToChart \* 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getXPixel() {#getXPixel--}
```
public int getXPixel()
```


Gets the x coordinate of the upper left corner in units of Pixel.

**Returns:**
int
### getXRatioToChart() {#getXRatioToChart--}
```
public double getXRatioToChart()
```


Gets the x coordinate of the upper left corner in units of ratio of the chart area.

**Remarks**

This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? XPixel = XRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


Gets the y coordinate of the upper left corner in units of 1/4000 of the chart area.

**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.YRatioToChart property, instead. Y = YRatioToChart \* 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getYPixel() {#getYPixel--}
```
public int getYPixel()
```


Gets the y coordinate of the upper left corner in units of Pixel.

**Returns:**
int
### getYRatioToChart() {#getYRatioToChart--}
```
public double getYRatioToChart()
```


Gets the y coordinate of the upper left corner in units of ratio of the chart area.

**Remarks**

This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? YPixel = YRatioToChart \* Chart.ChartObject.Height;

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


Indicates the text is auto generated.

**Returns:**
boolean
### isAutomaticRotation() {#isAutomaticRotation--}
```
public boolean isAutomaticRotation()
```


Indicates whether the text of the chart is automatically rotated.

**Returns:**
boolean
### isAutomaticSize() {#isAutomaticSize--}
```
public boolean isAutomaticSize()
```


Indicates whether the chart frame is automatic sized.

**Returns:**
boolean
### isDefaultPosBeSet() {#isDefaultPosBeSet--}
```
public boolean isDefaultPosBeSet()
```


Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set.

**Returns:**
boolean
### isDeleted() {#isDeleted--}
```
public boolean isDeleted()
```


Indicates whether this data labels is deleted.

**Returns:**
boolean
### isInnerMode() {#isInnerMode--}
```
public boolean isInnerMode()
```


Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels.

**Remarks**

Only for Xlsx file.

**Returns:**
boolean
### isNeverOverlap() {#isNeverOverlap--}
```
public boolean isNeverOverlap()
```


Indicates whether the datalabels display never overlap. (For Pie chart)

**Returns:**
boolean
### isResizeShapeToFitText() {#isResizeShapeToFitText--}
```
public boolean isResizeShapeToFitText()
```


Gets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Gets a value indicating whether the text is wrapped.

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


True if the text in the object changes font size when the object size changes. The default value is True.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoText(boolean value) {#setAutoText-boolean-}
```
public void setAutoText(boolean value)
```


Indicates the text is auto generated.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutomaticSize(boolean value) {#setAutomaticSize-boolean-}
```
public void setAutomaticSize(boolean value)
```


Indicates whether the chart frame is automatic sized.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setBackground(int value) {#setBackground-int-}
```
public void setBackground(int value)
```


Sets the display mode of the background

See [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOTE: This member is now obsolete. Instead, please use ChartFrame.BackgroundMode property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


Sets the display mode of the background

See [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDeleted(boolean value) {#setDeleted-boolean-}
```
public void setDeleted(boolean value)
```


Indicates whether this data labels is deleted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDirectionType(int value) {#setDirectionType-int-}
```
public void setDirectionType(int value)
```


Sets the direction of text.

See [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Sets the height of frame in units of 1/4000 of the chart area.

**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.HeightRatioToChart property, instead. Height = HeightRatioToChart \* 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Sets the height of frame in units of Pixel.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHeightRatioToChart(double value) {#setHeightRatioToChart-double-}
```
public void setHeightRatioToChart(double value)
```


Sets the height of frame in units of ratio of the chart area.

**Remarks**

This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? HeightPixel = HeightRatioToChart \* Chart.ChartObject.Height;

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setInnerMode(boolean value) {#setInnerMode-boolean-}
```
public void setInnerMode(boolean value)
```


Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels.

**Remarks**

Only for Xlsx file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLinkedSource(String value) {#setLinkedSource-java.lang.String-}
```
public void setLinkedSource(String value)
```


Sets a reference to the worksheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setNeverOverlap(boolean value) {#setNeverOverlap-boolean-}
```
public void setNeverOverlap(boolean value)
```


Indicates whether the datalabels display never overlap. (For Pie chart)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Sets the built-in number format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


Represents the format string for the DataLabels object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setNumberFormatLinked(boolean value) {#setNumberFormatLinked-boolean-}
```
public void setNumberFormatLinked(boolean value)
```


True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Represents the position of the data label.

See [LabelPositionType](../../com.aspose.cells/labelpositiontype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPositionAuto() {#setPositionAuto--}
```
public void setPositionAuto()
```


Set position of the frame to automatic

### setReadingOrder(int value) {#setReadingOrder-int-}
```
public void setReadingOrder(int value)
```


Represents text reading order.

See [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setResizeShapeToFitText(boolean value) {#setResizeShapeToFitText-boolean-}
```
public void setResizeShapeToFitText(boolean value)
```


Sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Represents text rotation angle.

**Remarks**


0: Not rotated.

255: Top to Bottom.

\-90: Downward.

90: Upward.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSeparatorType(int value) {#setSeparatorType-int-}
```
public void setSeparatorType(int value)
```


Sets the separator type used for the data labels on a chart.

See [DataLabelsSeparatorType](../../com.aspose.cells/datalabelsseparatortype).

**Remarks**

To set custom separator, please set the property [getSeparatorType()](../../com.aspose.cells/datalabels\#getSeparatorType--) as [DataLabelsSeparatorType.CUSTOM](../../com.aspose.cells/datalabelsseparatortype\#CUSTOM) and then specify the expected value for [getSeparatorValue()](../../com.aspose.cells/datalabels\#getSeparatorValue--).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSeparatorValue(String value) {#setSeparatorValue-java.lang.String-}
```
public void setSeparatorValue(String value)
```


Sets the separator value used for the data labels on a chart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


True if the frame has a shadow.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShapeType(int value) {#setShapeType-int-}
```
public void setShapeType(int value)
```


Sets shape type of data label.

See [DataLabelShapeType](../../com.aspose.cells/datalabelshapetype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setShowBubbleSize(boolean value) {#setShowBubbleSize-boolean-}
```
public void setShowBubbleSize(boolean value)
```


Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowCategoryName(boolean value) {#setShowCategoryName-boolean-}
```
public void setShowCategoryName(boolean value)
```


Represents a specified chart's data label category name display behavior.True to display the category name for the data labels on a chart. False to hide.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowCellRange(boolean value) {#setShowCellRange-boolean-}
```
public void setShowCellRange(boolean value)
```


Indicates whether showing cell range as the data labels.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowLegendKey(boolean value) {#setShowLegendKey-boolean-}
```
public void setShowLegendKey(boolean value)
```


Represents a specified chart's data label legend key display behavior. True if the data label legend key is visible.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowPercentage(boolean value) {#setShowPercentage-boolean-}
```
public void setShowPercentage(boolean value)
```


Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowSeriesName(boolean value) {#setShowSeriesName-boolean-}
```
public void setShowSeriesName(boolean value)
```


Indicates whether the series name displays for the data labels on a chart. True to show the series name. False to hide.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


Represents a specified chart's data label values display behavior. True displays the values. False to hide.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Sets the text of data label.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Represents text reading order.

See [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Remarks**

NOTE: This member is now obsolete. Instead, please use ChartTextFrame.ReadingOrder property. This property will be removed 12 months later since March 2020. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Sets the text horizontal alignment.

See [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Sets the text vertical alignment of text.

See [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Sets a value indicating whether the text is wrapped.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Sets the width of frame in units of 1/4000 of the chart area.

**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.WidthRatioToChart property, instead. Width = WidthRatioToChart \* 4000; This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Sets the width of frame in units of Pixel.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setWidthRatioToChart(double value) {#setWidthRatioToChart-double-}
```
public void setWidthRatioToChart(double value)
```


Sets the width of frame in units of ratio of the chart area.

**Remarks**

This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? WidthPixel = WidthRatioToChart \* Chart.ChartObject.Width;

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Sets the x coordinate of the upper left corner in units of 1/4000 of the chart area.

**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.XRatioToChart property, instead. X = XRatioToChart \* 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setXPixel(int value) {#setXPixel-int-}
```
public void setXPixel(int value)
```


Sets the x coordinate of the upper left corner in units of Pixel.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setXRatioToChart(double value) {#setXRatioToChart-double-}
```
public void setXRatioToChart(double value)
```


Sets the x coordinate of the upper left corner in units of ratio of the chart area.

**Remarks**

This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? XPixel = XRatioToChart \* Chart.ChartObject.Width;

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Sets the y coordinate of the upper left corner in units of 1/4000 of the chart area.

**Remarks**

NOTE: This member is now obsolete. Please use ChartFrame.YRatioToChart property, instead. Y = YRatioToChart \* 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setYPixel(int value) {#setYPixel-int-}
```
public void setYPixel(int value)
```


Sets the y coordinate of the upper left corner in units of Pixel.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setYRatioToChart(double value) {#setYRatioToChart-double-}
```
public void setYRatioToChart(double value)
```


Sets the y coordinate of the upper left corner in units of ratio of the chart area.

**Remarks**

This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? YPixel = YRatioToChart \* Chart.ChartObject.Height;

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

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

