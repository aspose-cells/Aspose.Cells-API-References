---
title: "Line"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Objekt, das das Linienformat darstellt."
type: docs
url: /de/java/com.aspose.cells/line/
---

**Inheritance:**
java.lang.Object
```
public class Line
```

Kapselt das Objekt, das das Linienformat darstellt.

**Example**

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
 
         	int chartIndex = sheet.getCharts().add(ChartType.LINE, 9, 9, 21, 15);
         Chart chart = sheet.getCharts().get(chartIndex);
         //Add series
         chart.getNSeries().add("A2:B4", true);
         //Set category data
         chart.getNSeries().setCategoryData("=Sheet1!$A$2:$A$4");
         //Applying a dotted line style on the lines of an NSeries
         chart.getNSeries().get(0).getBorder().setStyle(LineType.DOT);
         chart.getNSeries().get(0).getBorder().setColor(Color.getRed());
         //Applying a triangular marker style on the data markers of an NSeries
         chart.getNSeries().get(0).getMarker().setMarkerStyle(ChartMarkerType.TRIANGLE);
         //Setting the weight of all lines in an NSeries to medium
         chart.getNSeries().get(0).getBorder().setWeight(WeightType.MEDIUM_LINE);
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBeginArrowLength()](#getBeginArrowLength--) | Gibt die Länge der Pfeilspitze für den Anfang einer Linie an. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | Gibt die Breite der Pfeilspitze für den Anfang einer Linie an. |
| [getBeginType()](#getBeginType--) | Gibt eine Pfeilspitze für den Anfang einer Linie an. |
| [getCapType()](#getCapType--) | Gibt die Endkappen an. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Stellt die [Color](../../com.aspose.cells/color) der Linie dar. |
| [getCompoundType()](#getCompoundType--) | Gibt den zusammengesetzten Linientyp an |
| [getDashType()](#getDashType--) | Gibt den Strichlinientyp an |
| [getEndArrowLength()](#getEndArrowLength--) | Gibt die Länge der Pfeilspitze für das Ende einer Linie an. |
| [getEndArrowWidth()](#getEndArrowWidth--) | Gibt die Breite der Pfeilspitze für das Ende einer Linie an. |
| [getEndType()](#getEndType--) | Gibt einen Pfeilkopf für das Ende einer Linie an. |
| [getFormattingType()](#getFormattingType--) | Ermittelt den Formattyp. |
| [getGradientFill()](#getGradientFill--) | Stellt einen Farbverlauf dar. |
| [getJoinType()](#getJoinType--) | Gibt die Verbindungsenden an. |
| [getStyle()](#getStyle--) | Stellt den Stil der Linie dar. |
| [getThemeColor()](#getThemeColor--) | Ermittelt die Designfarbe. |
| [getTransparency()](#getTransparency--) | Gibt den Transparenzgrad der Linie zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
| [getWeight()](#getWeight--) | Ermittelt den [WeightType](../../com.aspose.cells/weighttype) der Linie. |
| [getWeightPt()](#getWeightPt--) | Ermittelt das Gewicht der Linie in Punkten. |
| [getWeightPx()](#getWeightPx--) | Ermittelt das Gewicht der Linie in Pixeln. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Gibt an, ob dieser Linienstil automatisch zugewiesen wird. |
| [isAutomaticColor()](#isAutomaticColor--) | Gibt an, ob die Farbe der Linie automatisch zugewiesen wird. |
| [isVisible()](#isVisible--) | Stellt dar, ob die Linie sichtbar ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuto(boolean value)](#setAuto-boolean-) | Gibt an, ob dieser Linienstil automatisch zugewiesen wird. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | Gibt die Länge der Pfeilspitze für den Anfang einer Linie an. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | Gibt die Breite der Pfeilspitze für den Anfang einer Linie an. |
| [setBeginType(int value)](#setBeginType-int-) | Gibt eine Pfeilspitze für den Anfang einer Linie an. |
| [setCapType(int value)](#setCapType-int-) | Gibt die Endkappen an. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Stellt die [Color](../../com.aspose.cells/color) der Linie dar. |
| [setCompoundType(int value)](#setCompoundType-int-) | Gibt den zusammengesetzten Linientyp an |
| [setDashType(int value)](#setDashType-int-) | Gibt den Strichlinientyp an |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | Gibt die Länge der Pfeilspitze für das Ende einer Linie an. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | Gibt die Breite der Pfeilspitze für das Ende einer Linie an. |
| [setEndType(int value)](#setEndType-int-) | Gibt einen Pfeilkopf für das Ende einer Linie an. |
| [setFormattingType(int value)](#setFormattingType-int-) | Legt den Formattyp fest. |
| [setJoinType(int value)](#setJoinType-int-) | Gibt die Verbindungsenden an. |
| [setStyle(int value)](#setStyle-int-) | Stellt den Stil der Linie dar. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Legt die Designfarbe fest. |
| [setTransparency(double value)](#setTransparency-double-) | Gibt den Transparenzgrad der Linie zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
| [setVisible(boolean value)](#setVisible-boolean-) | Stellt dar, ob die Linie sichtbar ist. |
| [setWeight(int value)](#setWeight-int-) | Legt den [WeightType](../../com.aspose.cells/weighttype) der Linie fest. |
| [setWeightPt(double value)](#setWeightPt-double-) | Legt das Gewicht der Linie in Punkten fest. |
| [setWeightPx(double value)](#setWeightPx-double-) | Legt das Gewicht der Linie in Pixeln fest. |
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
### getBeginArrowLength() {#getBeginArrowLength--}
```
public int getBeginArrowLength()
```


Gibt die Länge der Pfeilspitze für den Anfang einer Linie an.

Siehe [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Returns:**
int
### getBeginArrowWidth() {#getBeginArrowWidth--}
```
public int getBeginArrowWidth()
```


Gibt die Breite der Pfeilspitze für den Anfang einer Linie an.

Siehe [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Returns:**
int
### getBeginType() {#getBeginType--}
```
public int getBeginType()
```


Gibt eine Pfeilspitze für den Anfang einer Linie an.

Siehe [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Returns:**
int
### getCapType() {#getCapType--}
```
public int getCapType()
```


Gibt die Endkappen an.

Siehe [LineCapType](../../com.aspose.cells/linecaptype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```


Stellt die [Color](../../com.aspose.cells/color) der Linie dar.

**Returns:**
[Color](../../com.aspose.cells/color)
### getCompoundType() {#getCompoundType--}
```
public int getCompoundType()
```


Gibt den zusammengesetzten Linientyp an

Siehe [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Returns:**
int
### getDashType() {#getDashType--}
```
public int getDashType()
```


Gibt den Strichlinientyp an

Siehe [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Returns:**
int
### getEndArrowLength() {#getEndArrowLength--}
```
public int getEndArrowLength()
```


Gibt die Länge der Pfeilspitze für das Ende einer Linie an.

Siehe [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Returns:**
int
### getEndArrowWidth() {#getEndArrowWidth--}
```
public int getEndArrowWidth()
```


Gibt die Breite der Pfeilspitze für das Ende einer Linie an.

Siehe [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Returns:**
int
### getEndType() {#getEndType--}
```
public int getEndType()
```


Gibt einen Pfeilkopf für das Ende einer Linie an.

Siehe [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Returns:**
int
### getFormattingType() {#getFormattingType--}
```
public int getFormattingType()
```


Ermittelt den Formattyp.

Siehe [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype).

**Returns:**
int
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Stellt einen Farbverlauf dar.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Gibt die Verbindungsenden an.

Siehe [LineJoinType](../../com.aspose.cells/linejointype).

**Returns:**
int
### getStyle() {#getStyle--}
```
public int getStyle()
```


Stellt den Stil der Linie dar.

Siehe [LineType](../../com.aspose.cells/linetype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Ermittelt die Designfarbe.

**Remarks**

Wenn die Vordergrundfarbe keine Designfarbe ist, wird NULL zurückgegeben.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Gibt den Transparenzgrad der Linie zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent).

**Returns:**
double
### getWeight() {#getWeight--}
```
public int getWeight()
```


Ermittelt den [WeightType](../../com.aspose.cells/weighttype) der Linie.

Siehe [WeightType](../../com.aspose.cells/weighttype).

**Returns:**
int
### getWeightPt() {#getWeightPt--}
```
public double getWeightPt()
```


Ermittelt das Gewicht der Linie in Punkten.

**Returns:**
double
### getWeightPx() {#getWeightPx--}
```
public double getWeightPx()
```


Ermittelt das Gewicht der Linie in Pixeln.

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


Gibt an, ob dieser Linienstil automatisch zugewiesen wird.

**Returns:**
boolean
### isAutomaticColor() {#isAutomaticColor--}
```
public boolean isAutomaticColor()
```


Gibt an, ob die Farbe der Linie automatisch zugewiesen wird.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Stellt dar, ob die Linie sichtbar ist.

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




### setAuto(boolean value) {#setAuto-boolean-}
```
public void setAuto(boolean value)
```


Gibt an, ob dieser Linienstil automatisch zugewiesen wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setBeginArrowLength(int value) {#setBeginArrowLength-int-}
```
public void setBeginArrowLength(int value)
```


Gibt die Länge der Pfeilspitze für den Anfang einer Linie an.

Siehe [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setBeginArrowWidth(int value) {#setBeginArrowWidth-int-}
```
public void setBeginArrowWidth(int value)
```


Gibt die Breite der Pfeilspitze für den Anfang einer Linie an.

Siehe [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setBeginType(int value) {#setBeginType-int-}
```
public void setBeginType(int value)
```


Gibt eine Pfeilspitze für den Anfang einer Linie an.

Siehe [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setCapType(int value) {#setCapType-int-}
```
public void setCapType(int value)
```


Gibt die Endkappen an.

Siehe [LineCapType](../../com.aspose.cells/linecaptype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Stellt die [Color](../../com.aspose.cells/color) der Linie dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```


Gibt den zusammengesetzten Linientyp an

Siehe [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setDashType(int value) {#setDashType-int-}
```
public void setDashType(int value)
```


Gibt den Strichlinientyp an

Siehe [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setEndArrowLength(int value) {#setEndArrowLength-int-}
```
public void setEndArrowLength(int value)
```


Gibt die Länge der Pfeilspitze für das Ende einer Linie an.

Siehe [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setEndArrowWidth(int value) {#setEndArrowWidth-int-}
```
public void setEndArrowWidth(int value)
```


Gibt die Breite der Pfeilspitze für das Ende einer Linie an.

Siehe [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setEndType(int value) {#setEndType-int-}
```
public void setEndType(int value)
```


Gibt einen Pfeilkopf für das Ende einer Linie an.

Siehe [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setFormattingType(int value) {#setFormattingType-int-}
```
public void setFormattingType(int value)
```


Legt den Formattyp fest.

Siehe [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```


Gibt die Verbindungsenden an.

Siehe [LineJoinType](../../com.aspose.cells/linejointype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```


Stellt den Stil der Linie dar.

Siehe [LineType](../../com.aspose.cells/linetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Legt die Designfarbe fest.

**Remarks**

Wenn die Vordergrundfarbe keine Designfarbe ist, wird NULL zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Gibt den Transparenzgrad der Linie zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Stellt dar, ob die Linie sichtbar ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setWeight(int value) {#setWeight-int-}
```
public void setWeight(int value)
```


Legt den [WeightType](../../com.aspose.cells/weighttype) der Linie fest.

Siehe [WeightType](../../com.aspose.cells/weighttype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setWeightPt(double value) {#setWeightPt-double-}
```
public void setWeightPt(double value)
```


Legt das Gewicht der Linie in Punkten fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setWeightPx(double value) {#setWeightPx-double-}
```
public void setWeightPx(double value)
```


Legt das Gewicht der Linie in Pixeln fest.

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

