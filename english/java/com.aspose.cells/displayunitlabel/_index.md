---
title: DisplayUnitLabel
second_title: Aspose.Cells for Java API Reference
description: Represents the display unit label.
type: docs
url: /java/com.aspose.cells/displayunitlabel/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe), [com.aspose.cells.ChartTextFrame](../../com.aspose.cells/charttextframe)
```
public class DisplayUnitLabel extends ChartTextFrame
```

Represents the display unit label.

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
         //Setting the display unit of value(Y) axis.
         chart.getValueAxis().setDisplayUnit(DisplayUnitType.HUNDREDS);
         DisplayUnitLabel displayUnitLabel = chart.getValueAxis().getDisplayUnitLabel();
         //Setting the custom display unit label
         displayUnitLabel.setText("100");
         //Saving the Excel file
         workbook.save("book1.xls");
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
| [getLinkedSource()](#getLinkedSource--) | Gets a reference to the worksheet. |
| [getReadingOrder()](#getReadingOrder--) | Represents text reading order. |
| [getRotationAngle()](#getRotationAngle--) | Represents text rotation angle. |
| [getShadow()](#getShadow--) | True if the frame has a shadow. |
| [getShapeProperties()](#getShapeProperties--) | Gets the [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--) object. |
| [getText()](#getText--) | Gets the text of display unit label. |
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
| [isAutomaticSize()](#isAutomaticSize--) | Indicates whether the chart frame is automatic sized. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [isDeleted()](#isDeleted--) | Indicates whether this data labels is deleted. |
| [isInnerMode()](#isInnerMode--) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. |
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
| [setPositionAuto()](#setPositionAuto--) | Set position of the frame to automatic |
| [setReadingOrder(int value)](#setReadingOrder-int-) | Represents text reading order. |
| [setResizeShapeToFitText(boolean value)](#setResizeShapeToFitText-boolean-) | Sets whether a shape should be auto-fit to fully contain the text described within it. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Represents text rotation angle. |
| [setShadow(boolean value)](#setShadow-boolean-) | True if the frame has a shadow. |
| [setText(String value)](#setText-java.lang.String-) | Sets the text of display unit label. |
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
### getLinkedSource() {#getLinkedSource--}
```
public String getLinkedSource()
```


Gets a reference to the worksheet.

**Returns:**
java.lang.String
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


Gets the text of display unit label.

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


Sets the text of display unit label.

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

