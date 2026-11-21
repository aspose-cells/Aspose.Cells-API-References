---
title: "Axel"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar objektet som representerar en axel i ett diagram."
type: docs
url: /sv/java/com.aspose.cells/axis/
---

**Inheritance:**
java.lang.Object
```
public class Axis
```

Inkapslar objektet som representerar en axel i ett diagram.

**Example**

Från följande kod kan du lära dig hur du ställer in enhet, maximalt och minimalt värde för Axeln.

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
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(4);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(20);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 25, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
         //Set the max value of value axis
         chart.getValueAxis().setMaxValue(200);
         //Set the min value of value axis
         chart.getValueAxis().setMinValue(0);
         //Set the major unit
         chart.getValueAxis().setMajorUnit(25);
         //Category(X) axis crosses at the maxinum value.
         chart.getValueAxis().setCrossType(CrossType.MAXIMUM);
         //Set he number of categories or series between tick-mark labels. 
         chart.getCategoryAxis().setTickLabelSpacing(2);
 
         //do your business
 
         //Saving the Excel file
         workbook.save("book1.xlsx");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Hämtar [getArea()](../../com.aspose.cells/axis\#getArea--). |
| [getAxisBetweenCategories()](#getAxisBetweenCategories--) | Representerar om värdeaxeln korsar kategoriaxeln mellan kategorierna. |
| [getAxisLabels()](#getAxisLabels--) | Hämtar axelns etiketter efter anrop av metoden Chart.Calculate(). |
| [getAxisLine()](#getAxisLine--) | Hämtar utseendet för en Axel. |
| [getAxisTexts()](#getAxisTexts--) | Hämtar axelns etiketter efter anrop av metoden Chart.Calculate(). |
| [getBaseUnitScale()](#getBaseUnitScale--) | Representerar basenhetsskalan för kategoriaxeln. |
| [getBins()](#getBins--) | Representerar fack på ett diagram (Histogram/Pareto)-axel |
| [getCategoryType()](#getCategoryType--) | Representerar typen av kategoriaxeln. |
| [getClass()](#getClass--) |  |
| [getCrossAt()](#getCrossAt--) | Representerar punkten på värdeaxeln där kategoriaxeln korsar den. |
| [getCrossType()](#getCrossType--) | Representerar [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) på den angivna axeln där den andra axeln korsar. |
| [getCustUnit()](#getCustUnit--) | Anger ett anpassat värde för visningsenheten. |
| [getCustomDisplayUnit()](#getCustomDisplayUnit--) | Anger ett anpassat värde för visningsenheten. |
| [getCustomUnit()](#getCustomUnit--) | Anger ett anpassat värde för visningsenheten. |
| [getDisplayUnit()](#getDisplayUnit--) | Representerar enhetsetiketten för den angivna axeln. |
| [getDisplayUnitLabel()](#getDisplayUnitLabel--) | Representerar en enhetsetikett på en axel i det angivna diagrammet. |
| [getLogBase()](#getLogBase--) | Representerar den logaritmiska basen. |
| [getMajorGridLines()](#getMajorGridLines--) | Representerar huvudrutnätslinjer på en diagramaxel. |
| [getMajorTickMark()](#getMajorTickMark--) | Representerar typen av huvudstämplar för den angivna axeln. |
| [getMajorUnit()](#getMajorUnit--) | Representerar huvudenheterna för axeln. |
| [getMajorUnitScale()](#getMajorUnitScale--) | Representerar huvudenhetsskalan för kategoriaxeln. |
| [getMaxValue()](#getMaxValue--) | Representerar det maximala värdet på värdeaxeln. |
| [getMinValue()](#getMinValue--) | Representerar det minsta värdet på värdeaxeln. |
| [getMinorGridLines()](#getMinorGridLines--) | Representerar mindre rutnätslinjer på en diagramaxel. |
| [getMinorTickMark()](#getMinorTickMark--) | Representerar typen av mindre stämplar för den angivna axeln. |
| [getMinorUnit()](#getMinorUnit--) | Representerar de mindre enheterna för axeln. |
| [getMinorUnitScale()](#getMinorUnitScale--) | Representerar huvudenhetsskalan för kategoriaxeln. |
| [getTickLabelPosition()](#getTickLabelPosition--) | Representerar positionen för stämplsetiketter på den angivna axeln. |
| [getTickLabelSpacing()](#getTickLabelSpacing--) | Representerar antalet kategorier eller serier mellan tick‑markeringarnas etiketter. |
| [getTickLabels()](#getTickLabels--) | Returnerar ett [getTickLabels()](../../com.aspose.cells/axis\#getTickLabels--) objekt som representerar tick‑markeringarnas etiketter för den angivna axeln. |
| [getTickMarkSpacing()](#getTickMarkSpacing--) | Returnerar eller anger antalet kategorier eller serier mellan tick‑markeringar. |
| [getTitle()](#getTitle--) | Hämtar titeln för denna axel i diagrammet. |
| [hasMultiLevelLabels()](#hasMultiLevelLabels--) | Indikerar om etiketterna ska visas som flernivå. |
| [hashCode()](#hashCode--) |  |
| [isAutoTickLabelSpacing()](#isAutoTickLabelSpacing--) | Indikerar om avståndet mellan tick‑etiketter är automatiskt. |
| [isAutomaticMajorUnit()](#isAutomaticMajorUnit--) | Indikerar om huvud‑enheten för axeln tilldelas automatiskt. |
| [isAutomaticMaxValue()](#isAutomaticMaxValue--) | Indikerar om maxvärdet tilldelas automatiskt. |
| [isAutomaticMinValue()](#isAutomaticMinValue--) | Indikerar om minvärdet tilldelas automatiskt. |
| [isAutomaticMinorUnit()](#isAutomaticMinorUnit--) | Indikerar om underenheten för axeln tilldelas automatiskt. |
| [isBaseUnitAuto()](#isBaseUnitAuto--) | Representerar om basenheten är automatisk. |
| [isDisplayUnitLabelShown()](#isDisplayUnitLabelShown--) | Representerar om display‑enhetsetiketten visas på den angivna axeln. |
| [isLogarithmic()](#isLogarithmic--) | Representerar om värdeaxelns skaltyp är logaritmisk eller inte. |
| [isPlotOrderReversed()](#isPlotOrderReversed--) | Representerar om Microsoft Excel ritar datapunkter från sista till första. |
| [isVisible()](#isVisible--) | Representerar om axeln är synlig. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoTickLabelSpacing(boolean value)](#setAutoTickLabelSpacing-boolean-) | Indikerar om avståndet mellan tick‑etiketter är automatiskt. |
| [setAutomaticMajorUnit(boolean value)](#setAutomaticMajorUnit-boolean-) | Indikerar om huvud‑enheten för axeln tilldelas automatiskt. |
| [setAutomaticMaxValue(boolean value)](#setAutomaticMaxValue-boolean-) | Indikerar om maxvärdet tilldelas automatiskt. |
| [setAutomaticMinValue(boolean value)](#setAutomaticMinValue-boolean-) | Indikerar om minvärdet tilldelas automatiskt. |
| [setAutomaticMinorUnit(boolean value)](#setAutomaticMinorUnit-boolean-) | Indikerar om underenheten för axeln tilldelas automatiskt. |
| [setAxisBetweenCategories(boolean value)](#setAxisBetweenCategories-boolean-) | Representerar om värdeaxeln korsar kategoriaxeln mellan kategorierna. |
| [setBaseUnitAuto(boolean value)](#setBaseUnitAuto-boolean-) | Representerar om basenheten är automatisk. |
| [setBaseUnitScale(int value)](#setBaseUnitScale-int-) | Representerar basenhetsskalan för kategoriaxeln. |
| [setCategoryType(int value)](#setCategoryType-int-) | Representerar typen av kategoriaxeln. |
| [setCrossAt(double value)](#setCrossAt-double-) | Representerar punkten på värdeaxeln där kategoriaxeln korsar den. |
| [setCrossType(int value)](#setCrossType-int-) | Representerar [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) på den angivna axeln där den andra axeln korsar. |
| [setCustUnit(int value)](#setCustUnit-int-) | Anger ett anpassat värde för visningsenheten. |
| [setCustomDisplayUnit(double value)](#setCustomDisplayUnit-double-) | Anger ett anpassat värde för visningsenheten. |
| [setCustomUnit(int value)](#setCustomUnit-int-) | Anger ett anpassat värde för visningsenheten. |
| [setDisplayUnit(int value)](#setDisplayUnit-int-) | Representerar enhetsetiketten för den angivna axeln. |
| [setDisplayUnitLabelShown(boolean value)](#setDisplayUnitLabelShown-boolean-) | Representerar om display‑enhetsetiketten visas på den angivna axeln. |
| [setHasMultiLevelLabels(boolean value)](#setHasMultiLevelLabels-boolean-) | Indikerar om etiketterna ska visas som flernivå. |
| [setLogBase(double value)](#setLogBase-double-) | Representerar den logaritmiska basen. |
| [setLogarithmic(boolean value)](#setLogarithmic-boolean-) | Representerar om värdeaxelns skaltyp är logaritmisk eller inte. |
| [setMajorTickMark(int value)](#setMajorTickMark-int-) | Representerar typen av huvudstämplar för den angivna axeln. |
| [setMajorUnit(double value)](#setMajorUnit-double-) | Representerar huvudenheterna för axeln. |
| [setMajorUnitScale(int value)](#setMajorUnitScale-int-) | Representerar huvudenhetsskalan för kategoriaxeln. |
| [setMaxValue(Object value)](#setMaxValue-java.lang.Object-) | Representerar det maximala värdet på värdeaxeln. |
| [setMinValue(Object value)](#setMinValue-java.lang.Object-) | Representerar det minsta värdet på värdeaxeln. |
| [setMinorTickMark(int value)](#setMinorTickMark-int-) | Representerar typen av mindre stämplar för den angivna axeln. |
| [setMinorUnit(double value)](#setMinorUnit-double-) | Representerar de mindre enheterna för axeln. |
| [setMinorUnitScale(int value)](#setMinorUnitScale-int-) | Representerar huvudenhetsskalan för kategoriaxeln. |
| [setPlotOrderReversed(boolean value)](#setPlotOrderReversed-boolean-) | Representerar om Microsoft Excel ritar datapunkter från sista till första. |
| [setTickLabelPosition(int value)](#setTickLabelPosition-int-) | Representerar positionen för stämplsetiketter på den angivna axeln. |
| [setTickLabelSpacing(int value)](#setTickLabelSpacing-int-) | Representerar antalet kategorier eller serier mellan tick‑markeringarnas etiketter. |
| [setTickMarkSpacing(int value)](#setTickMarkSpacing-int-) | Returnerar eller anger antalet kategorier eller serier mellan tick‑markeringar. |
| [setVisible(boolean value)](#setVisible-boolean-) | Representerar om axeln är synlig. |
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
### getArea() {#getArea--}
```
public Area getArea()
```


Hämtar [getArea()](../../com.aspose.cells/axis\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getAxisBetweenCategories() {#getAxisBetweenCategories--}
```
public boolean getAxisBetweenCategories()
```


Representerar om värdeaxeln korsar kategoriaxeln mellan kategorierna.

**Remarks**

Denna egenskap gäller endast för kategori‑axlar och gäller inte för 3‑D‑diagram.

**Returns:**
boolean
### getAxisLabels() {#getAxisLabels--}
```
public ArrayList getAxisLabels()
```


Hämtar axelns etiketter efter anrop av metoden Chart.Calculate().

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd i stället Axis.GetAxisTexts‑metoden. Denna egenskap kommer att tas bort 12 månader senare från och med november 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.util.ArrayList
### getAxisLine() {#getAxisLine--}
```
public Line getAxisLine()
```


Hämtar utseendet för en Axel.

**Returns:**
[Line](../../com.aspose.cells/line)
### getAxisTexts() {#getAxisTexts--}
```
public String[] getAxisTexts()
```


Hämtar axelns etiketter efter anrop av metoden Chart.Calculate().

**Returns:**
java.lang.String[]
### getBaseUnitScale() {#getBaseUnitScale--}
```
public int getBaseUnitScale()
```


Representerar basenhetsskalan för kategoriaxeln.

Se [TimeUnit](../../com.aspose.cells/timeunit).

**Remarks**

Gäller endast när egenskapen CategoryType är inställd på TimeScale.

**Returns:**
int
### getBins() {#getBins--}
```
public AxisBins getBins()
```


Representerar fack på ett diagram (Histogram/Pareto)-axel

**Remarks**

Endast för histogram‑ eller Pareto‑diagram.

**Returns:**
[AxisBins](../../com.aspose.cells/axisbins)
### getCategoryType() {#getCategoryType--}
```
public int getCategoryType()
```


Representerar typen av kategoriaxeln.

Se [CategoryType](../../com.aspose.cells/categorytype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCrossAt() {#getCrossAt--}
```
public double getCrossAt()
```


Representerar punkten på värdeaxeln där kategoriaxeln korsar den.

**Remarks**

Numret ska vara ett heltal när det gäller kategori‑axeln. Och värdet måste ligga mellan 1 och 31999.

**Returns:**
double
### getCrossType() {#getCrossType--}
```
public int getCrossType()
```


Representerar [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) på den angivna axeln där den andra axeln korsar.

Se [CrossType](../../com.aspose.cells/crosstype).

**Returns:**
int
### getCustUnit() {#getCustUnit--}
```
public int getCustUnit()
```


Anger ett anpassat värde för visningsenheten.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd i stället Axis.CustomUnit‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med januari 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getCustomDisplayUnit() {#getCustomDisplayUnit--}
```
public double getCustomDisplayUnit()
```


Anger ett anpassat värde för visningsenheten.

**Returns:**
double
### getCustomUnit() {#getCustomUnit--}
```
public int getCustomUnit()
```


Anger ett anpassat värde för visningsenheten.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd i stället Axis.CustomDisplayUnit‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getDisplayUnit() {#getDisplayUnit--}
```
public int getDisplayUnit()
```


Representerar enhetsetiketten för den angivna axeln.

Se [DisplayUnitType](../../com.aspose.cells/displayunittype).

**Returns:**
int
### getDisplayUnitLabel() {#getDisplayUnitLabel--}
```
public DisplayUnitLabel getDisplayUnitLabel()
```


Representerar en enhetsetikett på en axel i det angivna diagrammet. Enhetsetiketter är användbara för att diagrammera stora värden - till exempel i miljoner eller miljarder.

**Returns:**
[DisplayUnitLabel](../../com.aspose.cells/displayunitlabel)
### getLogBase() {#getLogBase--}
```
public double getLogBase()
```


Representerar den logaritmiska basen. Standardvärdet är 10.

**Returns:**
double
### getMajorGridLines() {#getMajorGridLines--}
```
public Line getMajorGridLines()
```


Representerar huvudrutnätslinjer på en diagramaxel.

**Example**

```
         chart.getValueAxis().getMajorGridLines().setVisible(false);
         chart.getCategoryAxis().getMajorGridLines().setVisible(true);
```

**Returns:**
[Line](../../com.aspose.cells/line)
### getMajorTickMark() {#getMajorTickMark--}
```
public int getMajorTickMark()
```


Representerar typen av huvudstämplar för den angivna axeln.

Se [TickMarkType](../../com.aspose.cells/tickmarktype).

**Returns:**
int
### getMajorUnit() {#getMajorUnit--}
```
public double getMajorUnit()
```


Representerar huvudenheterna för axeln.

**Remarks**

De stora enheterna måste vara större än noll.

**Returns:**
double
### getMajorUnitScale() {#getMajorUnitScale--}
```
public int getMajorUnitScale()
```


Representerar huvudenhetsskalan för kategoriaxeln.

Se [TimeUnit](../../com.aspose.cells/timeunit).

**Example**

```
         chart.getCategoryAxis().setCategoryType(CategoryType.TIME_SCALE);
         /*TimeUnit*/int majorUnitScale = chart.getCategoryAxis().getMajorUnitScale(); //get
         chart.getCategoryAxis().setMajorUnitScale(majorUnitScale); //set
         chart.getCategoryAxis().setMajorUnit(2);
```

**Returns:**
int
### getMaxValue() {#getMaxValue--}
```
public Object getMaxValue()
```


Representerar det maximala värdet på värdeaxeln.

**Remarks**

Typen maxValue kan endast vara double eller DateTime

**Returns:**
java.lang.Object
### getMinValue() {#getMinValue--}
```
public Object getMinValue()
```


Representerar det minsta värdet på värdeaxeln.

**Remarks**

Typen minValue kan endast vara double eller DateTime

**Returns:**
java.lang.Object
### getMinorGridLines() {#getMinorGridLines--}
```
public Line getMinorGridLines()
```


Representerar mindre rutnätslinjer på en diagramaxel.

**Returns:**
[Line](../../com.aspose.cells/line)
### getMinorTickMark() {#getMinorTickMark--}
```
public int getMinorTickMark()
```


Representerar typen av mindre stämplar för den angivna axeln.

Se [TickMarkType](../../com.aspose.cells/tickmarktype).

**Returns:**
int
### getMinorUnit() {#getMinorUnit--}
```
public double getMinorUnit()
```


Representerar de mindre enheterna för axeln.

**Remarks**

De mindre enheterna måste vara större än noll.

**Returns:**
double
### getMinorUnitScale() {#getMinorUnitScale--}
```
public int getMinorUnitScale()
```


Representerar huvudenhetsskalan för kategoriaxeln.

Se [TimeUnit](../../com.aspose.cells/timeunit).

**Example**

```
         chart.getCategoryAxis().setCategoryType(CategoryType.TIME_SCALE);
         chart.getCategoryAxis().setMinorUnitScale(TimeUnit.MONTHS);
         chart.getCategoryAxis().setMinorUnit(2);
```

**Returns:**
int
### getTickLabelPosition() {#getTickLabelPosition--}
```
public int getTickLabelPosition()
```


Representerar positionen för stämplsetiketter på den angivna axeln.

Se [TickLabelPositionType](../../com.aspose.cells/ticklabelpositiontype).

**Returns:**
int
### getTickLabelSpacing() {#getTickLabelSpacing--}
```
public int getTickLabelSpacing()
```


Representerar antalet kategorier eller serier mellan tick‑mark‑etiketter. Gäller endast för kategori‑ och serieaxlar.

**Remarks**

Numret måste vara mellan 1 och 31999.

**Returns:**
int
### getTickLabels() {#getTickLabels--}
```
public TickLabels getTickLabels()
```


Returnerar ett [getTickLabels()](../../com.aspose.cells/axis\#getTickLabels--) objekt som representerar tick‑markeringarnas etiketter för den angivna axeln.

**Returns:**
[TickLabels](../../com.aspose.cells/ticklabels)
### getTickMarkSpacing() {#getTickMarkSpacing--}
```
public int getTickMarkSpacing()
```


Returnerar eller anger antalet kategorier eller serier mellan tick‑markeringar. Gäller endast för kategori‑ och serieaxlar.

**Remarks**

Numret måste vara mellan 1 och 31999.

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Hämtar titeln för denna axel i diagrammet.

**Returns:**
[Title](../../com.aspose.cells/title)
### hasMultiLevelLabels() {#hasMultiLevelLabels--}
```
public boolean hasMultiLevelLabels()
```


Indikerar om etiketterna ska visas som flernivå.

**Remarks**

Endast giltig för kategoriaxel.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoTickLabelSpacing() {#isAutoTickLabelSpacing--}
```
public boolean isAutoTickLabelSpacing()
```


Indikerar om avståndet mellan tick‑etiketter är automatiskt.

**Returns:**
boolean
### isAutomaticMajorUnit() {#isAutomaticMajorUnit--}
```
public boolean isAutomaticMajorUnit()
```


Indikerar om huvud‑enheten för axeln tilldelas automatiskt.

**Returns:**
boolean
### isAutomaticMaxValue() {#isAutomaticMaxValue--}
```
public boolean isAutomaticMaxValue()
```


Indikerar om maxvärdet tilldelas automatiskt.

**Returns:**
boolean
### isAutomaticMinValue() {#isAutomaticMinValue--}
```
public boolean isAutomaticMinValue()
```


Indikerar om minvärdet tilldelas automatiskt.

**Returns:**
boolean
### isAutomaticMinorUnit() {#isAutomaticMinorUnit--}
```
public boolean isAutomaticMinorUnit()
```


Indikerar om underenheten för axeln tilldelas automatiskt.

**Returns:**
boolean
### isBaseUnitAuto() {#isBaseUnitAuto--}
```
public boolean isBaseUnitAuto()
```


Representerar om basenheten är automatisk.

**Returns:**
boolean
### isDisplayUnitLabelShown() {#isDisplayUnitLabelShown--}
```
public boolean isDisplayUnitLabelShown()
```


Representerar om display‑enhetsetiketten visas på den angivna axeln.

**Remarks**

Standardvärdet är True. Fungerar endast när [getDisplayUnit()](../../com.aspose.cells/axis\#getDisplayUnit--) inte är [DisplayUnitType.NONE](../../com.aspose.cells/displayunittype\#NONE).

**Returns:**
boolean
### isLogarithmic() {#isLogarithmic--}
```
public boolean isLogarithmic()
```


Representerar om värdeaxelns skaltyp är logaritmisk eller inte.

**Returns:**
boolean
### isPlotOrderReversed() {#isPlotOrderReversed--}
```
public boolean isPlotOrderReversed()
```


Representerar om Microsoft Excel ritar datapunkter från sista till första.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Representerar om axeln är synlig.

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




### setAutoTickLabelSpacing(boolean value) {#setAutoTickLabelSpacing-boolean-}
```
public void setAutoTickLabelSpacing(boolean value)
```


Indikerar om avståndet mellan tick‑etiketter är automatiskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAutomaticMajorUnit(boolean value) {#setAutomaticMajorUnit-boolean-}
```
public void setAutomaticMajorUnit(boolean value)
```


Indikerar om huvud‑enheten för axeln tilldelas automatiskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAutomaticMaxValue(boolean value) {#setAutomaticMaxValue-boolean-}
```
public void setAutomaticMaxValue(boolean value)
```


Indikerar om maxvärdet tilldelas automatiskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAutomaticMinValue(boolean value) {#setAutomaticMinValue-boolean-}
```
public void setAutomaticMinValue(boolean value)
```


Indikerar om minvärdet tilldelas automatiskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAutomaticMinorUnit(boolean value) {#setAutomaticMinorUnit-boolean-}
```
public void setAutomaticMinorUnit(boolean value)
```


Indikerar om underenheten för axeln tilldelas automatiskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAxisBetweenCategories(boolean value) {#setAxisBetweenCategories-boolean-}
```
public void setAxisBetweenCategories(boolean value)
```


Representerar om värdeaxeln korsar kategoriaxeln mellan kategorierna.

**Remarks**

Denna egenskap gäller endast för kategori‑axlar och gäller inte för 3‑D‑diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setBaseUnitAuto(boolean value) {#setBaseUnitAuto-boolean-}
```
public void setBaseUnitAuto(boolean value)
```


Representerar om basenheten är automatisk.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setBaseUnitScale(int value) {#setBaseUnitScale-int-}
```
public void setBaseUnitScale(int value)
```


Representerar basenhetsskalan för kategoriaxeln.

Se [TimeUnit](../../com.aspose.cells/timeunit).

**Remarks**

Gäller endast när egenskapen CategoryType är inställd på TimeScale.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setCategoryType(int value) {#setCategoryType-int-}
```
public void setCategoryType(int value)
```


Representerar typen av kategoriaxeln.

Se [CategoryType](../../com.aspose.cells/categorytype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setCrossAt(double value) {#setCrossAt-double-}
```
public void setCrossAt(double value)
```


Representerar punkten på värdeaxeln där kategoriaxeln korsar den.

**Remarks**

Numret ska vara ett heltal när det gäller kategori‑axeln. Och värdet måste ligga mellan 1 och 31999.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setCrossType(int value) {#setCrossType-int-}
```
public void setCrossType(int value)
```


Representerar [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) på den angivna axeln där den andra axeln korsar.

Se [CrossType](../../com.aspose.cells/crosstype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setCustUnit(int value) {#setCustUnit-int-}
```
public void setCustUnit(int value)
```


Anger ett anpassat värde för visningsenheten.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd i stället Axis.CustomUnit‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med januari 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setCustomDisplayUnit(double value) {#setCustomDisplayUnit-double-}
```
public void setCustomDisplayUnit(double value)
```


Anger ett anpassat värde för visningsenheten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setCustomUnit(int value) {#setCustomUnit-int-}
```
public void setCustomUnit(int value)
```


Anger ett anpassat värde för visningsenheten.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd i stället Axis.CustomDisplayUnit‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setDisplayUnit(int value) {#setDisplayUnit-int-}
```
public void setDisplayUnit(int value)
```


Representerar enhetsetiketten för den angivna axeln.

Se [DisplayUnitType](../../com.aspose.cells/displayunittype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setDisplayUnitLabelShown(boolean value) {#setDisplayUnitLabelShown-boolean-}
```
public void setDisplayUnitLabelShown(boolean value)
```


Representerar om display‑enhetsetiketten visas på den angivna axeln.

**Remarks**

Standardvärdet är True. Fungerar endast när [getDisplayUnit()](../../com.aspose.cells/axis\#getDisplayUnit--) inte är [DisplayUnitType.NONE](../../com.aspose.cells/displayunittype\#NONE).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHasMultiLevelLabels(boolean value) {#setHasMultiLevelLabels-boolean-}
```
public void setHasMultiLevelLabels(boolean value)
```


Indikerar om etiketterna ska visas som flernivå.

**Remarks**

Endast giltig för kategoriaxel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setLogBase(double value) {#setLogBase-double-}
```
public void setLogBase(double value)
```


Representerar den logaritmiska basen. Standardvärdet är 10.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setLogarithmic(boolean value) {#setLogarithmic-boolean-}
```
public void setLogarithmic(boolean value)
```


Representerar om värdeaxelns skaltyp är logaritmisk eller inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setMajorTickMark(int value) {#setMajorTickMark-int-}
```
public void setMajorTickMark(int value)
```


Representerar typen av huvudstämplar för den angivna axeln.

Se [TickMarkType](../../com.aspose.cells/tickmarktype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMajorUnit(double value) {#setMajorUnit-double-}
```
public void setMajorUnit(double value)
```


Representerar huvudenheterna för axeln.

**Remarks**

De stora enheterna måste vara större än noll.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setMajorUnitScale(int value) {#setMajorUnitScale-int-}
```
public void setMajorUnitScale(int value)
```


Representerar huvudenhetsskalan för kategoriaxeln.

Se [TimeUnit](../../com.aspose.cells/timeunit).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMaxValue(Object value) {#setMaxValue-java.lang.Object-}
```
public void setMaxValue(Object value)
```


Representerar det maximala värdet på värdeaxeln.

**Remarks**

Typen maxValue kan endast vara double eller DateTime

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object |  |

### setMinValue(Object value) {#setMinValue-java.lang.Object-}
```
public void setMinValue(Object value)
```


Representerar det minsta värdet på värdeaxeln.

**Remarks**

Typen minValue kan endast vara double eller DateTime

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object |  |

### setMinorTickMark(int value) {#setMinorTickMark-int-}
```
public void setMinorTickMark(int value)
```


Representerar typen av mindre stämplar för den angivna axeln.

Se [TickMarkType](../../com.aspose.cells/tickmarktype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMinorUnit(double value) {#setMinorUnit-double-}
```
public void setMinorUnit(double value)
```


Representerar de mindre enheterna för axeln.

**Remarks**

De mindre enheterna måste vara större än noll.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setMinorUnitScale(int value) {#setMinorUnitScale-int-}
```
public void setMinorUnitScale(int value)
```


Representerar huvudenhetsskalan för kategoriaxeln.

Se [TimeUnit](../../com.aspose.cells/timeunit).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPlotOrderReversed(boolean value) {#setPlotOrderReversed-boolean-}
```
public void setPlotOrderReversed(boolean value)
```


Representerar om Microsoft Excel ritar datapunkter från sista till första.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setTickLabelPosition(int value) {#setTickLabelPosition-int-}
```
public void setTickLabelPosition(int value)
```


Representerar positionen för stämplsetiketter på den angivna axeln.

Se [TickLabelPositionType](../../com.aspose.cells/ticklabelpositiontype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTickLabelSpacing(int value) {#setTickLabelSpacing-int-}
```
public void setTickLabelSpacing(int value)
```


Representerar antalet kategorier eller serier mellan tick‑mark‑etiketter. Gäller endast för kategori‑ och serieaxlar.

**Remarks**

Numret måste vara mellan 1 och 31999.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTickMarkSpacing(int value) {#setTickMarkSpacing-int-}
```
public void setTickMarkSpacing(int value)
```


Returnerar eller anger antalet kategorier eller serier mellan tick‑markeringar. Gäller endast för kategori‑ och serieaxlar.

**Remarks**

Numret måste vara mellan 1 och 31999.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Representerar om axeln är synlig.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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

