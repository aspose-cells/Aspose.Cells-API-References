---
title: "ErrorBar"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Fehlerbalken einer Datenreihe dar."
type: docs
url: /de/java/com.aspose.cells/errorbar/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Line](../../com.aspose.cells/line)
```
public class ErrorBar extends Line
```

Stellt die Fehlerbalken einer Datenreihe dar.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("a1").putValue(2);
         cells.get("a2").putValue(5);
         cells.get("a3").putValue(3);
         cells.get("a4").putValue(6);
         cells.get("b1").putValue(4);
         cells.get("b2").putValue(3);
         cells.get("b3").putValue(6);
         cells.get("b4").putValue(7);
 
         cells.get("C1").putValue("Q1");
         cells.get("C2").putValue("Q2");
         cells.get("C3").putValue("Y1");
         cells.get("C4").putValue("Y2");
 
         int chartIndex = workbook.getWorksheets().get(0).getCharts().add(ChartType.COLUMN, 11, 0, 27, 10);
 
         Chart chart = workbook.getWorksheets().get(0).getCharts().get(chartIndex);
         chart.getNSeries().add("A1:B4", true);
 
         chart.getNSeries().setCategoryData("C1:C4");
 
         for(int i = 0; i <chart.getNSeries().getCount(); i ++)
         {
         		Series aseries = chart.getNSeries().get(i);
         		aseries.getYErrorBar().setDisplayType(ErrorBarDisplayType.MINUS);
         		aseries.getYErrorBar().setType(ErrorBarType.FIXED_VALUE);
         		aseries.getYErrorBar().setAmount(5);
         }
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAmount()](#getAmount--) | Stellt die Menge des Fehlerbalkens dar. |
| [getBeginArrowLength()](#getBeginArrowLength--) | Gibt die Länge der Pfeilspitze für den Anfang einer Linie an. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | Gibt die Breite der Pfeilspitze für den Anfang einer Linie an. |
| [getBeginType()](#getBeginType--) | Gibt eine Pfeilspitze für den Anfang einer Linie an. |
| [getCapType()](#getCapType--) | Gibt die Endkappen an. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Stellt die [Color](../../com.aspose.cells/color) der Linie dar. |
| [getCompoundType()](#getCompoundType--) | Gibt den zusammengesetzten Linientyp an |
| [getDashType()](#getDashType--) | Gibt den Strichlinientyp an |
| [getDisplayType()](#getDisplayType--) | Stellt den Anzeigetyp des Fehlerbalkens dar. |
| [getEndArrowLength()](#getEndArrowLength--) | Gibt die Länge der Pfeilspitze für das Ende einer Linie an. |
| [getEndArrowWidth()](#getEndArrowWidth--) | Gibt die Breite der Pfeilspitze für das Ende einer Linie an. |
| [getEndType()](#getEndType--) | Gibt einen Pfeilkopf für das Ende einer Linie an. |
| [getFormattingType()](#getFormattingType--) | Ermittelt den Formattyp. |
| [getGradientFill()](#getGradientFill--) | Stellt einen Farbverlauf dar. |
| [getJoinType()](#getJoinType--) | Gibt die Verbindungsenden an. |
| [getMinusValue()](#getMinusValue--) | Stellt die negative Fehlermenge dar, wenn der Fehlerbalkentyp Custom ist. |
| [getPlusValue()](#getPlusValue--) | Stellt die positive Fehlermenge dar, wenn der Fehlerbalkentyp Custom ist. |
| [getShowMarkerTTop()](#getShowMarkerTTop--) | Gibt an, ob Fehlerbalken mit einem T-Top formatiert werden. |
| [getStyle()](#getStyle--) | Stellt den Stil der Linie dar. |
| [getThemeColor()](#getThemeColor--) | Ermittelt die Designfarbe. |
| [getTransparency()](#getTransparency--) | Gibt den Transparenzgrad der Linie zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
| [getType()](#getType--) | Stellt den Betragstyp des Fehlerbalkens dar. |
| [getWeight()](#getWeight--) | Ermittelt den [WeightType](../../com.aspose.cells/weighttype) der Linie. |
| [getWeightPt()](#getWeightPt--) | Ermittelt das Gewicht der Linie in Punkten. |
| [getWeightPx()](#getWeightPx--) | Ermittelt das Gewicht der Linie in Pixeln. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Gibt an, ob dieser Linienstil automatisch zugewiesen wird. |
| [isAutomaticColor()](#isAutomaticColor--) | Gibt an, ob die Farbe der Linie automatisch zugewiesen wird. |
| [isVisible()](#isVisible--) | Stellt dar, ob die Linie sichtbar ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAmount(double value)](#setAmount-double-) | Stellt die Menge des Fehlerbalkens dar. |
| [setAuto(boolean value)](#setAuto-boolean-) | Gibt an, ob dieser Linienstil automatisch zugewiesen wird. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | Gibt die Länge der Pfeilspitze für den Anfang einer Linie an. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | Gibt die Breite der Pfeilspitze für den Anfang einer Linie an. |
| [setBeginType(int value)](#setBeginType-int-) | Gibt eine Pfeilspitze für den Anfang einer Linie an. |
| [setCapType(int value)](#setCapType-int-) | Gibt die Endkappen an. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Stellt die [Color](../../com.aspose.cells/color) der Linie dar. |
| [setCompoundType(int value)](#setCompoundType-int-) | Gibt den zusammengesetzten Linientyp an |
| [setDashType(int value)](#setDashType-int-) | Gibt den Strichlinientyp an |
| [setDisplayType(int value)](#setDisplayType-int-) | Stellt den Anzeigetyp des Fehlerbalkens dar. |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | Gibt die Länge der Pfeilspitze für das Ende einer Linie an. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | Gibt die Breite der Pfeilspitze für das Ende einer Linie an. |
| [setEndType(int value)](#setEndType-int-) | Gibt einen Pfeilkopf für das Ende einer Linie an. |
| [setFormattingType(int value)](#setFormattingType-int-) | Legt den Formattyp fest. |
| [setJoinType(int value)](#setJoinType-int-) | Gibt die Verbindungsenden an. |
| [setMinusValue(String value)](#setMinusValue-java.lang.String-) | Stellt die negative Fehlermenge dar, wenn der Fehlerbalkentyp Custom ist. |
| [setPlusValue(String value)](#setPlusValue-java.lang.String-) | Stellt die positive Fehlermenge dar, wenn der Fehlerbalkentyp Custom ist. |
| [setShowMarkerTTop(boolean value)](#setShowMarkerTTop-boolean-) | Gibt an, ob Fehlerbalken mit einem T-Top formatiert werden. |
| [setStyle(int value)](#setStyle-int-) | Stellt den Stil der Linie dar. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Legt die Designfarbe fest. |
| [setTransparency(double value)](#setTransparency-double-) | Gibt den Transparenzgrad der Linie zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
| [setType(int value)](#setType-int-) | Stellt den Betragstyp des Fehlerbalkens dar. |
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
### getAmount() {#getAmount--}
```
public double getAmount()
```


Stellt die Menge des Fehlerbalkens dar.

**Remarks**

Der Betrag muss größer oder gleich null sein.

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
### getDisplayType() {#getDisplayType--}
```
public int getDisplayType()
```


Stellt den Anzeigetyp des Fehlerbalkens dar.

Siehe [ErrorBarDisplayType](../../com.aspose.cells/errorbardisplaytype).

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
### getMinusValue() {#getMinusValue--}
```
public String getMinusValue()
```


Stellt die negative Fehlermenge dar, wenn der Fehlerbalkentyp Custom ist.

**Returns:**
java.lang.String
### getPlusValue() {#getPlusValue--}
```
public String getPlusValue()
```


Stellt die positive Fehlermenge dar, wenn der Fehlerbalkentyp Custom ist.

**Returns:**
java.lang.String
### getShowMarkerTTop() {#getShowMarkerTTop--}
```
public boolean getShowMarkerTTop()
```


Gibt an, ob Fehlerbalken mit einem T-Top formatiert werden.

**Returns:**
boolean
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


Stellt den Betragstyp des Fehlerbalkens dar.

Siehe [ErrorBarType](../../com.aspose.cells/errorbartype).

**Example**

```
         Workbook wb = new Workbook("chart.xlsx");
         Chart chart = wb.getWorksheets().get(0).getCharts().get(0);
         Series aseries = chart.getNSeries().get(0);
         //Gets custom error bar type
         /*ErrorBarType*/int errBarType = aseries.getYErrorBar().getType();
         //Sets custom error bar type
         aseries.getYErrorBar().setType(ErrorBarType.CUSTOM);
         aseries.getYErrorBar().setPlusValue("=Sheet1!A1");
         aseries.getYErrorBar().setMinusValue("=Sheet1!A2");
```

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




### setAmount(double value) {#setAmount-double-}
```
public void setAmount(double value)
```


Stellt die Menge des Fehlerbalkens dar.

**Remarks**

Der Betrag muss größer oder gleich null sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

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

### setDisplayType(int value) {#setDisplayType-int-}
```
public void setDisplayType(int value)
```


Stellt den Anzeigetyp des Fehlerbalkens dar.

Siehe [ErrorBarDisplayType](../../com.aspose.cells/errorbardisplaytype).

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

### setMinusValue(String value) {#setMinusValue-java.lang.String-}
```
public void setMinusValue(String value)
```


Stellt die negative Fehlermenge dar, wenn der Fehlerbalkentyp Custom ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setPlusValue(String value) {#setPlusValue-java.lang.String-}
```
public void setPlusValue(String value)
```


Stellt die positive Fehlermenge dar, wenn der Fehlerbalkentyp Custom ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setShowMarkerTTop(boolean value) {#setShowMarkerTTop-boolean-}
```
public void setShowMarkerTTop(boolean value)
```


Gibt an, ob Fehlerbalken mit einem T-Top formatiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Stellt den Betragstyp des Fehlerbalkens dar.

Siehe [ErrorBarType](../../com.aspose.cells/errorbartype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

