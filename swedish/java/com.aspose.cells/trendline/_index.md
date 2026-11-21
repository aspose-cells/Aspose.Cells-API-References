---
title: "Trendlinje"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en trendlinje i ett diagram."
type: docs
url: /sv/java/com.aspose.cells/trendline/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Line](../../com.aspose.cells/line)
```
public class Trendline extends Line
```

Representerar en trendlinje i ett diagram.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackward()](#getBackward--) | Returnerar eller anger antalet perioder (eller enheter på ett spridningsdiagram) som trendlinjen sträcker sig bakåt. |
| [getBeginArrowLength()](#getBeginArrowLength--) | Anger längden på pilspetsen för början av en linje. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | Anger bredden på pilspetsen för början av en linje. |
| [getBeginType()](#getBeginType--) | Anger en pilspets för början av en linje. |
| [getCapType()](#getCapType--) | Anger avslutningskapparna. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Representerar [Color](../../com.aspose.cells/color) för linjen. |
| [getCompoundType()](#getCompoundType--) | Anger den sammansatta linjetypen |
| [getDashType()](#getDashType--) | Anger den streckade linjetypen |
| [getDataLabels()](#getDataLabels--) | Representerar DataLabels-objektet för den angivna serien. |
| [getDisplayEquation()](#getDisplayEquation--) | Representerar om ekvationen för trendlinjen visas på diagrammet (i samma datamärkning som R-kvadrerat-värdet). |
| [getDisplayRSquared()](#getDisplayRSquared--) | Representerar om R-kvadrerat-värdet för trendlinjen visas på diagrammet (i samma datamärkning som ekvationen). |
| [getEndArrowLength()](#getEndArrowLength--) | Anger längden på pilspetsen för slutet av en linje. |
| [getEndArrowWidth()](#getEndArrowWidth--) | Anger bredden på pilspetsen för slutet av en linje. |
| [getEndType()](#getEndType--) | Anger en pilspets för slutet av en linje. |
| [getFormattingType()](#getFormattingType--) | Hämtar formattyp. |
| [getForward()](#getForward--) | Returnerar eller anger antalet perioder (eller enheter på ett spridningsdiagram) som trendlinjen sträcker sig framåt. |
| [getGradientFill()](#getGradientFill--) | Representerar gradientfyllning. |
| [getIntercept()](#getIntercept--) | Returnerar eller anger punkten där trendlinjen korsar värdeaxeln. |
| [getJoinType()](#getJoinType--) | Anger anslutningsändarna. |
| [getLegendEntry()](#getLegendEntry--) | Hämtar förklaringsposten enligt denna trendlinje |
| [getName()](#getName--) | Returnerar namnet på trendlinjen. |
| [getOrder()](#getOrder--) | Returnerar eller anger trendlinjens ordning (ett heltal större än 1) när trendlinjetypen är Polynom. |
| [getPeriod()](#getPeriod--) | Returnerar eller anger perioden för den glidande medelvärdestrendlinjen. |
| [getStyle()](#getStyle--) | Representerar linjens stil. |
| [getThemeColor()](#getThemeColor--) | Hämtar temafärgen. |
| [getTransparency()](#getTransparency--) | Returnerar eller anger graden av transparens för linjen som ett värde från 0.0 (opak) till 1.0 (klar). |
| [getType()](#getType--) | Returnerar trendlinjetypen. |
| [getWeight()](#getWeight--) | Hämtar [WeightType](../../com.aspose.cells/weighttype) för linjen. |
| [getWeightPt()](#getWeightPt--) | Hämtar linjens vikt i enheter av punkter. |
| [getWeightPx()](#getWeightPx--) | Hämtar linjens vikt i enheter av pixlar. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Indikerar om denna linjestil är automatiskt tilldelad. |
| [isAutomaticColor()](#isAutomaticColor--) | Indikerar om linjens färg är automatiskt tilldelad. |
| [isInterceptAuto()](#isInterceptAuto--) | Indikerar om Microsoft Workbook automatiskt bestämmer interceptet för trendlinjen. |
| [isNameAuto()](#isNameAuto--) | Returnerar om Microsoft Excel automatiskt bestämmer namnet på trendlinjen. |
| [isVisible()](#isVisible--) | Representerar om linjen är synlig. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuto(boolean value)](#setAuto-boolean-) | Indikerar om denna linjestil är automatiskt tilldelad. |
| [setBackward(double value)](#setBackward-double-) | Returnerar eller anger antalet perioder (eller enheter på ett spridningsdiagram) som trendlinjen sträcker sig bakåt. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | Anger längden på pilspetsen för början av en linje. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | Anger bredden på pilspetsen för början av en linje. |
| [setBeginType(int value)](#setBeginType-int-) | Anger en pilspets för början av en linje. |
| [setCapType(int value)](#setCapType-int-) | Anger avslutningskapparna. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Representerar [Color](../../com.aspose.cells/color) för linjen. |
| [setCompoundType(int value)](#setCompoundType-int-) | Anger den sammansatta linjetypen |
| [setDashType(int value)](#setDashType-int-) | Anger den streckade linjetypen |
| [setDisplayEquation(boolean value)](#setDisplayEquation-boolean-) | Representerar om ekvationen för trendlinjen visas på diagrammet (i samma datamärkning som R-kvadrerat-värdet). |
| [setDisplayRSquared(boolean value)](#setDisplayRSquared-boolean-) | Representerar om R-kvadrerat-värdet för trendlinjen visas på diagrammet (i samma datamärkning som ekvationen). |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | Anger längden på pilspetsen för slutet av en linje. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | Anger bredden på pilspetsen för slutet av en linje. |
| [setEndType(int value)](#setEndType-int-) | Anger en pilspets för slutet av en linje. |
| [setFormattingType(int value)](#setFormattingType-int-) | Anger formattyp. |
| [setForward(double value)](#setForward-double-) | Returnerar eller anger antalet perioder (eller enheter på ett spridningsdiagram) som trendlinjen sträcker sig framåt. |
| [setIntercept(double value)](#setIntercept-double-) | Returnerar eller anger punkten där trendlinjen korsar värdeaxeln. |
| [setInterceptAuto(boolean isInterceptAuto)](#setInterceptAuto-boolean-) | Anger om Microsoft Workbook automatiskt bestämmer interceptet för trendlinjen. |
| [setJoinType(int value)](#setJoinType-int-) | Anger anslutningsändarna. |
| [setName(String value)](#setName-java.lang.String-) | Returnerar namnet på trendlinjen. |
| [setNameAuto(boolean value)](#setNameAuto-boolean-) | Returnerar om Microsoft Excel automatiskt bestämmer namnet på trendlinjen. |
| [setOrder(int value)](#setOrder-int-) | Returnerar eller anger trendlinjens ordning (ett heltal större än 1) när trendlinjetypen är Polynom. |
| [setPeriod(int value)](#setPeriod-int-) | Returnerar eller anger perioden för den glidande medelvärdestrendlinjen. |
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
### getBackward() {#getBackward--}
```
public double getBackward()
```


Returnerar eller anger antalet perioder (eller enheter i ett spridningsdiagram) som trendlinjen sträcker sig bakåt. Antalet perioder måste vara större än eller lika med noll. Om diagramtypen är kolumn måste antalet perioder vara mellan 0 och 0,5.

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
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


Representerar DataLabels-objektet för den angivna serien.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDisplayEquation() {#getDisplayEquation--}
```
public boolean getDisplayEquation()
```


Anger om ekvationen för trendlinjen visas i diagrammet (i samma datamärkning som R-kvadratvärdet). Att sätta denna egenskap till True aktiverar automatiskt datamärkningar.

**Returns:**
boolean
### getDisplayRSquared() {#getDisplayRSquared--}
```
public boolean getDisplayRSquared()
```


Anger om R-kvadratvärdet för trendlinjen visas i diagrammet (i samma datamärkning som ekvationen). Att sätta denna egenskap till True aktiverar automatiskt datamärkningar.

**Returns:**
boolean
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
### getForward() {#getForward--}
```
public double getForward()
```


Returnerar eller anger antalet perioder (eller enheter i ett spridningsdiagram) som trendlinjen sträcker sig framåt. Antalet perioder måste vara större än eller lika med noll.

**Returns:**
double
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Representerar gradientfyllning.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getIntercept() {#getIntercept--}
```
public double getIntercept()
```


Returnerar eller anger punkten där trendlinjen korsar värdeaxeln.

**Returns:**
double
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Anger anslutningsändarna.

Se [LineJoinType](../../com.aspose.cells/linejointype).

**Returns:**
int
### getLegendEntry() {#getLegendEntry--}
```
public LegendEntry getLegendEntry()
```


Hämtar förklaringsposten enligt denna trendlinje

**Returns:**
[LegendEntry](../../com.aspose.cells/legendentry)
### getName() {#getName--}
```
public String getName()
```


Returnerar namnet på trendlinjen.

**Returns:**
java.lang.String
### getOrder() {#getOrder--}
```
public int getOrder()
```


Returnerar eller anger trendlinjens ordning (ett heltal större än 1) när trendlinjetypen är Polynom. Ordningen måste vara mellan 2 och 6.

**Returns:**
int
### getPeriod() {#getPeriod--}
```
public int getPeriod()
```


Returnerar eller anger perioden för den glidande medelvärdestrendlinjen.

**Remarks**

Detta värde bör vara mellan 2 och 255. Och det måste vara mindre än antalet diagrampunkter i serien.

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
### getType() {#getType--}
```
public int getType()
```


Returnerar trendlinjetypen.

Se [TrendlineType](../../com.aspose.cells/trendlinetype).

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
### isInterceptAuto() {#isInterceptAuto--}
```
public boolean isInterceptAuto()
```


Indikerar om Microsoft Workbook automatiskt bestämmer interceptet för trendlinjen.

**Returns:**
boolean
### isNameAuto() {#isNameAuto--}
```
public boolean isNameAuto()
```


Returnerar om Microsoft Excel automatiskt bestämmer namnet på trendlinjen.

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

### setBackward(double value) {#setBackward-double-}
```
public void setBackward(double value)
```


Returnerar eller anger antalet perioder (eller enheter i ett spridningsdiagram) som trendlinjen sträcker sig bakåt. Antalet perioder måste vara större än eller lika med noll. Om diagramtypen är kolumn måste antalet perioder vara mellan 0 och 0,5.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

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

### setDisplayEquation(boolean value) {#setDisplayEquation-boolean-}
```
public void setDisplayEquation(boolean value)
```


Anger om ekvationen för trendlinjen visas i diagrammet (i samma datamärkning som R-kvadratvärdet). Att sätta denna egenskap till True aktiverar automatiskt datamärkningar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDisplayRSquared(boolean value) {#setDisplayRSquared-boolean-}
```
public void setDisplayRSquared(boolean value)
```


Anger om R-kvadratvärdet för trendlinjen visas i diagrammet (i samma datamärkning som ekvationen). Att sätta denna egenskap till True aktiverar automatiskt datamärkningar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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

### setForward(double value) {#setForward-double-}
```
public void setForward(double value)
```


Returnerar eller anger antalet perioder (eller enheter i ett spridningsdiagram) som trendlinjen sträcker sig framåt. Antalet perioder måste vara större än eller lika med noll.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setIntercept(double value) {#setIntercept-double-}
```
public void setIntercept(double value)
```


Returnerar eller anger punkten där trendlinjen korsar värdeaxeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setInterceptAuto(boolean isInterceptAuto) {#setInterceptAuto-boolean-}
```
public void setInterceptAuto(boolean isInterceptAuto)
```


Anger om Microsoft Workbook automatiskt bestämmer interceptet för trendlinjen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isInterceptAuto | boolean |  |

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

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Returnerar namnet på trendlinjen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setNameAuto(boolean value) {#setNameAuto-boolean-}
```
public void setNameAuto(boolean value)
```


Returnerar om Microsoft Excel automatiskt bestämmer namnet på trendlinjen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setOrder(int value) {#setOrder-int-}
```
public void setOrder(int value)
```


Returnerar eller anger trendlinjens ordning (ett heltal större än 1) när trendlinjetypen är Polynom. Ordningen måste vara mellan 2 och 6.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPeriod(int value) {#setPeriod-int-}
```
public void setPeriod(int value)
```


Returnerar eller anger perioden för den glidande medelvärdestrendlinjen.

**Remarks**

Detta värde bör vara mellan 2 och 255. Och det måste vara mindre än antalet diagrampunkter i serien.

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

