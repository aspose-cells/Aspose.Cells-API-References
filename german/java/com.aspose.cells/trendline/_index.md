---
title: "Trendlinie"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt eine Trendlinie in einem Diagramm dar."
type: docs
url: /de/java/com.aspose.cells/trendline/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Line](../../com.aspose.cells/line)
```
public class Trendline extends Line
```

Stellt eine Trendlinie in einem Diagramm dar.

**Example**

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
         //adding a linear trendline
         int index = chart.getNSeries().get(0).getTrendLines().add(TrendlineType.LINEAR);
         Trendline trendline = chart.getNSeries().get(0).getTrendLines().get(index);
         //Setting the custom name of the trendline.
         trendline.setName("Linear");
         //Displaying the equation on chart
         trendline.setDisplayEquation(true);
         //Displaying the R-Squared value on chart
         trendline.setDisplayRSquared(true);
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackward()](#getBackward--) | Gibt die Anzahl der Perioden (oder Einheiten in einem Streudiagramm) zurück oder legt sie fest, über die die Trendlinie rückwärts erstreckt wird. |
| [getBeginArrowLength()](#getBeginArrowLength--) | Gibt die Länge der Pfeilspitze für den Anfang einer Linie an. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | Gibt die Breite der Pfeilspitze für den Anfang einer Linie an. |
| [getBeginType()](#getBeginType--) | Gibt eine Pfeilspitze für den Anfang einer Linie an. |
| [getCapType()](#getCapType--) | Gibt die Endkappen an. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Stellt die [Color](../../com.aspose.cells/color) der Linie dar. |
| [getCompoundType()](#getCompoundType--) | Gibt den zusammengesetzten Linientyp an |
| [getDashType()](#getDashType--) | Gibt den Strichlinientyp an |
| [getDataLabels()](#getDataLabels--) | Stellt das DataLabels-Objekt für die angegebene Serie dar. |
| [getDisplayEquation()](#getDisplayEquation--) | Stellt dar, ob die Gleichung für die Trendlinie im Diagramm angezeigt wird (im selben Datenbeschriftung wie der R-Quadrat-Wert). |
| [getDisplayRSquared()](#getDisplayRSquared--) | Stellt dar, ob der R-Quadrat-Wert der Trendlinie im Diagramm angezeigt wird (im selben Datenbeschriftung wie die Gleichung). |
| [getEndArrowLength()](#getEndArrowLength--) | Gibt die Länge der Pfeilspitze für das Ende einer Linie an. |
| [getEndArrowWidth()](#getEndArrowWidth--) | Gibt die Breite der Pfeilspitze für das Ende einer Linie an. |
| [getEndType()](#getEndType--) | Gibt einen Pfeilkopf für das Ende einer Linie an. |
| [getFormattingType()](#getFormattingType--) | Ermittelt den Formattyp. |
| [getForward()](#getForward--) | Gibt die Anzahl der Perioden (oder Einheiten in einem Streudiagramm) zurück oder legt sie fest, um die die Trendlinie nach vorne verläuft. |
| [getGradientFill()](#getGradientFill--) | Stellt einen Farbverlauf dar. |
| [getIntercept()](#getIntercept--) | Gibt den Punkt zurück oder legt ihn fest, an dem die Trendlinie die Werteachse schneidet. |
| [getJoinType()](#getJoinType--) | Gibt die Verbindungsenden an. |
| [getLegendEntry()](#getLegendEntry--) | Ermittelt den Legendeeintrag entsprechend dieser Trendlinie |
| [getName()](#getName--) | Gibt den Namen der Trendlinie zurück. |
| [getOrder()](#getOrder--) | Gibt die Reihenfolge der Trendlinie zurück oder legt sie fest (eine ganze Zahl größer als 1), wenn der Trendlinientyp Polynomisch ist. |
| [getPeriod()](#getPeriod--) | Gibt den Zeitraum für die gleitende Mittelwert-Trendlinie zurück oder legt ihn fest. |
| [getStyle()](#getStyle--) | Stellt den Stil der Linie dar. |
| [getThemeColor()](#getThemeColor--) | Ermittelt die Designfarbe. |
| [getTransparency()](#getTransparency--) | Gibt den Transparenzgrad der Linie zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
| [getType()](#getType--) | Gibt den Trendlinientyp zurück. |
| [getWeight()](#getWeight--) | Ermittelt den [WeightType](../../com.aspose.cells/weighttype) der Linie. |
| [getWeightPt()](#getWeightPt--) | Ermittelt das Gewicht der Linie in Punkten. |
| [getWeightPx()](#getWeightPx--) | Ermittelt das Gewicht der Linie in Pixeln. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Gibt an, ob dieser Linienstil automatisch zugewiesen wird. |
| [isAutomaticColor()](#isAutomaticColor--) | Gibt an, ob die Farbe der Linie automatisch zugewiesen wird. |
| [isInterceptAuto()](#isInterceptAuto--) | Gibt an, ob Microsoft Workbook den Schnittpunkt der Trendlinie automatisch bestimmt. |
| [isNameAuto()](#isNameAuto--) | Gibt zurück, ob Microsoft Excel den Namen der Trendlinie automatisch bestimmt. |
| [isVisible()](#isVisible--) | Stellt dar, ob die Linie sichtbar ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuto(boolean value)](#setAuto-boolean-) | Gibt an, ob dieser Linienstil automatisch zugewiesen wird. |
| [setBackward(double value)](#setBackward-double-) | Gibt die Anzahl der Perioden (oder Einheiten in einem Streudiagramm) zurück oder legt sie fest, über die die Trendlinie rückwärts erstreckt wird. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | Gibt die Länge der Pfeilspitze für den Anfang einer Linie an. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | Gibt die Breite der Pfeilspitze für den Anfang einer Linie an. |
| [setBeginType(int value)](#setBeginType-int-) | Gibt eine Pfeilspitze für den Anfang einer Linie an. |
| [setCapType(int value)](#setCapType-int-) | Gibt die Endkappen an. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Stellt die [Color](../../com.aspose.cells/color) der Linie dar. |
| [setCompoundType(int value)](#setCompoundType-int-) | Gibt den zusammengesetzten Linientyp an |
| [setDashType(int value)](#setDashType-int-) | Gibt den Strichlinientyp an |
| [setDisplayEquation(boolean value)](#setDisplayEquation-boolean-) | Stellt dar, ob die Gleichung für die Trendlinie im Diagramm angezeigt wird (im selben Datenbeschriftung wie der R-Quadrat-Wert). |
| [setDisplayRSquared(boolean value)](#setDisplayRSquared-boolean-) | Stellt dar, ob der R-Quadrat-Wert der Trendlinie im Diagramm angezeigt wird (im selben Datenbeschriftung wie die Gleichung). |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | Gibt die Länge der Pfeilspitze für das Ende einer Linie an. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | Gibt die Breite der Pfeilspitze für das Ende einer Linie an. |
| [setEndType(int value)](#setEndType-int-) | Gibt einen Pfeilkopf für das Ende einer Linie an. |
| [setFormattingType(int value)](#setFormattingType-int-) | Legt den Formattyp fest. |
| [setForward(double value)](#setForward-double-) | Gibt die Anzahl der Perioden (oder Einheiten in einem Streudiagramm) zurück oder legt sie fest, um die die Trendlinie nach vorne verläuft. |
| [setIntercept(double value)](#setIntercept-double-) | Gibt den Punkt zurück oder legt ihn fest, an dem die Trendlinie die Werteachse schneidet. |
| [setInterceptAuto(boolean isInterceptAuto)](#setInterceptAuto-boolean-) | Legt fest, ob Microsoft Workbook den Schnittpunkt der Trendlinie automatisch bestimmt. |
| [setJoinType(int value)](#setJoinType-int-) | Gibt die Verbindungsenden an. |
| [setName(String value)](#setName-java.lang.String-) | Gibt den Namen der Trendlinie zurück. |
| [setNameAuto(boolean value)](#setNameAuto-boolean-) | Gibt zurück, ob Microsoft Excel den Namen der Trendlinie automatisch bestimmt. |
| [setOrder(int value)](#setOrder-int-) | Gibt die Reihenfolge der Trendlinie zurück oder legt sie fest (eine ganze Zahl größer als 1), wenn der Trendlinientyp Polynomisch ist. |
| [setPeriod(int value)](#setPeriod-int-) | Gibt den Zeitraum für die gleitende Mittelwert-Trendlinie zurück oder legt ihn fest. |
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
### getBackward() {#getBackward--}
```
public double getBackward()
```


Gibt die Anzahl der Perioden (oder Einheiten in einem Streudiagramm) zurück oder legt sie fest, um die die Trendlinie rückwärts verläuft. Die Anzahl der Perioden muss größer oder gleich null sein. Wenn der Diagrammtyp Spalte ist, muss die Anzahl der Perioden zwischen 0 und 0,5 liegen.

**Returns:**
double
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
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


Stellt das DataLabels-Objekt für die angegebene Serie dar.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDisplayEquation() {#getDisplayEquation--}
```
public boolean getDisplayEquation()
```


Gibt an, ob die Gleichung für die Trendlinie im Diagramm angezeigt wird (im selben Datenbeschriftungsfeld wie der Bestimmtheitsmaßwert). Das Setzen dieser Eigenschaft auf True aktiviert automatisch Datenbeschriftungen.

**Returns:**
boolean
### getDisplayRSquared() {#getDisplayRSquared--}
```
public boolean getDisplayRSquared()
```


Gibt an, ob der Bestimmtheitsmaßwert der Trendlinie im Diagramm angezeigt wird (im selben Datenbeschriftungsfeld wie die Gleichung). Das Setzen dieser Eigenschaft auf True aktiviert automatisch Datenbeschriftungen.

**Returns:**
boolean
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
### getForward() {#getForward--}
```
public double getForward()
```


Gibt die Anzahl der Perioden (oder Einheiten in einem Streudiagramm) zurück oder legt sie fest, um die die Trendlinie vorwärts verläuft. Die Anzahl der Perioden muss größer oder gleich null sein.

**Returns:**
double
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Stellt einen Farbverlauf dar.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getIntercept() {#getIntercept--}
```
public double getIntercept()
```


Gibt den Punkt zurück oder legt ihn fest, an dem die Trendlinie die Werteachse schneidet.

**Returns:**
double
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Gibt die Verbindungsenden an.

Siehe [LineJoinType](../../com.aspose.cells/linejointype).

**Returns:**
int
### getLegendEntry() {#getLegendEntry--}
```
public LegendEntry getLegendEntry()
```


Ermittelt den Legendeeintrag entsprechend dieser Trendlinie

**Returns:**
[LegendEntry](../../com.aspose.cells/legendentry)
### getName() {#getName--}
```
public String getName()
```


Gibt den Namen der Trendlinie zurück.

**Returns:**
java.lang.String
### getOrder() {#getOrder--}
```
public int getOrder()
```


Gibt die Reihenfolge der Trendlinie (eine ganze Zahl größer als 1) zurück oder legt sie fest, wenn der Trendlinientyp Polynom ist. Die Reihenfolge muss zwischen 2 und 6 liegen.

**Returns:**
int
### getPeriod() {#getPeriod--}
```
public int getPeriod()
```


Gibt den Zeitraum für die gleitende Mittelwert-Trendlinie zurück oder legt ihn fest.

**Remarks**

Dieser Wert sollte zwischen 2 und 255 liegen. Und er muss kleiner sein als die Anzahl der Diagrammpunkte in der Serie.

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
### getType() {#getType--}
```
public int getType()
```


Gibt den Trendlinientyp zurück.

Siehe [TrendlineType](../../com.aspose.cells/trendlinetype).

**Returns:**
int
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
### isInterceptAuto() {#isInterceptAuto--}
```
public boolean isInterceptAuto()
```


Gibt an, ob Microsoft Workbook den Schnittpunkt der Trendlinie automatisch bestimmt.

**Returns:**
boolean
### isNameAuto() {#isNameAuto--}
```
public boolean isNameAuto()
```


Gibt zurück, ob Microsoft Excel den Namen der Trendlinie automatisch bestimmt.

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

### setBackward(double value) {#setBackward-double-}
```
public void setBackward(double value)
```


Gibt die Anzahl der Perioden (oder Einheiten in einem Streudiagramm) zurück oder legt sie fest, um die die Trendlinie rückwärts verläuft. Die Anzahl der Perioden muss größer oder gleich null sein. Wenn der Diagrammtyp Spalte ist, muss die Anzahl der Perioden zwischen 0 und 0,5 liegen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

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

### setDisplayEquation(boolean value) {#setDisplayEquation-boolean-}
```
public void setDisplayEquation(boolean value)
```


Gibt an, ob die Gleichung für die Trendlinie im Diagramm angezeigt wird (im selben Datenbeschriftungsfeld wie der Bestimmtheitsmaßwert). Das Setzen dieser Eigenschaft auf True aktiviert automatisch Datenbeschriftungen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDisplayRSquared(boolean value) {#setDisplayRSquared-boolean-}
```
public void setDisplayRSquared(boolean value)
```


Gibt an, ob der Bestimmtheitsmaßwert der Trendlinie im Diagramm angezeigt wird (im selben Datenbeschriftungsfeld wie die Gleichung). Das Setzen dieser Eigenschaft auf True aktiviert automatisch Datenbeschriftungen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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

### setForward(double value) {#setForward-double-}
```
public void setForward(double value)
```


Gibt die Anzahl der Perioden (oder Einheiten in einem Streudiagramm) zurück oder legt sie fest, um die die Trendlinie vorwärts verläuft. Die Anzahl der Perioden muss größer oder gleich null sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setIntercept(double value) {#setIntercept-double-}
```
public void setIntercept(double value)
```


Gibt den Punkt zurück oder legt ihn fest, an dem die Trendlinie die Werteachse schneidet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setInterceptAuto(boolean isInterceptAuto) {#setInterceptAuto-boolean-}
```
public void setInterceptAuto(boolean isInterceptAuto)
```


Legt fest, ob Microsoft Workbook den Schnittpunkt der Trendlinie automatisch bestimmt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isInterceptAuto | boolean |  |

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

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Gibt den Namen der Trendlinie zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setNameAuto(boolean value) {#setNameAuto-boolean-}
```
public void setNameAuto(boolean value)
```


Gibt zurück, ob Microsoft Excel den Namen der Trendlinie automatisch bestimmt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setOrder(int value) {#setOrder-int-}
```
public void setOrder(int value)
```


Gibt die Reihenfolge der Trendlinie (eine ganze Zahl größer als 1) zurück oder legt sie fest, wenn der Trendlinientyp Polynom ist. Die Reihenfolge muss zwischen 2 und 6 liegen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPeriod(int value) {#setPeriod-int-}
```
public void setPeriod(int value)
```


Gibt den Zeitraum für die gleitende Mittelwert-Trendlinie zurück oder legt ihn fest.

**Remarks**

Dieser Wert sollte zwischen 2 und 255 liegen. Und er muss kleiner sein als die Anzahl der Diagrammpunkte in der Serie.

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

