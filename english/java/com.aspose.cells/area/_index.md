---
title: Area
second_title: Aspose.Cells for Java API Reference
description: Encapsulates the object that represents an area format.
type: docs
url: /java/com.aspose.cells/area/
---

**Inheritance:**
java.lang.Object
```
public class Area
```

Encapsulates the object that represents an area format.

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Workbook object
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
         //Setting the foreground color of the plot area
         chart.getPlotArea().getArea().setForegroundColor(Color.getBlue());
         //Setting the foreground color of the chart area
         chart.getChartArea().getArea().setForegroundColor(Color.getYellow());
         //Setting the foreground color of the 1st NSeries area
         chart.getNSeries().get(0).getArea().setForegroundColor(Color.getRed());
         //Setting the foreground color of the area of the 1st NSeries point
         chart.getNSeries().get(0).getPoints().get(0).getArea().setForegroundColor(Color.getCyan());
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundColor()](#getBackgroundColor--) | the background [Color](../../com.aspose.cells/color) of the [Area](../../com.aspose.cells/area). |
| [getClass()](#getClass--) |  |
| [getFillFormat()](#getFillFormat--) | Represents a [getFillFormat()](../../com.aspose.cells/area\#getFillFormat--) object that contains fill formatting properties for the specified chart or shape. |
| [getForegroundColor()](#getForegroundColor--) | the foreground [Color](../../com.aspose.cells/color). |
| [getFormatting()](#getFormatting--) | Represents the formatting of the area. |
| [getInvertIfNegative()](#getInvertIfNegative--) | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [getTransparency()](#getTransparency--) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Indicates Microsoft Workbook automatically determines the area pattern. |
| [isVisible()](#isVisible--) | Indicates whether the area is visible in the chart. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuto(boolean isAuto)](#setAuto-boolean-) | Sets whether Microsoft Workbook automatically determines the area pattern. |
| [setBackgroundColor(Color value)](#setBackgroundColor-com.aspose.cells.Color-) | For the description of this property, please see [getBackgroundColor()](../../com.aspose.cells/area\#getBackgroundColor--) |
| [setForegroundColor(Color value)](#setForegroundColor-com.aspose.cells.Color-) | For the description of this property, please see [getForegroundColor()](../../com.aspose.cells/area\#getForegroundColor--) |
| [setFormatting(int value)](#setFormatting-int-) | For the description of this property, please see [getFormatting()](../../com.aspose.cells/area\#getFormatting--) |
| [setInvertIfNegative(boolean value)](#setInvertIfNegative-boolean-) | For the description of this property, please see [getInvertIfNegative()](../../com.aspose.cells/area\#getInvertIfNegative--) |
| [setTransparency(double value)](#setTransparency-double-) | For the description of this property, please see [getTransparency()](../../com.aspose.cells/area\#getTransparency--) |
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
### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


the background [Color](../../com.aspose.cells/color) of the [Area](../../com.aspose.cells/area).

**Returns:**
[Color](../../com.aspose.cells/color)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFillFormat() {#getFillFormat--}
```
public FillFormat getFillFormat()
```


Represents a [getFillFormat()](../../com.aspose.cells/area\#getFillFormat--) object that contains fill formatting properties for the specified chart or shape.

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getForegroundColor() {#getForegroundColor--}
```
public Color getForegroundColor()
```


the foreground [Color](../../com.aspose.cells/color).

**Returns:**
[Color](../../com.aspose.cells/color)
### getFormatting() {#getFormatting--}
```
public int getFormatting()
```


Represents the formatting of the area.

**Returns:**
int
### getInvertIfNegative() {#getInvertIfNegative--}
```
public boolean getInvertIfNegative()
```


If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Workbook object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(-100);
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "A3"
         chart.getNSeries().add("A1:A3", true);
         chart.getNSeries().get(0).getArea().setInvertIfNegative(true);
         //Setting the foreground color of the 1st NSeries area
         chart.getNSeries().get(0).getArea().setForegroundColor(Color.getRed());
         //Setting the background color of the 1st NSeries area.
         //The displayed area color of second chart point will be the background color.
         chart.getNSeries().get(0).getArea().setBackgroundColor(Color.getYellow());
         //Saving the Excel file
         workbook.save("book1.xls");
```

**Returns:**
boolean
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

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


Indicates Microsoft Workbook automatically determines the area pattern.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Indicates whether the area is visible in the chart.

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




### setAuto(boolean isAuto) {#setAuto-boolean-}
```
public void setAuto(boolean isAuto)
```


Sets whether Microsoft Workbook automatically determines the area pattern.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isAuto | boolean | isAuto whether Microsoft Workbook automatically determines the area pattern. |

### setBackgroundColor(Color value) {#setBackgroundColor-com.aspose.cells.Color-}
```
public void setBackgroundColor(Color value)
```


For the description of this property, please see [getBackgroundColor()](../../com.aspose.cells/area\#getBackgroundColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForegroundColor(Color value) {#setForegroundColor-com.aspose.cells.Color-}
```
public void setForegroundColor(Color value)
```


For the description of this property, please see [getForegroundColor()](../../com.aspose.cells/area\#getForegroundColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setFormatting(int value) {#setFormatting-int-}
```
public void setFormatting(int value)
```


For the description of this property, please see [getFormatting()](../../com.aspose.cells/area\#getFormatting--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setInvertIfNegative(boolean value) {#setInvertIfNegative-boolean-}
```
public void setInvertIfNegative(boolean value)
```


For the description of this property, please see [getInvertIfNegative()](../../com.aspose.cells/area\#getInvertIfNegative--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


For the description of this property, please see [getTransparency()](../../com.aspose.cells/area\#getTransparency--)

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

