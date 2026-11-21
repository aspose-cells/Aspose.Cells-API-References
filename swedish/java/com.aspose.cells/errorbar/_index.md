---
title: "ErrorBar"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar felstapeln för dataserier."
type: docs
url: /sv/java/com.aspose.cells/errorbar/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Line](../../com.aspose.cells/line)
```
public class ErrorBar extends Line
```

Representerar felstapeln för dataserier.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAmount()](#getAmount--) | Representerar mängden felstaplar. |
| [getBeginArrowLength()](#getBeginArrowLength--) | Anger längden på pilspetsen för början av en linje. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | Anger bredden på pilspetsen för början av en linje. |
| [getBeginType()](#getBeginType--) | Anger en pilspets för början av en linje. |
| [getCapType()](#getCapType--) | Anger avslutningskapparna. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Representerar [Color](../../com.aspose.cells/color) för linjen. |
| [getCompoundType()](#getCompoundType--) | Anger den sammansatta linjetypen |
| [getDashType()](#getDashType--) | Anger den streckade linjetypen |
| [getDisplayType()](#getDisplayType--) | Representerar visningstypen för felstaplar. |
| [getEndArrowLength()](#getEndArrowLength--) | Anger längden på pilspetsen för slutet av en linje. |
| [getEndArrowWidth()](#getEndArrowWidth--) | Anger bredden på pilspetsen för slutet av en linje. |
| [getEndType()](#getEndType--) | Anger en pilspets för slutet av en linje. |
| [getFormattingType()](#getFormattingType--) | Hämtar formattyp. |
| [getGradientFill()](#getGradientFill--) | Representerar gradientfyllning. |
| [getJoinType()](#getJoinType--) | Anger anslutningsändarna. |
| [getMinusValue()](#getMinusValue--) | Representerar negativt felvärde när felstapeln är Custom. |
| [getPlusValue()](#getPlusValue--) | Representerar positivt felvärde när felstapeln är Custom. |
| [getShowMarkerTTop()](#getShowMarkerTTop--) | Indikerar om felstaplar formateras med en T-top. |
| [getStyle()](#getStyle--) | Representerar linjens stil. |
| [getThemeColor()](#getThemeColor--) | Hämtar temafärgen. |
| [getTransparency()](#getTransparency--) | Returnerar eller anger graden av transparens för linjen som ett värde från 0.0 (opak) till 1.0 (klar). |
| [getType()](#getType--) | Representerar felstapelsbeloppstyp. |
| [getWeight()](#getWeight--) | Hämtar [WeightType](../../com.aspose.cells/weighttype) för linjen. |
| [getWeightPt()](#getWeightPt--) | Hämtar linjens vikt i enheter av punkter. |
| [getWeightPx()](#getWeightPx--) | Hämtar linjens vikt i enheter av pixlar. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Indikerar om denna linjestil är automatiskt tilldelad. |
| [isAutomaticColor()](#isAutomaticColor--) | Indikerar om linjens färg är automatiskt tilldelad. |
| [isVisible()](#isVisible--) | Representerar om linjen är synlig. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAmount(double value)](#setAmount-double-) | Representerar mängden felstaplar. |
| [setAuto(boolean value)](#setAuto-boolean-) | Indikerar om denna linjestil är automatiskt tilldelad. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | Anger längden på pilspetsen för början av en linje. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | Anger bredden på pilspetsen för början av en linje. |
| [setBeginType(int value)](#setBeginType-int-) | Anger en pilspets för början av en linje. |
| [setCapType(int value)](#setCapType-int-) | Anger avslutningskapparna. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Representerar [Color](../../com.aspose.cells/color) för linjen. |
| [setCompoundType(int value)](#setCompoundType-int-) | Anger den sammansatta linjetypen |
| [setDashType(int value)](#setDashType-int-) | Anger den streckade linjetypen |
| [setDisplayType(int value)](#setDisplayType-int-) | Representerar visningstypen för felstaplar. |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | Anger längden på pilspetsen för slutet av en linje. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | Anger bredden på pilspetsen för slutet av en linje. |
| [setEndType(int value)](#setEndType-int-) | Anger en pilspets för slutet av en linje. |
| [setFormattingType(int value)](#setFormattingType-int-) | Anger formattyp. |
| [setJoinType(int value)](#setJoinType-int-) | Anger anslutningsändarna. |
| [setMinusValue(String value)](#setMinusValue-java.lang.String-) | Representerar negativt felvärde när felstapeln är Custom. |
| [setPlusValue(String value)](#setPlusValue-java.lang.String-) | Representerar positivt felvärde när felstapeln är Custom. |
| [setShowMarkerTTop(boolean value)](#setShowMarkerTTop-boolean-) | Indikerar om felstaplar formateras med en T-top. |
| [setStyle(int value)](#setStyle-int-) | Representerar linjens stil. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Anger temafärgen. |
| [setTransparency(double value)](#setTransparency-double-) | Returnerar eller anger graden av transparens för linjen som ett värde från 0.0 (opak) till 1.0 (klar). |
| [setType(int value)](#setType-int-) | Representerar felstapelsbeloppstyp. |
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
### getAmount() {#getAmount--}
```
public double getAmount()
```


Representerar mängden felstaplar.

**Remarks**

Beloppet måste vara större än eller lika med noll.

**Returns:**
double
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
### getDisplayType() {#getDisplayType--}
```
public int getDisplayType()
```


Representerar visningstypen för felstaplar.

Se [ErrorBarDisplayType](../../com.aspose.cells/errorbardisplaytype).

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
### getMinusValue() {#getMinusValue--}
```
public String getMinusValue()
```


Representerar negativt felvärde när felstapeln är Custom.

**Returns:**
java.lang.String
### getPlusValue() {#getPlusValue--}
```
public String getPlusValue()
```


Representerar positivt felvärde när felstapeln är Custom.

**Returns:**
java.lang.String
### getShowMarkerTTop() {#getShowMarkerTTop--}
```
public boolean getShowMarkerTTop()
```


Indikerar om felstaplar formateras med en T-top.

**Returns:**
boolean
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
### getType() {#getType--}
```
public int getType()
```


Representerar felstapelsbeloppstyp.

Se [ErrorBarType](../../com.aspose.cells/errorbartype).

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




### setAmount(double value) {#setAmount-double-}
```
public void setAmount(double value)
```


Representerar mängden felstaplar.

**Remarks**

Beloppet måste vara större än eller lika med noll.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

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

### setDisplayType(int value) {#setDisplayType-int-}
```
public void setDisplayType(int value)
```


Representerar visningstypen för felstaplar.

Se [ErrorBarDisplayType](../../com.aspose.cells/errorbardisplaytype).

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

### setMinusValue(String value) {#setMinusValue-java.lang.String-}
```
public void setMinusValue(String value)
```


Representerar negativt felvärde när felstapeln är Custom.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setPlusValue(String value) {#setPlusValue-java.lang.String-}
```
public void setPlusValue(String value)
```


Representerar positivt felvärde när felstapeln är Custom.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setShowMarkerTTop(boolean value) {#setShowMarkerTTop-boolean-}
```
public void setShowMarkerTTop(boolean value)
```


Indikerar om felstaplar formateras med en T-top.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Representerar felstapelsbeloppstyp.

Se [ErrorBarType](../../com.aspose.cells/errorbartype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

