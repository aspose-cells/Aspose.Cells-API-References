---
title: "Line"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar objektet som representerar linjeformatet."
type: docs
url: /sv/java/com.aspose.cells/line/
---

**Inheritance:**
java.lang.Object
```
public class Line
```

Inkapslar objektet som representerar linjeformatet.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBeginArrowLength()](#getBeginArrowLength--) | Anger längden på pilspetsen för början av en linje. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | Anger bredden på pilspetsen för början av en linje. |
| [getBeginType()](#getBeginType--) | Anger en pilspets för början av en linje. |
| [getCapType()](#getCapType--) | Anger avslutningskapparna. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Representerar [Color](../../com.aspose.cells/color) för linjen. |
| [getCompoundType()](#getCompoundType--) | Anger den sammansatta linjetypen |
| [getDashType()](#getDashType--) | Anger den streckade linjetypen |
| [getEndArrowLength()](#getEndArrowLength--) | Anger längden på pilspetsen för slutet av en linje. |
| [getEndArrowWidth()](#getEndArrowWidth--) | Anger bredden på pilspetsen för slutet av en linje. |
| [getEndType()](#getEndType--) | Anger en pilspets för slutet av en linje. |
| [getFormattingType()](#getFormattingType--) | Hämtar formattyp. |
| [getGradientFill()](#getGradientFill--) | Representerar gradientfyllning. |
| [getJoinType()](#getJoinType--) | Anger anslutningsändarna. |
| [getStyle()](#getStyle--) | Representerar linjens stil. |
| [getThemeColor()](#getThemeColor--) | Hämtar temafärgen. |
| [getTransparency()](#getTransparency--) | Returnerar eller anger graden av transparens för linjen som ett värde från 0.0 (opak) till 1.0 (klar). |
| [getWeight()](#getWeight--) | Hämtar [WeightType](../../com.aspose.cells/weighttype) för linjen. |
| [getWeightPt()](#getWeightPt--) | Hämtar linjens vikt i enheter av punkter. |
| [getWeightPx()](#getWeightPx--) | Hämtar linjens vikt i enheter av pixlar. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Indikerar om denna linjestil är automatiskt tilldelad. |
| [isAutomaticColor()](#isAutomaticColor--) | Indikerar om linjens färg är automatiskt tilldelad. |
| [isVisible()](#isVisible--) | Representerar om linjen är synlig. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuto(boolean value)](#setAuto-boolean-) | Indikerar om denna linjestil är automatiskt tilldelad. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | Anger längden på pilspetsen för början av en linje. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | Anger bredden på pilspetsen för början av en linje. |
| [setBeginType(int value)](#setBeginType-int-) | Anger en pilspets för början av en linje. |
| [setCapType(int value)](#setCapType-int-) | Anger avslutningskapparna. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Representerar [Color](../../com.aspose.cells/color) för linjen. |
| [setCompoundType(int value)](#setCompoundType-int-) | Anger den sammansatta linjetypen |
| [setDashType(int value)](#setDashType-int-) | Anger den streckade linjetypen |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | Anger längden på pilspetsen för slutet av en linje. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | Anger bredden på pilspetsen för slutet av en linje. |
| [setEndType(int value)](#setEndType-int-) | Anger en pilspets för slutet av en linje. |
| [setFormattingType(int value)](#setFormattingType-int-) | Anger formattyp. |
| [setJoinType(int value)](#setJoinType-int-) | Anger anslutningsändarna. |
| [setStyle(int value)](#setStyle-int-) | Representerar linjens stil. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Anger temafärgen. |
| [setTransparency(double value)](#setTransparency-double-) | Returnerar eller anger graden av transparens för linjen som ett värde från 0.0 (opak) till 1.0 (klar). |
| [setVisible(boolean value)](#setVisible-boolean-) | Representerar om linjen är synlig. |
| [setWeight(int value)](#setWeight-int-) | Anger [WeightType](../../com.aspose.cells/weighttype) för linjen. |
| [setWeightPt(double value)](#setWeightPt-double-) | Anger linjens vikt i enheter av punkter. |
| [setWeightPx(double value)](#setWeightPx-double-) | Ställer in linjens vikt i enhet pixlar. |
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
### getBeginArrowLength() {#getBeginArrowLength--}
```
public int getBeginArrowLength()
```


Anger längden på pilspetsen för början av en linje.

Se [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Returns:**
int
### getBeginArrowWidth() {#getBeginArrowWidth--}
```
public int getBeginArrowWidth()
```


Anger bredden på pilspetsen för början av en linje.

Se [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Returns:**
int
### getBeginType() {#getBeginType--}
```
public int getBeginType()
```


Anger en pilspets för början av en linje.

Se [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Returns:**
int
### getCapType() {#getCapType--}
```
public int getCapType()
```


Anger avslutningskapparna.

Se [LineCapType](../../com.aspose.cells/linecaptype).

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


Representerar [Color](../../com.aspose.cells/color) för linjen.

**Returns:**
[Color](../../com.aspose.cells/color)
### getCompoundType() {#getCompoundType--}
```
public int getCompoundType()
```


Anger den sammansatta linjetypen

Se [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Returns:**
int
### getDashType() {#getDashType--}
```
public int getDashType()
```


Anger den streckade linjetypen

Se [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Returns:**
int
### getEndArrowLength() {#getEndArrowLength--}
```
public int getEndArrowLength()
```


Anger längden på pilspetsen för slutet av en linje.

Se [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Returns:**
int
### getEndArrowWidth() {#getEndArrowWidth--}
```
public int getEndArrowWidth()
```


Anger bredden på pilspetsen för slutet av en linje.

Se [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Returns:**
int
### getEndType() {#getEndType--}
```
public int getEndType()
```


Anger en pilspets för slutet av en linje.

Se [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Returns:**
int
### getFormattingType() {#getFormattingType--}
```
public int getFormattingType()
```


Hämtar formattyp.

Se [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype).

**Returns:**
int
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Representerar gradientfyllning.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Anger anslutningsändarna.

Se [LineJoinType](../../com.aspose.cells/linejointype).

**Returns:**
int
### getStyle() {#getStyle--}
```
public int getStyle()
```


Representerar linjens stil.

Se [LineType](../../com.aspose.cells/linetype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Hämtar temafärgen.

**Remarks**

Om förgrundsfärgen inte är en temafärg returneras NULL.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Returnerar eller anger graden av transparens för linjen som ett värde från 0.0 (opak) till 1.0 (klar).

**Returns:**
double
### getWeight() {#getWeight--}
```
public int getWeight()
```


Hämtar [WeightType](../../com.aspose.cells/weighttype) för linjen.

Se [WeightType](../../com.aspose.cells/weighttype).

**Returns:**
int
### getWeightPt() {#getWeightPt--}
```
public double getWeightPt()
```


Hämtar linjens vikt i enheter av punkter.

**Returns:**
double
### getWeightPx() {#getWeightPx--}
```
public double getWeightPx()
```


Hämtar linjens vikt i enheter av pixlar.

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


Indikerar om denna linjestil är automatiskt tilldelad.

**Returns:**
boolean
### isAutomaticColor() {#isAutomaticColor--}
```
public boolean isAutomaticColor()
```


Indikerar om linjens färg är automatiskt tilldelad.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Representerar om linjen är synlig.

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


Indikerar om denna linjestil är automatiskt tilldelad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setBeginArrowLength(int value) {#setBeginArrowLength-int-}
```
public void setBeginArrowLength(int value)
```


Anger längden på pilspetsen för början av en linje.

Se [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setBeginArrowWidth(int value) {#setBeginArrowWidth-int-}
```
public void setBeginArrowWidth(int value)
```


Anger bredden på pilspetsen för början av en linje.

Se [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setBeginType(int value) {#setBeginType-int-}
```
public void setBeginType(int value)
```


Anger en pilspets för början av en linje.

Se [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setCapType(int value) {#setCapType-int-}
```
public void setCapType(int value)
```


Anger avslutningskapparna.

Se [LineCapType](../../com.aspose.cells/linecaptype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Representerar [Color](../../com.aspose.cells/color) för linjen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```


Anger den sammansatta linjetypen

Se [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setDashType(int value) {#setDashType-int-}
```
public void setDashType(int value)
```


Anger den streckade linjetypen

Se [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setEndArrowLength(int value) {#setEndArrowLength-int-}
```
public void setEndArrowLength(int value)
```


Anger längden på pilspetsen för slutet av en linje.

Se [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setEndArrowWidth(int value) {#setEndArrowWidth-int-}
```
public void setEndArrowWidth(int value)
```


Anger bredden på pilspetsen för slutet av en linje.

Se [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setEndType(int value) {#setEndType-int-}
```
public void setEndType(int value)
```


Anger en pilspets för slutet av en linje.

Se [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setFormattingType(int value) {#setFormattingType-int-}
```
public void setFormattingType(int value)
```


Anger formattyp.

Se [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```


Anger anslutningsändarna.

Se [LineJoinType](../../com.aspose.cells/linejointype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```


Representerar linjens stil.

Se [LineType](../../com.aspose.cells/linetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Anger temafärgen.

**Remarks**

Om förgrundsfärgen inte är en temafärg returneras NULL.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Returnerar eller anger graden av transparens för linjen som ett värde från 0.0 (opak) till 1.0 (klar).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Representerar om linjen är synlig.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setWeight(int value) {#setWeight-int-}
```
public void setWeight(int value)
```


Anger [WeightType](../../com.aspose.cells/weighttype) för linjen.

Se [WeightType](../../com.aspose.cells/weighttype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setWeightPt(double value) {#setWeightPt-double-}
```
public void setWeightPt(double value)
```


Anger linjens vikt i enheter av punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setWeightPx(double value) {#setWeightPx-double-}
```
public void setWeightPx(double value)
```


Ställer in linjens vikt i enhet pixlar.

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

