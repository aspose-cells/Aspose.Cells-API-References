---
title: Legend
second_title: Aspose.Cells for Java API Reference
description: Encapsulates the object that represents the chart legend.
type: docs
url: /java/com.aspose.cells/legend/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe), [com.aspose.cells.ChartTextFrame](../../com.aspose.cells/charttextframe)
```
public class Legend extends ChartTextFrame
```

Encapsulates the object that represents the chart legend.

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
## Methods

| Method | Description |
| --- | --- |
| [characters(int startIndex, int length)](#characters-int-int-) | Returns a Characters object that represents a range of characters within the text. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Gets the [Area](../../com.aspose.cells/area). |
| [getAutoScaleFont()](#getAutoScaleFont--) | True if the text in the object changes font size when the object size changes. |
| [getBackground()](#getBackground--) | Gets the display mode of the background NOTE: This member is now obsolete. |
| [getBackgroundMode()](#getBackgroundMode--) | Gets the display mode of the background |
| [getBorder()](#getBorder--) | Gets the [Line](../../com.aspose.cells/line). |
| [getChart()](#getChart--) | Gets the chart to which this object belongs. |
| [getClass()](#getClass--) |  |
| [getDefaultHeight()](#getDefaultHeight--) | Represents height of default position |
| [getDefaultWidth()](#getDefaultWidth--) | Represents width of default position |
| [getDefaultX()](#getDefaultX--) | Represents x of default position |
| [getDefaultY()](#getDefaultY--) | Represents y of default position |
| [getDirectionType()](#getDirectionType--) | Gets the direction of text. |
| [getFont()](#getFont--) | Gets a [ChartArea.getFont()](../../com.aspose.cells/chartarea\#getFont--) object of the specified ChartFrame object. |
| [getHeight()](#getHeight--) | Gets the height of frame in units of 1/4000 of the chart area. |
| [getLegendEntries()](#getLegendEntries--) | Gets a collection of all the LegendEntry objects in the specified chart legend. |
| [getLegendEntriesLabels()](#getLegendEntriesLabels--) | Gets the labels of the legend entries after call Chart.Calculate() method. |
| [getLinkedSource()](#getLinkedSource--) | Gets a reference to the worksheet. |
| [getPosition()](#getPosition--) | Gets the legend position type. |
| [getReadingOrder()](#getReadingOrder--) | Represents text reading order. |
| [getRotationAngle()](#getRotationAngle--) | Represents text rotation angle. |
| [getShadow()](#getShadow--) | True if the frame has a shadow. |
| [getShapeProperties()](#getShapeProperties--) | Gets the [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--) object. |
| [getText()](#getText--) | Gets the text of a frame's title. |
| [getTextDirection()](#getTextDirection--) | Represents text reading order. |
| [getTextFont()](#getTextFont--) | Gets a [ChartArea.getFont()](../../com.aspose.cells/chartarea\#getFont--) object of the specified ChartFrame object. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Gets the text horizontal alignment. |
| [getTextOptions()](#getTextOptions--) | Gets the options of the text. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Gets the text vertical alignment of text. |
| [getWidth()](#getWidth--) | Gets the width of frame in units of 1/4000 of the chart area. |
| [getX()](#getX--) | Gets the x coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [getY()](#getY--) | Gets the y coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [hashCode()](#hashCode--) |  |
| [isAutoText()](#isAutoText--) | Indicates the text is auto generated. |
| [isAutomaticRotation()](#isAutomaticRotation--) | Indicates whether the text of the chart is automatically rotated. |
| [isAutomaticSize()](#isAutomaticSize--) | Indicates whether the chart frame is automatic sized. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [isDeleted()](#isDeleted--) | Indicates whether this data labels is deleted. |
| [isInnerMode()](#isInnerMode--) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. |
| [isOverLay()](#isOverLay--) | Gets whether other chart elements shall be allowed to overlap this chart element. |
| [isResizeShapeToFitText()](#isResizeShapeToFitText--) | Gets whether a shape should be auto-fit to fully contain the text described within it. |
| [isTextWrapped()](#isTextWrapped--) | Gets a value indicating whether the text is wrapped. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | True if the text in the object changes font size when the object size changes. |
| [setAutoText(boolean value)](#setAutoText-boolean-) | Indicates the text is auto generated. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Indicates whether the chart frame is automatic sized. |
| [setBackground(int value)](#setBackground-int-) | Sets the display mode of the background NOTE: This member is now obsolete. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Sets the display mode of the background |
| [setDeleted(boolean value)](#setDeleted-boolean-) | Indicates whether this data labels is deleted. |
| [setDirectionType(int value)](#setDirectionType-int-) | Sets the direction of text. |
| [setHeight(int value)](#setHeight-int-) | Sets the height of frame in units of 1/4000 of the chart area. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. |
| [setLinkedSource(String value)](#setLinkedSource-java.lang.String-) | Sets a reference to the worksheet. |
| [setOverLay(boolean value)](#setOverLay-boolean-) | Sets whether other chart elements shall be allowed to overlap this chart element. |
| [setPosition(int value)](#setPosition-int-) | Sets the legend position type. |
| [setPositionAuto()](#setPositionAuto--) | Set position of the frame to automatic |
| [setReadingOrder(int value)](#setReadingOrder-int-) | Represents text reading order. |
| [setResizeShapeToFitText(boolean value)](#setResizeShapeToFitText-boolean-) | Sets whether a shape should be auto-fit to fully contain the text described within it. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Represents text rotation angle. |
| [setShadow(boolean value)](#setShadow-boolean-) | True if the frame has a shadow. |
| [setText(String value)](#setText-java.lang.String-) | Sets the text of a frame's title. |
| [setTextDirection(int value)](#setTextDirection-int-) | Represents text reading order. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Sets the text horizontal alignment. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Sets the text vertical alignment of text. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Sets a value indicating whether the text is wrapped. |
| [setWidth(int value)](#setWidth-int-) | Sets the width of frame in units of 1/4000 of the chart area. |
| [setX(int value)](#setX-int-) | Sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [setY(int value)](#setY-int-) | Sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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


Gets the display mode of the background NOTE: This member is now obsolete. Instead, please use ChartFrame.BackgroundMode property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


Gets the display mode of the background

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


Represents height of default position

**Returns:**
int
### getDefaultWidth() {#getDefaultWidth--}
```
public int getDefaultWidth()
```


Represents width of default position

**Returns:**
int
### getDefaultX() {#getDefaultX--}
```
public int getDefaultX()
```


Represents x of default position

**Returns:**
int
### getDefaultY() {#getDefaultY--}
```
public int getDefaultY()
```


Represents y of default position

**Returns:**
int
### getDirectionType() {#getDirectionType--}
```
public int getDirectionType()
```


Gets the direction of text.

**Returns:**
int
### getFont() {#getFont--}
```
public Font getFont()
```


Gets a [ChartArea.getFont()](../../com.aspose.cells/chartarea\#getFont--) object of the specified ChartFrame object.

**Returns:**
[Font](../../com.aspose.cells/font)
### getHeight() {#getHeight--}
```
public int getHeight()
```


Gets the height of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Height In Pixels = Y \* Chart.ChartObject.Height / 4000;

**Returns:**
int
### getLegendEntries() {#getLegendEntries--}
```
public LegendEntryCollection getLegendEntries()
```


Gets a collection of all the LegendEntry objects in the specified chart legend. Setting the legend entries of the surface chart is not supported. So it will return null if the chart type is surface chart type.

**Returns:**
[LegendEntryCollection](../../com.aspose.cells/legendentrycollection)
### getLegendEntriesLabels() {#getLegendEntriesLabels--}
```
public ArrayList getLegendEntriesLabels()
```


Gets the labels of the legend entries after call Chart.Calculate() method.

**Returns:**
java.util.ArrayList
### getLinkedSource() {#getLinkedSource--}
```
public String getLinkedSource()
```


Gets a reference to the worksheet.

**Returns:**
java.lang.String
### getPosition() {#getPosition--}
```
public int getPosition()
```


Gets the legend position type.
Default position is right.

If the legend is at left or right side of the chart, setting Legend.X property will not take effect.

If the legend is at top or bottom side of the chart, setting Legend.Y property will not take effect.


**Returns:**
int
### getReadingOrder() {#getReadingOrder--}
```
public int getReadingOrder()
```


Represents text reading order.

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Represents text rotation angle.
0: Not rotated.

255: Top to Bottom.

\-90: Downward.

90: Upward.


**Returns:**
int
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
### getText() {#getText--}
```
public String getText()
```


Gets the text of a frame's title.

**Returns:**
java.lang.String
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Represents text reading order. NOTE: This member is now obsolete. Instead, please use ChartTextFrame.ReadingOrder property. This property will be removed 12 months later since March 2020. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getTextFont() {#getTextFont--}
```
public Font getTextFont()
```


Gets a [ChartArea.getFont()](../../com.aspose.cells/chartarea\#getFont--) object of the specified ChartFrame object. NOTE: This member is now obsolete. Instead, please use ChartFrame.Font property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
[Font](../../com.aspose.cells/font)
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```
public int getTextHorizontalAlignment()
```


Gets the text horizontal alignment.

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

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Gets the width of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Width In Pixels = Width \* Chart.ChartObject.Height / 4000;

**Returns:**
int
### getX() {#getX--}
```
public int getX()
```


Gets the x coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? X In Pixels = X \* Chart.ChartObject.Width / 4000;

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


Gets the y coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Y In Pixels = Y \* Chart.ChartObject.Height / 4000;

**Returns:**
int
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


Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. Only for Xlsx file.

**Returns:**
boolean
### isOverLay() {#isOverLay--}
```
public boolean isOverLay()
```


Gets whether other chart elements shall be allowed to overlap this chart element.

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


Sets the display mode of the background NOTE: This member is now obsolete. Instead, please use ChartFrame.BackgroundMode property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


Sets the display mode of the background

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

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Sets the height of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Height In Pixels = Y \* Chart.ChartObject.Height / 4000;

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setInnerMode(boolean value) {#setInnerMode-boolean-}
```
public void setInnerMode(boolean value)
```


Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. Only for Xlsx file.

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

### setOverLay(boolean value) {#setOverLay-boolean-}
```
public void setOverLay(boolean value)
```


Sets whether other chart elements shall be allowed to overlap this chart element.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Sets the legend position type.
Default position is right.

If the legend is at left or right side of the chart, setting Legend.X property will not take effect.

If the legend is at top or bottom side of the chart, setting Legend.Y property will not take effect.


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
0: Not rotated.

255: Top to Bottom.

\-90: Downward.

90: Upward.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


True if the frame has a shadow.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Sets the text of a frame's title.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Represents text reading order. NOTE: This member is now obsolete. Instead, please use ChartTextFrame.ReadingOrder property. This property will be removed 12 months later since March 2020. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Sets the text horizontal alignment.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Sets the text vertical alignment of text.

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


Sets the width of frame in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Width In Pixels = Width \* Chart.ChartObject.Height / 4000;

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? X In Pixels = X \* Chart.ChartObject.Width / 4000;

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. How to convert units of 1/4000 to pixels? Y In Pixels = Y \* Chart.ChartObject.Height / 4000;

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

