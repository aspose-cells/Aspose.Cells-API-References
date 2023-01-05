---
title: ChartArea
second_title: Aspose.Cells for Java API Reference
description: Encapsulates the object that represents the chart area in the worksheet.
type: docs
url: /java/com.aspose.cells/chartarea/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe)
```
public class ChartArea extends ChartFrame
```

Encapsulates the object that represents the chart area in the worksheet.

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
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
 
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
 
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
 
         //Getting Chart Area
         ChartArea chartArea = chart.getChartArea();
 
         //Setting the foreground color of the chart area
         chartArea.getArea().setForegroundColor(Color.getYellow());
 
         //Setting Chart Area Shadow
         chartArea.setShadow(true);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Methods

| Method | Description |
| --- | --- |
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
| [getFont()](#getFont--) | Gets a [getFont()](../../com.aspose.cells/chartarea\#getFont--) object of the specified chartarea object. |
| [getHeight()](#getHeight--) | Gets the vertical offset from its lower right corner row. |
| [getShadow()](#getShadow--) | True if the frame has a shadow. |
| [getShapeProperties()](#getShapeProperties--) | Gets the [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--) object. |
| [getTextFont()](#getTextFont--) | Gets a [ChartArea.getFont()](../../com.aspose.cells/chartarea\#getFont--) object of the specified ChartFrame object. |
| [getTextOptions()](#getTextOptions--) | Gets the options of the text. |
| [getWidth()](#getWidth--) | Gets the horizontal offset from its lower right corner column. |
| [getX()](#getX--) | Gets or gets the horizontal offset from its upper left corner column. |
| [getY()](#getY--) | Gets or gets the vertical offset from its upper left corner row. |
| [hashCode()](#hashCode--) |  |
| [isAutomaticSize()](#isAutomaticSize--) | Indicates whether the chart frame is automatic sized. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [isInnerMode()](#isInnerMode--) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | True if the text in the object changes font size when the object size changes. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Indicates whether the chart frame is automatic sized. |
| [setBackground(int value)](#setBackground-int-) | Sets the display mode of the background NOTE: This member is now obsolete. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Sets the display mode of the background |
| [setHeight(int value)](#setHeight-int-) | Sets the vertical offset from its lower right corner row. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. |
| [setPositionAuto()](#setPositionAuto--) | Set position of the frame to automatic |
| [setShadow(boolean value)](#setShadow-boolean-) | True if the frame has a shadow. |
| [setWidth(int value)](#setWidth-int-) | Sets the horizontal offset from its lower right corner column. |
| [setX(int value)](#setX-int-) | Gets or gets the horizontal offset from its upper left corner column. |
| [setY(int value)](#setY-int-) | Gets or gets the vertical offset from its upper left corner row. |
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
### getFont() {#getFont--}
```
public Font getFont()
```


Gets a [getFont()](../../com.aspose.cells/chartarea\#getFont--) object of the specified chartarea object.

**Returns:**
[Font](../../com.aspose.cells/font)
### getHeight() {#getHeight--}
```
public int getHeight()
```


Gets the vertical offset from its lower right corner row.

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
### getTextFont() {#getTextFont--}
```
public Font getTextFont()
```


Gets a [ChartArea.getFont()](../../com.aspose.cells/chartarea\#getFont--) object of the specified ChartFrame object. NOTE: This member is now obsolete. Instead, please use ChartFrame.Font property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
[Font](../../com.aspose.cells/font)
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Gets the options of the text.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getWidth() {#getWidth--}
```
public int getWidth()
```


Gets the horizontal offset from its lower right corner column.

**Returns:**
int
### getX() {#getX--}
```
public int getX()
```


Gets or gets the horizontal offset from its upper left corner column.

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


Gets or gets the vertical offset from its upper left corner row.

**Returns:**
int
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
### isInnerMode() {#isInnerMode--}
```
public boolean isInnerMode()
```


Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. Only for Xlsx file.

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

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Sets the vertical offset from its lower right corner row.

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

### setPositionAuto() {#setPositionAuto--}
```
public void setPositionAuto()
```


Set position of the frame to automatic

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


True if the frame has a shadow.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Sets the horizontal offset from its lower right corner column.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Gets or gets the horizontal offset from its upper left corner column.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Gets or gets the vertical offset from its upper left corner row.

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

