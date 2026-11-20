---
title: "Walls"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Objekt, das die Wände eines 3‑D‑Diagramms darstellt."
type: docs
url: /de/java/com.aspose.cells/walls/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Area](../../com.aspose.cells/area), [com.aspose.cells.Floor](../../com.aspose.cells/floor)
```
public class Walls extends Floor
```

Kapselt das Objekt, das die Wände eines 3‑D‑Diagramms darstellt.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundColor()](#getBackgroundColor--) | Ruft die Hintergrund-[Color](../../com.aspose.cells/color) des [Area](../../com.aspose.cells/area) ab. |
| [getBorder()](#getBorder--) | Ruft die Rand-[Line](../../com.aspose.cells/line) ab. |
| [getCenterX()](#getCenterX--) | Liest die x‑Koordinate der linken unteren Ecke des Wandzentrums in Einheiten von 1/4000 der Diagrammbreite nach Aufruf der Methode Chart.Calculate(). |
| [getCenterXPx()](#getCenterXPx--) | Liest die x‑Koordinate der linken unteren Ecke des Wandzentrums in Pixeln nach Aufruf der Methode Chart.Calculate(). |
| [getCenterY()](#getCenterY--) | Liest die y‑Koordinate der linken unteren Ecke des Wandzentrums in Einheiten von 1/4000 der Diagrammhöhe nach Aufruf der Methode Chart.Calculate(). |
| [getCenterYPx()](#getCenterYPx--) | Liest die y‑Koordinate der linken unteren Ecke des Wandzentrums in Pixeln nach Aufruf der Methode Chart.Calculate(). |
| [getClass()](#getClass--) |  |
| [getCubePointCount()](#getCubePointCount--) | Liest die Anzahl der Würfelpunkte nach Aufruf der Methode Chart.Calculate(). |
| [getCubePointXPx(int index)](#getCubePointXPx-int-) | Liest die x‑Koordinate des Scheitelpunkts des Wandwürfels nach Aufruf der Methode Chart.Calculate(). |
| [getCubePointYPx(int index)](#getCubePointYPx-int-) | Liest die y‑Koordinate des Scheitelpunkts des Wandwürfels nach Aufruf der Methode Chart.Calculate(). |
| [getDepth()](#getDepth--) | Liest die Tiefe von vorne nach hinten in Einheiten von 1/4000 der Diagrammbreite nach Aufruf der Methode Chart.Calculate(). |
| [getDepthPx()](#getDepthPx--) | Liest die Tiefe von vorne nach hinten in Pixeln nach Aufruf der Methode Chart.Calculate(). |
| [getFillFormat()](#getFillFormat--) | Stellt ein [getFillFormat()](../../com.aspose.cells/area\#getFillFormat--) Objekt dar, das Füllformatierungs‑Eigenschaften für das angegebene Diagramm oder die angegebene Form enthält. |
| [getForegroundColor()](#getForegroundColor--) | Ruft die Vordergrund-[Color](../../com.aspose.cells/color) ab. |
| [getFormatting()](#getFormatting--) | Stellt die Formatierung des Bereichs dar. |
| [getHeight()](#getHeight--) | Ermittelt die Höhe von oben nach unten in Einheiten von 1/4000 der Diagrammhöhe, nachdem die Methode Chart.Calculate() aufgerufen wurde. |
| [getHeightPx()](#getHeightPx--) | Ermittelt die Höhe von oben nach unten in Pixeln, nachdem die Methode Chart.Calculate() aufgerufen wurde. |
| [getInvertIfNegative()](#getInvertIfNegative--) | Wenn die Eigenschaft wahr ist und der Wert des Diagrammpunkts eine negative Zahl ist, werden Vordergrund‑ und Hintergrundfarbe vertauscht. |
| [getTransparency()](#getTransparency--) | Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
| [getWidth()](#getWidth--) | Ermittelt die Breite von links nach rechts in Einheiten von 1/4000 der Diagrammbreite, nachdem die Methode Chart.Calculate() aufgerufen wurde. |
| [getWidthPx()](#getWidthPx--) | Ermittelt die Breite von links nach rechts in Pixeln, nachdem die Methode Chart.Calculate() aufgerufen wurde. |
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
### getCenterX() {#getCenterX--}
```
public int getCenterX()
```


Liest die x‑Koordinate der linken unteren Ecke des Wandzentrums in Einheiten von 1/4000 der Diagrammbreite nach Aufruf der Methode Chart.Calculate().

**Returns:**
int
### getCenterXPx() {#getCenterXPx--}
```
public int getCenterXPx()
```


Liest die x‑Koordinate der linken unteren Ecke des Wandzentrums in Pixeln nach Aufruf der Methode Chart.Calculate().

**Returns:**
int
### getCenterY() {#getCenterY--}
```
public int getCenterY()
```


Liest die y‑Koordinate der linken unteren Ecke des Wandzentrums in Einheiten von 1/4000 der Diagrammhöhe nach Aufruf der Methode Chart.Calculate().

**Returns:**
int
### getCenterYPx() {#getCenterYPx--}
```
public int getCenterYPx()
```


Liest die y‑Koordinate der linken unteren Ecke des Wandzentrums in Pixeln nach Aufruf der Methode Chart.Calculate().

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCubePointCount() {#getCubePointCount--}
```
public int getCubePointCount()
```


Liest die Anzahl der Würfelpunkte nach Aufruf der Methode Chart.Calculate().

**Returns:**
int
### getCubePointXPx(int index) {#getCubePointXPx-int-}
```
public float getCubePointXPx(int index)
```


Ermittelt die x‑Koordinate des Scheitelpunkts des Wandwürfels nach dem Aufruf der Methode Chart.Calculate(). Die Anzahl der Scheitelpunkte des Wandwürfels beträgt acht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int |  |

**Returns:**
float
### getCubePointYPx(int index) {#getCubePointYPx-int-}
```
public float getCubePointYPx(int index)
```


Ermittelt die y‑Koordinate des Scheitelpunkts des Wandwürfels nach dem Aufruf der Methode Chart.Calculate(). Die Anzahl der Scheitelpunkte des Wandwürfels beträgt acht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int |  |

**Returns:**
float
### getDepth() {#getDepth--}
```
public int getDepth()
```


Liest die Tiefe von vorne nach hinten in Einheiten von 1/4000 der Diagrammbreite nach Aufruf der Methode Chart.Calculate().

**Returns:**
int
### getDepthPx() {#getDepthPx--}
```
public int getDepthPx()
```


Liest die Tiefe von vorne nach hinten in Pixeln nach Aufruf der Methode Chart.Calculate().

**Returns:**
int
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
### getHeight() {#getHeight--}
```
public int getHeight()
```


Ermittelt die Höhe von oben nach unten in Einheiten von 1/4000 der Diagrammhöhe, nachdem die Methode Chart.Calculate() aufgerufen wurde.

**Returns:**
int
### getHeightPx() {#getHeightPx--}
```
public int getHeightPx()
```


Ermittelt die Höhe von oben nach unten in Pixeln, nachdem die Methode Chart.Calculate() aufgerufen wurde.

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
### getWidth() {#getWidth--}
```
public int getWidth()
```


Ermittelt die Breite von links nach rechts in Einheiten von 1/4000 der Diagrammbreite, nachdem die Methode Chart.Calculate() aufgerufen wurde.

**Returns:**
int
### getWidthPx() {#getWidthPx--}
```
public int getWidthPx()
```


Ermittelt die Breite von links nach rechts in Pixeln, nachdem die Methode Chart.Calculate() aufgerufen wurde.

**Returns:**
int
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

