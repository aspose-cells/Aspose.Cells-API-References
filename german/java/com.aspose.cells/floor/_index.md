---
title: "Floor"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Objekt, das den Boden eines 3‑D‑Diagramms darstellt."
type: docs
url: /de/java/com.aspose.cells/floor/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Area](../../com.aspose.cells/area)
```
public class Floor extends Area
```

Kapselt das Objekt, das den Boden eines 3‑D‑Diagramms darstellt.

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
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundColor()](#getBackgroundColor--) | Ruft die Hintergrund-[Color](../../com.aspose.cells/color) des [Area](../../com.aspose.cells/area) ab. |
| [getBorder()](#getBorder--) | Ruft die Rand-[Line](../../com.aspose.cells/line) ab. |
| [getClass()](#getClass--) |  |
| [getFillFormat()](#getFillFormat--) | Stellt ein [getFillFormat()](../../com.aspose.cells/area\#getFillFormat--) Objekt dar, das Füllformatierungs‑Eigenschaften für das angegebene Diagramm oder die angegebene Form enthält. |
| [getForegroundColor()](#getForegroundColor--) | Ruft die Vordergrund-[Color](../../com.aspose.cells/color) ab. |
| [getFormatting()](#getFormatting--) | Stellt die Formatierung des Bereichs dar. |
| [getInvertIfNegative()](#getInvertIfNegative--) | Wenn die Eigenschaft wahr ist und der Wert des Diagrammpunkts eine negative Zahl ist, werden Vordergrund‑ und Hintergrundfarbe vertauscht. |
| [getTransparency()](#getTransparency--) | Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundColor(Color value)](#setBackgroundColor-com.aspose.cells.Color-) | Setzt die Hintergrund-[Color](../../com.aspose.cells/color)-Farbe des [Area](../../com.aspose.cells/area). |
| [setBorder(Line value)](#setBorder-com.aspose.cells.Line-) | Sets the border [Line](../../com.aspose.cells/line). |
| [setForegroundColor(Color value)](#setForegroundColor-com.aspose.cells.Color-) | Setzt die Vordergrund-[Color](../../com.aspose.cells/color)-Farbe. |
| [setFormatting(int value)](#setFormatting-int-) | Stellt die Formatierung des Bereichs dar. |
| [setInvertIfNegative(boolean value)](#setInvertIfNegative-boolean-) | Wenn die Eigenschaft wahr ist und der Wert des Diagrammpunkts eine negative Zahl ist, werden Vordergrund‑ und Hintergrundfarbe vertauscht. |
| [setTransparency(double value)](#setTransparency-double-) | Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


Ruft die Hintergrund-[Color](../../com.aspose.cells/color) des [Area](../../com.aspose.cells/area) ab.

**Returns:**
[Color](../../com.aspose.cells/color)
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Ruft die Rand-[Line](../../com.aspose.cells/line) ab.

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


Stellt ein [getFillFormat()](../../com.aspose.cells/area\#getFillFormat--) Objekt dar, das Füllformatierungs‑Eigenschaften für das angegebene Diagramm oder die angegebene Form enthält.

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getForegroundColor() {#getForegroundColor--}
```
public Color getForegroundColor()
```


Ruft die Vordergrund-[Color](../../com.aspose.cells/color) ab.

**Returns:**
[Color](../../com.aspose.cells/color)
### getFormatting() {#getFormatting--}
```
public int getFormatting()
```


Stellt die Formatierung des Bereichs dar.

Siehe [FormattingType](../../com.aspose.cells/formattingtype).

**Returns:**
int
### getInvertIfNegative() {#getInvertIfNegative--}
```
public boolean getInvertIfNegative()
```


Wenn die Eigenschaft wahr ist und der Wert des Diagrammpunkts eine negative Zahl ist, werden Vordergrund‑ und Hintergrundfarbe vertauscht.

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


Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent).

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


Setzt die Hintergrund-[Color](../../com.aspose.cells/color)-Farbe des [Area](../../com.aspose.cells/area).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setBorder(Line value) {#setBorder-com.aspose.cells.Line-}
```
public void setBorder(Line value)
```


Sets the border [Line](../../com.aspose.cells/line).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Line](../../com.aspose.cells/line) |  |

### setForegroundColor(Color value) {#setForegroundColor-com.aspose.cells.Color-}
```
public void setForegroundColor(Color value)
```


Setzt die Vordergrund-[Color](../../com.aspose.cells/color)-Farbe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setFormatting(int value) {#setFormatting-int-}
```
public void setFormatting(int value)
```


Stellt die Formatierung des Bereichs dar.

Siehe [FormattingType](../../com.aspose.cells/formattingtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setInvertIfNegative(boolean value) {#setInvertIfNegative-boolean-}
```
public void setInvertIfNegative(boolean value)
```


Wenn die Eigenschaft wahr ist und der Wert des Diagrammpunkts eine negative Zahl ist, werden Vordergrund‑ und Hintergrundfarbe vertauscht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

