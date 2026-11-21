---
title: "Floor"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar objektet som representerar golvet i ett 3‑D‑diagram."
type: docs
url: /sv/java/com.aspose.cells/floor/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Area](../../com.aspose.cells/area)
```
public class Floor extends Area
```

Inkapslar objektet som representerar golvet i ett 3‑D‑diagram.

**Example**

```
         //Instantiate the License class
         License license = new License();
 
         //Pass only the name of the license file embedded in the assembly
         license.setLicense("Aspose.Cells.lic");
 
         //Instantiate the workbook object
         Workbook workbook = new Workbook();
 
         //Get cells collection
         Cells cells = workbook.getWorksheets().get(0).getCells();
 
         //Put values in cells
         cells.get("A1").putValue(1);
 
         cells.get("A2").putValue(2);
 
         cells.get("A3").putValue(3);
 
         //get charts colletion
         ChartCollection charts = workbook.getWorksheets().get(0).getCharts();
 
         //add a new chart 
         int index = charts.add(ChartType.COLUMN_3_D_STACKED, 5, 0, 15, 5);
 
         //get the newly added chart
         Chart chart = charts.get(index);
 
         //set charts nseries
         chart.getNSeries().add("A1:A3", true);
 
         //Show data labels
         chart.getNSeries().get(0).getDataLabels().setShowValue(true);
 
         //Get chart's floor
         Floor floor = chart.getFloor();
 
         //set floor's border as red
         floor.getBorder().setColor(com.aspose.cells.Color.getRed());
 
         //set fill format
         floor.getFillFormat().setPresetColorGradient(GradientPresetType.CALM_WATER, GradientStyleType.DIAGONAL_DOWN, 2); 
 
         //save the file
         workbook.save("dest.xls");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundColor()](#getBackgroundColor--) | Hämtar bakgrundens [Color](../../com.aspose.cells/color) för [Area](../../com.aspose.cells/area). |
| [getBorder()](#getBorder--) | Hämtar kantens [Line](../../com.aspose.cells/line). |
| [getClass()](#getClass--) |  |
| [getFillFormat()](#getFillFormat--) | Representerar ett [getFillFormat()](../../com.aspose.cells/area\#getFillFormat--) objekt som innehåller fyllningsformaterings‑egenskaper för det angivna diagrammet eller formen. |
| [getForegroundColor()](#getForegroundColor--) | Hämtar förgrundens [Color](../../com.aspose.cells/color). |
| [getFormatting()](#getFormatting--) | Representerar formateringen av området. |
| [getInvertIfNegative()](#getInvertIfNegative--) | Om egenskapen är sann och värdet för diagrampunkten är ett negativt tal, kommer förgrundsfärgen och bakgrundsfärgen att bytas. |
| [getTransparency()](#getTransparency--) | Returnerar eller anger graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (klar). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundColor(Color value)](#setBackgroundColor-com.aspose.cells.Color-) | Ställer in bakgrundens [Color](../../com.aspose.cells/color) för [Area](../../com.aspose.cells/area). |
| [setBorder(Line value)](#setBorder-com.aspose.cells.Line-) | Ställer in kanten [Line](../../com.aspose.cells/line). |
| [setForegroundColor(Color value)](#setForegroundColor-com.aspose.cells.Color-) | Ställer in förgrundens [Color](../../com.aspose.cells/color). |
| [setFormatting(int value)](#setFormatting-int-) | Representerar formateringen av området. |
| [setInvertIfNegative(boolean value)](#setInvertIfNegative-boolean-) | Om egenskapen är sann och värdet för diagrampunkten är ett negativt tal, kommer förgrundsfärgen och bakgrundsfärgen att bytas. |
| [setTransparency(double value)](#setTransparency-double-) | Returnerar eller anger graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (klar). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


Hämtar bakgrundens [Color](../../com.aspose.cells/color) för [Area](../../com.aspose.cells/area).

**Returns:**
[Color](../../com.aspose.cells/color)
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Hämtar kantens [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
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


Representerar ett [getFillFormat()](../../com.aspose.cells/area\#getFillFormat--) objekt som innehåller fyllningsformaterings‑egenskaper för det angivna diagrammet eller formen.

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getForegroundColor() {#getForegroundColor--}
```
public Color getForegroundColor()
```


Hämtar förgrundens [Color](../../com.aspose.cells/color).

**Returns:**
[Color](../../com.aspose.cells/color)
### getFormatting() {#getFormatting--}
```
public int getFormatting()
```


Representerar formateringen av området.

Se [FormattingType](../../com.aspose.cells/formattingtype).

**Returns:**
int
### getInvertIfNegative() {#getInvertIfNegative--}
```
public boolean getInvertIfNegative()
```


Om egenskapen är sann och värdet för diagrampunkten är ett negativt tal, kommer förgrundsfärgen och bakgrundsfärgen att bytas.

**Example**

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
         boolean isNegative = chart.getNSeries().get(0).getArea().getInvertIfNegative();
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


Returnerar eller anger graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (klar).

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBackgroundColor(Color value) {#setBackgroundColor-com.aspose.cells.Color-}
```
public void setBackgroundColor(Color value)
```


Ställer in bakgrundens [Color](../../com.aspose.cells/color) för [Area](../../com.aspose.cells/area).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setBorder(Line value) {#setBorder-com.aspose.cells.Line-}
```
public void setBorder(Line value)
```


Ställer in kanten [Line](../../com.aspose.cells/line).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Line](../../com.aspose.cells/line) |  |

### setForegroundColor(Color value) {#setForegroundColor-com.aspose.cells.Color-}
```
public void setForegroundColor(Color value)
```


Ställer in förgrundens [Color](../../com.aspose.cells/color).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setFormatting(int value) {#setFormatting-int-}
```
public void setFormatting(int value)
```


Representerar formateringen av området.

Se [FormattingType](../../com.aspose.cells/formattingtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setInvertIfNegative(boolean value) {#setInvertIfNegative-boolean-}
```
public void setInvertIfNegative(boolean value)
```


Om egenskapen är sann och värdet för diagrampunkten är ett negativt tal, kommer förgrundsfärgen och bakgrundsfärgen att bytas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Returnerar eller anger graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (klar).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

