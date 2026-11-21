---
title: "Series"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar objektet som representerar en enskild dataserie i ett diagram."
type: docs
url: /sv/java/com.aspose.cells/series/
---

**Inheritance:**
java.lang.Object
```
public class Series
```

Inkapslar objektet som representerar en enskild dataserie i ett diagram.

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
         int seriesIndex = chart.getNSeries().add("A1:B4", true);
         //Setting the data source for the category data of NSeries
         chart.getNSeries().setCategoryData("C1:C4");
         Series series = chart.getNSeries().get(seriesIndex);
         //Setting the values of the series.
         series.setValues("=B1:B4");
         //Changing the chart type of the series.
         series.setType(ChartType.LINE);
         //Setting marker properties.
         series.getMarker().setMarkerStyle(ChartMarkerType.CIRCLE);
         series.getMarker().setForegroundColorSetType(FormattingType.AUTOMATIC);
         series.getMarker().setForegroundColor(com.aspose.cells.Color.getBlack());
         series.getMarker().setBackgroundColorSetType(FormattingType.AUTOMATIC);
 
         //do your business
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Representerar bakgrundsområdet för Series-objektet. |
| [getBar3DShapeType()](#getBar3DShapeType--) | Hämtar 3D-formtypen som används med 3D-stapeldiagram eller kolumndiagram. |
| [getBorder()](#getBorder--) | Representerar kanten på ett Series-objekt. |
| [getBubbleScale()](#getBubbleScale--) | Hämtar skalningsfaktorn för bubblor i den angivna diagramgruppen. |
| [getBubbleSizeRepresents()](#getBubbleSizeRepresents--) | Hämtar vad bubblstorleken representerar i ett bubbeldiagram. |
| [getBubbleSizes()](#getBubbleSizes--) | Hämtar bubblestorleksvärdena för diagramserien. |
| [getCachedCategoryValues()](#getCachedCategoryValues--) | Hämtar de cachade kategorivärdena för serien |
| [getCachedValues()](#getCachedValues--) | Hämtar de cachade värdena för serien |
| [getCategoryValues()](#getCategoryValues--) | Hämtar de faktiska kategorivärdena som används för att plotta varje punkt i denna serie i diagrammet. |
| [getClass()](#getClass--) |  |
| [getCountOfDataValues()](#getCountOfDataValues--) | Hämtar antalet datavärden. |
| [getDataLabels()](#getDataLabels--) | Representerar DataLabels-objektet för den angivna ASeries. |
| [getDisplayName()](#getDisplayName--) | Hämtar seriens namn som visas i diagramgrafen. |
| [getDoughnutHoleSize()](#getDoughnutHoleSize--) | Returnerar eller anger storleken på hålet i en donutdiagramgrupp. |
| [getDownBars()](#getDownBars--) | Returnerar ett [DropBars](../../com.aspose.cells/dropbars)-objekt som representerar nedårraderna i ett linjediagram. |
| [getDropLines()](#getDropLines--) | Returnerar ett [Line](../../com.aspose.cells/line)-objekt som representerar droplinjerna för en serie i ett linje- eller områdesdiagram. |
| [getExplosion()](#getExplosion--) | Avståndet för en öppen pajskiva från mitten av pajdiagrammet uttrycks som en procentandel av pajens diameter. |
| [getFirstSliceAngle()](#getFirstSliceAngle--) | Hämtar vinkeln på den första paj- eller munkdiagramdelen, i grader (medurs från vertikal). |
| [getGapWidth()](#getGapWidth--) | Returnerar eller anger avståndet mellan stapel‑ eller kolumnkluster, som en procentandel av stapelns eller kolumnens bredd. |
| [getHas3DEffect()](#getHas3DEffect--) | Sant om serien har ett tredimensionellt utseende. |
| [getHiLoLines()](#getHiLoLines--) | Returnerar ett HiLoLines-objekt som representerar hög-låg-linjerna för en serie i ett linjediagram. |
| [getLayoutProperties()](#getLayoutProperties--) | Representerar layoutens egenskaper. |
| [getLeaderLines()](#getLeaderLines--) | Representerar ledarlinjer i ett diagram. |
| [getLegendEntry()](#getLegendEntry--) | Hämtar förklaringsposten enligt denna serie. |
| [getMarker()](#getMarker--) | Hämtar [getMarker()](../../com.aspose.cells/series\#getMarker--). |
| [getName()](#getName--) | Hämtar namnet på dataserien. |
| [getOverlap()](#getOverlap--) | Anger hur staplar och kolumner placeras. |
| [getPlotOnSecondAxis()](#getPlotOnSecondAxis--) | Indikerar om denna serie plottas på den andra värdeaxeln. |
| [getPointValues()](#getPointValues--) | Hämtar de faktiska värdena som används för att plotta varje punkt i denna serie i diagrammet. |
| [getPoints()](#getPoints--) | Hämtar samlingen av punkter i en serie i ett diagram. |
| [getSecondPlotSize()](#getSecondPlotSize--) | Returnerar eller anger storleken på den sekundära delen av antingen ett paj‑paj‑diagram eller ett stapel‑paj‑diagram, som en procentandel av storleken på den primära pajen. |
| [getSeriesLines()](#getSeriesLines--) | Returnerar ett SeriesLines-objekt som representerar serielinjerna för ett staplat stapeldiagram eller ett staplat kolumndiagram. |
| [getShadow()](#getShadow--) | Sant om serien har en skugga. |
| [getShapeProperties()](#getShapeProperties--) | Hämtar [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)-objektet som innehåller de visuella formegenskaperna för serien. |
| [getShowNegativeBubbles()](#getShowNegativeBubbles--) | Sant om negativa bubblor visas för diagramgruppen. |
| [getSizeRepresents()](#getSizeRepresents--) | Hämtar vad bubblstorleken representerar i ett bubbeldiagram. |
| [getSmooth()](#getSmooth--) | Representerar kurvutjämning. |
| [getSplitType()](#getSplitType--) | Returnerar eller anger ett värde som bestämmer hur man avgör vilka datapunkter som finns i den andra pajen eller stapeln i ett paj‑i‑paj‑ eller stapel‑i‑paj‑diagram. |
| [getSplitValue()](#getSplitValue--) | Returnerar eller anger ett värde som ska användas för att bestämma vilka datapunkter som finns i den andra pajen eller stapeln i ett paj‑i‑paj‑ eller stapel‑i‑paj‑diagram. |
| [getTrendLines()](#getTrendLines--) | Returnerar alla trendlinjer för denna serie. |
| [getType()](#getType--) | Hämtar typen för en dataserie. |
| [getUpBars()](#getUpBars--) | Returnerar ett DropBars‑objekt som representerar uppåtriktade staplar i ett linjediagram. |
| [getValues()](#getValues--) | Representerar Y‑värdena för denna diagramserie. |
| [getValuesFormatCode()](#getValuesFormatCode--) | Representerar formatkoden för värdenas NumberList. |
| [getXErrorBar()](#getXErrorBar--) | Representerar felstapeln i X‑riktning för serien. |
| [getXValues()](#getXValues--) | Representerar X‑värdena för denna diagramserie. |
| [getXValuesFormatCode()](#getXValuesFormatCode--) | Representerar formatkoden för X‑värdenas NumberList. |
| [getYErrorBar()](#getYErrorBar--) | Representerar felstapeln i Y‑riktning för serien. |
| [hasDropLines()](#hasDropLines--) | Sant om diagrammet har droplinjer. |
| [hasHiLoLines()](#hasHiLoLines--) | Sant om linjediagrammet har hög‑låg‑linjer. |
| [hasLeaderLines()](#hasLeaderLines--) | Sant om serien har ledarlinjer. |
| [hasRadarAxisLabels()](#hasRadarAxisLabels--) | Sant om ett radardiagram har kategori‑axel‑etiketter. |
| [hasSeriesLines()](#hasSeriesLines--) | Sant om ett staplat kolumndiagram eller stapeldiagram har serielinjer eller om ett paj‑i‑paj‑diagram eller stapel‑i‑paj‑diagram har anslutningslinjer mellan de två sektionerna. |
| [hasUpDownBars()](#hasUpDownBars--) | Sant om ett linjediagram har upp‑ och nedstaplar. |
| [hashCode()](#hashCode--) |  |
| [isAutoSplit()](#isAutoSplit--) | Indikerar om tröskelvärdet är automatiskt. |
| [isColorVaried()](#isColorVaried--) | Representerar om färgen på punkterna varierar. |
| [isFiltered()](#isFiltered--) | Indikerar om serien är markerad eller filtrerad. |
| [isVerticalValues()](#isVerticalValues--) | Indikerar om datakällan är vertikal. |
| [move(int count)](#move-int-) | Flyttar serien upp eller ner. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBar3DShapeType(int value)](#setBar3DShapeType-int-) | Ställer in 3D‑formtypen som används med 3D‑stapeldiagram eller kolumndiagram. |
| [setBubbleScale(int value)](#setBubbleScale-int-) | Ställer in skalningsfaktorn för bubblor i den angivna diagramgruppen. |
| [setBubbleSizeRepresents(int value)](#setBubbleSizeRepresents-int-) | Hämtar vad bubblstorleken representerar i ett bubbeldiagram. |
| [setBubbleSizes(String value)](#setBubbleSizes-java.lang.String-) | Ställer in bubbelförstoringsvärdena för diagramserien. |
| [setColorVaried(boolean value)](#setColorVaried-boolean-) | Representerar om färgen på punkterna varierar. |
| [setDoughnutHoleSize(int value)](#setDoughnutHoleSize-int-) | Returnerar eller anger storleken på hålet i en donutdiagramgrupp. |
| [setExplosion(int value)](#setExplosion-int-) | Avståndet för en öppen pajskiva från mitten av pajdiagrammet uttrycks som en procentandel av pajens diameter. |
| [setFiltered(boolean value)](#setFiltered-boolean-) | Indikerar om serien är markerad eller filtrerad. |
| [setFirstSliceAngle(short value)](#setFirstSliceAngle-short-) | Ställer in vinkeln för den första sektorn i ett cirkeldiagram eller donutdiagram, i grader (medurs från vertikal). |
| [setGapWidth(short value)](#setGapWidth-short-) | Returnerar eller anger avståndet mellan stapel‑ eller kolumnkluster, som en procentandel av stapelns eller kolumnens bredd. |
| [setHas3DEffect(boolean value)](#setHas3DEffect-boolean-) | Sant om serien har ett tredimensionellt utseende. |
| [setHasDropLines(boolean value)](#setHasDropLines-boolean-) | Sant om diagrammet har droplinjer. |
| [setHasHiLoLines(boolean value)](#setHasHiLoLines-boolean-) | Sant om linjediagrammet har hög‑låg‑linjer. |
| [setHasLeaderLines(boolean value)](#setHasLeaderLines-boolean-) | Sant om serien har ledarlinjer. |
| [setHasRadarAxisLabels(boolean value)](#setHasRadarAxisLabels-boolean-) | Sant om ett radardiagram har kategori‑axel‑etiketter. |
| [setHasSeriesLines(boolean value)](#setHasSeriesLines-boolean-) | Sant om ett staplat kolumndiagram eller stapeldiagram har serielinjer eller om ett paj‑i‑paj‑diagram eller stapel‑i‑paj‑diagram har anslutningslinjer mellan de två sektionerna. |
| [setHasUpDownBars(boolean value)](#setHasUpDownBars-boolean-) | Sant om ett linjediagram har upp‑ och nedstaplar. |
| [setName(String value)](#setName-java.lang.String-) | Ställer in namnet på dataserien. |
| [setOverlap(short value)](#setOverlap-short-) | Anger hur staplar och kolumner placeras. |
| [setPlotOnSecondAxis(boolean value)](#setPlotOnSecondAxis-boolean-) | Indikerar om denna serie plottas på den andra värdeaxeln. |
| [setSecondPlotSize(short value)](#setSecondPlotSize-short-) | Returnerar eller anger storleken på den sekundära delen av antingen ett paj‑paj‑diagram eller ett stapel‑paj‑diagram, som en procentandel av storleken på den primära pajen. |
| [setShadow(boolean value)](#setShadow-boolean-) | Sant om serien har en skugga. |
| [setShowNegativeBubbles(boolean value)](#setShowNegativeBubbles-boolean-) | Sant om negativa bubblor visas för diagramgruppen. |
| [setSizeRepresents(int value)](#setSizeRepresents-int-) | Ställer in vad bubbelförstoringen representerar i ett bubbeldiagram. |
| [setSmooth(boolean value)](#setSmooth-boolean-) | Representerar kurvutjämning. |
| [setSplitType(int value)](#setSplitType-int-) | Returnerar eller anger ett värde som bestämmer hur man avgör vilka datapunkter som finns i den andra pajen eller stapeln i ett paj‑i‑paj‑ eller stapel‑i‑paj‑diagram. |
| [setSplitValue(double value)](#setSplitValue-double-) | Returnerar eller anger ett värde som ska användas för att bestämma vilka datapunkter som finns i den andra pajen eller stapeln i ett paj‑i‑paj‑ eller stapel‑i‑paj‑diagram. |
| [setType(int value)](#setType-int-) | Ställer in en dataserietyp. |
| [setValues(String value)](#setValues-java.lang.String-) | Representerar Y‑värdena för denna diagramserie. |
| [setValuesFormatCode(String value)](#setValuesFormatCode-java.lang.String-) | Representerar formatkoden för värdenas NumberList. |
| [setXValues(String value)](#setXValues-java.lang.String-) | Representerar X‑värdena för denna diagramserie. |
| [setXValuesFormatCode(String value)](#setXValuesFormatCode-java.lang.String-) | Representerar formatkoden för X‑värdenas NumberList. |
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


Representerar bakgrundsområdet för Series-objektet.

**Returns:**
[Area](../../com.aspose.cells/area)
### getBar3DShapeType() {#getBar3DShapeType--}
```
public int getBar3DShapeType()
```


Hämtar 3D-formtypen som används med 3D-stapeldiagram eller kolumndiagram.

Se [Bar3DShapeType](../../com.aspose.cells/bar3dshapetype).

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Representerar kanten på ett Series-objekt.

**Returns:**
[Line](../../com.aspose.cells/line)
### getBubbleScale() {#getBubbleScale--}
```
public int getBubbleScale()
```


Hämtar skalningsfaktorn för bubblor i den angivna diagramgruppen. Den kan vara ett heltal mellan 0 (noll) och 300, motsvarande en procentsats av standardstorleken. Gäller endast för bubbeldiagram.

**Returns:**
int
### getBubbleSizeRepresents() {#getBubbleSizeRepresents--}
```
public int getBubbleSizeRepresents()
```


Hämtar vad bubblstorleken representerar i ett bubbeldiagram.

Se [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen Aspose.Cells.Charts.Series.SizeRepresents. Denna egenskap kommer att tas bort 12 månader senare sedan JANUARI 2012. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getBubbleSizes() {#getBubbleSizes--}
```
public String getBubbleSizes()
```


Hämtar bubblestorleksvärdena för diagramserien.

**Remarks**

Endast för [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) eller [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Returns:**
java.lang.String
### getCachedCategoryValues() {#getCachedCategoryValues--}
```
public ArrayList getCachedCategoryValues()
```


Hämtar de cachade kategorivärdena för serien

**Remarks**

OBS: Denna egenskap är för närvarande endast för internt bruk. Den kommer att ändras eller tas bort i nästa version.

**Returns:**
java.util.ArrayList
### getCachedValues() {#getCachedValues--}
```
public ArrayList getCachedValues()
```


Hämtar de cachade värdena för serien

**Remarks**

OBS: Denna egenskap är för närvarande endast för internt bruk. Den kommer att ändras eller tas bort i nästa version.

**Returns:**
java.util.ArrayList
### getCategoryValues() {#getCategoryValues--}
```
public ChartDataValue[][] getCategoryValues()
```


Hämtar de faktiska kategorivärdena som används för att plotta varje punkt i denna serie i diagrammet.

**Remarks**

Denna egenskap ger ett bekvämt sätt att hämta de faktiska värdena som motsvarar data definierade av [getXValues()](../../com.aspose.cells/series\#getXValues--), särskilt när den angivna datakällan är en extern länk, formel, ...etc.

**Example**

```
         //Standalone example
         Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Chart chart = worksheet.getCharts().get(0);
         chart.calculate();
         String XValues = chart.getNSeries().get(0).getXValues();
         // XValues may be like "[External.xlsx]Sheet1!$B$2:$C$6" which is complicated
         // for user to get the actual values(the values may be linked to another workbook,
         // or cached in current workbook). Here you can use CategoryValues property
         // to get the category values actually displayed in the Excel interface
         // in the form of a two-dimensional array.
         ChartDataValue[][] v1 = chart.getNSeries().get(0).getCategoryValues();
```

**Returns:**
com.aspose.cells.ChartDataValue[][]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCountOfDataValues() {#getCountOfDataValues--}
```
public int getCountOfDataValues()
```


Hämtar antalet datavärden.

**Returns:**
int
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


Representerar DataLabels-objektet för den angivna ASeries.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Hämtar seriens namn som visas i diagramgrafen.

**Returns:**
java.lang.String
### getDoughnutHoleSize() {#getDoughnutHoleSize--}
```
public int getDoughnutHoleSize()
```


Returnerar eller anger storleken på hålet i en donutdiagramgrupp. Hålets storlek uttrycks som en procentsats av diagrammets storlek, mellan 10 och 90 procent.

**Returns:**
int
### getDownBars() {#getDownBars--}
```
public DropBars getDownBars()
```


Returnerar ett [DropBars](../../com.aspose.cells/dropbars) object som representerar down bars i ett linjediagram. Gäller endast för linjediagram.

**Returns:**
[DropBars](../../com.aspose.cells/dropbars)
### getDropLines() {#getDropLines--}
```
public Line getDropLines()
```


Returnerar ett [Line](../../com.aspose.cells/line) object som representerar droplinjer för en serie i ett linje- eller områdesdiagram. Gäller endast för linjediagram eller områdesdiagram.

**Returns:**
[Line](../../com.aspose.cells/line)
### getExplosion() {#getExplosion--}
```
public int getExplosion()
```


Avståndet för en öppen pajskiva från mitten av pajdiagrammet uttrycks som en procentandel av pajens diameter.

**Returns:**
int
### getFirstSliceAngle() {#getFirstSliceAngle--}
```
public short getFirstSliceAngle()
```


Hämtar vinkeln på den första paj- eller donut-diagramsegmentet, i grader (medurs från vertikal). Gäller endast för paj-, 3‑D‑paj- och donutdiagram, med värden från 0 till 360.

**Returns:**
short
### getGapWidth() {#getGapWidth--}
```
public short getGapWidth()
```


Returnerar eller anger utrymmet mellan stapel- eller kolumnkluster, som en procentandel av stapelns eller kolumnens bredd. Värdet för denna egenskap måste vara mellan 0 och 500.

**Returns:**
short
### getHas3DEffect() {#getHas3DEffect--}
```
public boolean getHas3DEffect()
```


Sant om serien har ett tredimensionellt utseende.

**Remarks**

Gäller endast för [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) eller [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D)-diagram.

**Returns:**
boolean
### getHiLoLines() {#getHiLoLines--}
```
public Line getHiLoLines()
```


Returnerar ett HiLoLines object som representerar hög-låg-linjer för en serie i ett linjediagram. Gäller endast för linjediagram.

**Returns:**
[Line](../../com.aspose.cells/line)
### getLayoutProperties() {#getLayoutProperties--}
```
public SeriesLayoutProperties getLayoutProperties()
```


Representerar layoutens egenskaper.

**Returns:**
[SeriesLayoutProperties](../../com.aspose.cells/serieslayoutproperties)
### getLeaderLines() {#getLeaderLines--}
```
public Line getLeaderLines()
```


Representerar ledarlinjer i ett diagram. Ledarlinjer kopplar datamärkningar till datapunkter. Detta objekt är inte en samling; det finns inget objekt som representerar en enskild ledarlinje.

**Returns:**
[Line](../../com.aspose.cells/line)
### getLegendEntry() {#getLegendEntry--}
```
public LegendEntry getLegendEntry()
```


Hämtar förklaringsposten enligt denna serie.

**Returns:**
[LegendEntry](../../com.aspose.cells/legendentry)
### getMarker() {#getMarker--}
```
public Marker getMarker()
```


Hämtar [getMarker()](../../com.aspose.cells/series\#getMarker--).

**Returns:**
[Marker](../../com.aspose.cells/marker)
### getName() {#getName--}
```
public String getName()
```


Hämtar namnet på dataserien.

**Example**

```
         //Reference name to a cell
         chart.getNSeries().get(0).setName("=A1");
 
         //Set a string to name
         chart.getNSeries().get(0).setName("First Series");
```

**Returns:**
java.lang.String
### getOverlap() {#getOverlap--}
```
public short getOverlap()
```


Anger hur staplar och kolumner placeras. Kan vara ett värde mellan -100 och 100. Gäller endast för 2‑D stapeldiagram och 2‑D kolumndiagram.

**Returns:**
short
### getPlotOnSecondAxis() {#getPlotOnSecondAxis--}
```
public boolean getPlotOnSecondAxis()
```


Indikerar om denna serie plottas på den andra värdeaxeln.

**Returns:**
boolean
### getPointValues() {#getPointValues--}
```
public ChartDataValue[] getPointValues()
```


Hämtar de faktiska värdena som används för att plotta varje punkt i denna serie i diagrammet.

**Remarks**

Denna egenskap ger ett bekvämt sätt att hämta de faktiska värdena som motsvarar data definierade av [getValues()](../../com.aspose.cells/series\#getValues--), särskilt när den angivna datakällan är en extern länk, formel, ...etc.

**Example**

```
         Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Chart chart = worksheet.getCharts().get(0);
         chart.calculate();
         String Values = chart.getNSeries().get(0).getValues();
         // Values could be like "[External.xlsx]Sheet1!$A$1:$A$6" which is complicated
         // for user to get the actual values(the values may be linked to another workbook,
         // or cached in current workbook). Here you can use PointValues property
         // to get the values actually displayed in the Excel interface
         // in the form of an array.
         ChartDataValue[] v1 = chart.getNSeries().get(0).getPointValues();
```

**Returns:**
com.aspose.cells.ChartDataValue[]
### getPoints() {#getPoints--}
```
public ChartPointCollection getPoints()
```


Hämtar samlingen av punkter i en serie i ett diagram.

**Remarks**

När diagrammet är Pie of Pie eller Bar of Pie är den sista punkten en annan punkt i den första pajplotten.

**Returns:**
[ChartPointCollection](../../com.aspose.cells/chartpointcollection)
### getSecondPlotSize() {#getSecondPlotSize--}
```
public short getSecondPlotSize()
```


Returnerar eller anger storleken på den sekundära delen av antingen ett pie of pie-diagram eller ett bar of pie-diagram, som en procentsats av storleken på den primära pajen. Kan vara ett värde mellan 5 och 200.

**Returns:**
short
### getSeriesLines() {#getSeriesLines--}
```
public Line getSeriesLines()
```


Returnerar ett SeriesLines object som representerar serielinjer för ett staplat stapeldiagram eller ett staplat kolumndiagram. Gäller endast för staplade stapel- och kolumndiagram.

**Returns:**
[Line](../../com.aspose.cells/line)
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Sant om serien har en skugga.

**Returns:**
boolean
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Hämtar [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)-objektet som innehåller de visuella formegenskaperna för serien.

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShowNegativeBubbles() {#getShowNegativeBubbles--}
```
public boolean getShowNegativeBubbles()
```


Sant om negativa bubblor visas för diagramgruppen. Gäller endast för bubbeldiagram.

**Returns:**
boolean
### getSizeRepresents() {#getSizeRepresents--}
```
public int getSizeRepresents()
```


Hämtar vad bubblstorleken representerar i ett bubbeldiagram.

Se [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

BubbleSizeRepresents.SizeIsArea betyder att värdet [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) är bubblans area. BubbleSizeRepresents.SizeIsWidth betyder att värdet [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) är bubblans bredd.

**Returns:**
int
### getSmooth() {#getSmooth--}
```
public boolean getSmooth()
```


Representerar kurvutjämning. Sant om kurvutjämning är aktiverad för linjediagrammet eller spridningsdiagrammet. Gäller endast för linjediagram och spridningsdiagram med linjer.

**Returns:**
boolean
### getSplitType() {#getSplitType--}
```
public int getSplitType()
```


Returnerar eller anger ett värde som bestämmer hur man avgör vilka datapunkter som finns i den andra pajen eller stapeln i ett paj‑i‑paj‑ eller stapel‑i‑paj‑diagram.

Se [ChartSplitType](../../com.aspose.cells/chartsplittype).

**Returns:**
int
### getSplitValue() {#getSplitValue--}
```
public double getSplitValue()
```


Returnerar eller anger ett värde som ska användas för att bestämma vilka datapunkter som finns i den andra pajen eller stapeln i ett paj‑i‑paj‑ eller stapel‑i‑paj‑diagram.

**Returns:**
double
### getTrendLines() {#getTrendLines--}
```
public TrendlineCollection getTrendLines()
```


Returnerar alla trendlinjer för denna serie.

**Returns:**
[TrendlineCollection](../../com.aspose.cells/trendlinecollection)
### getType() {#getType--}
```
public int getType()
```


Hämtar typen för en dataserie.

Se [ChartType](../../com.aspose.cells/charttype).

**Returns:**
int
### getUpBars() {#getUpBars--}
```
public DropBars getUpBars()
```


Returnerar ett DropBars-objekt som representerar uppåtriktade staplar i ett linjediagram. Gäller endast för linjediagram.

**Returns:**
[DropBars](../../com.aspose.cells/dropbars)
### getValues() {#getValues--}
```
public String getValues()
```


Representerar Y‑värdena för denna diagramserie.

**Remarks**

För att få de faktiska värdena (motsvarande varje punkt i denna serie) som definieras av denna egenskap, använd [getPointValues()](../../com.aspose.cells/series\#getPointValues--).

**Returns:**
java.lang.String
### getValuesFormatCode() {#getValuesFormatCode--}
```
public String getValuesFormatCode()
```


Representerar formatkoden för värdenas NumberList.

**Returns:**
java.lang.String
### getXErrorBar() {#getXErrorBar--}
```
public ErrorBar getXErrorBar()
```


Representerar felstapeln i X‑riktning för serien.

**Returns:**
[ErrorBar](../../com.aspose.cells/errorbar)
### getXValues() {#getXValues--}
```
public String getXValues()
```


Representerar X‑värdena för denna diagramserie.

**Remarks**

Endast för spridnings- och bubbeldiagram. Använd [SeriesCollection.getCategoryData()](../../com.aspose.cells/seriescollection\#getCategoryData--) för andra diagramtyper. [getCategoryValues()](../../com.aspose.cells/series\#getCategoryValues--) används för att hämta de faktiska kategorivärdena för denna serie.

**Returns:**
java.lang.String
### getXValuesFormatCode() {#getXValuesFormatCode--}
```
public String getXValuesFormatCode()
```


Representerar formatkoden för X‑värdenas NumberList.

**Returns:**
java.lang.String
### getYErrorBar() {#getYErrorBar--}
```
public ErrorBar getYErrorBar()
```


Representerar felstapeln i Y‑riktning för serien.

**Returns:**
[ErrorBar](../../com.aspose.cells/errorbar)
### hasDropLines() {#hasDropLines--}
```
public boolean hasDropLines()
```


Sant om diagrammet har droplinjer. Gäller endast för linjediagram eller områdesdiagram.

**Returns:**
boolean
### hasHiLoLines() {#hasHiLoLines--}
```
public boolean hasHiLoLines()
```


Sant om linjediagrammet har hög-låg-linjer. Gäller endast för linjediagram.

**Returns:**
boolean
### hasLeaderLines() {#hasLeaderLines--}
```
public boolean hasLeaderLines()
```


Sant om serien har ledarlinjer.

**Returns:**
boolean
### hasRadarAxisLabels() {#hasRadarAxisLabels--}
```
public boolean hasRadarAxisLabels()
```


Sant om ett radardiagram har kategorialetiketter på axeln. Gäller endast för radardiagram.

**Returns:**
boolean
### hasSeriesLines() {#hasSeriesLines--}
```
public boolean hasSeriesLines()
```


Sant om ett staplat kolumndiagram eller stapeldiagram har serielinjer eller om ett Pie of Pie-diagram eller Bar of Pie-diagram har anslutningslinjer mellan de två sektionerna. Gäller endast för staplade kolumndiagram, stapeldiagram, Pie of Pie-diagram eller Bar of Pie-diagram.

**Returns:**
boolean
### hasUpDownBars() {#hasUpDownBars--}
```
public boolean hasUpDownBars()
```


Sant om ett linjediagram har upp- och nedåtriktade staplar. Gäller endast för linjediagram.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoSplit() {#isAutoSplit--}
```
public boolean isAutoSplit()
```


Indikerar om tröskelvärdet är automatiskt.

**Returns:**
boolean
### isColorVaried() {#isColorVaried--}
```
public boolean isColorVaried()
```


Representerar om färgen på punkterna varierar. Diagrammet måste innehålla endast en serie eller så är diagrammet ett cirkeldiagram.

**Returns:**
boolean
### isFiltered() {#isFiltered--}
```
public boolean isFiltered()
```


Indikerar om serien är markerad eller filtrerad. Sant betyder att denna serie är filtrerad och den kommer inte att visas i diagrammet.

**Returns:**
boolean
### isVerticalValues() {#isVerticalValues--}
```
public boolean isVerticalValues()
```


Indikerar om datakällan är vertikal.

**Returns:**
boolean
### move(int count) {#move-int-}
```
public void move(int count)
```


Flyttar serien upp eller ner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| antal | int | Antalet steg upp eller ner. Flytta serien uppåt om detta är mindre än noll; flytta serien nedåt om detta är större än noll. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBar3DShapeType(int value) {#setBar3DShapeType-int-}
```
public void setBar3DShapeType(int value)
```


Ställer in 3D‑formtypen som används med 3D‑stapeldiagram eller kolumndiagram.

Se [Bar3DShapeType](../../com.aspose.cells/bar3dshapetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setBubbleScale(int value) {#setBubbleScale-int-}
```
public void setBubbleScale(int value)
```


Ställer in skalningsfaktorn för bubblor i den angivna diagramgruppen. Det kan vara ett heltal från 0 (noll) till 300, vilket motsvarar en procentandel av standardstorleken. Gäller endast för bubbeldiagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setBubbleSizeRepresents(int value) {#setBubbleSizeRepresents-int-}
```
public void setBubbleSizeRepresents(int value)
```


Hämtar vad bubblstorleken representerar i ett bubbeldiagram.

Se [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen Aspose.Cells.Charts.Series.SizeRepresents. Denna egenskap kommer att tas bort 12 månader senare sedan JANUARI 2012. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setBubbleSizes(String value) {#setBubbleSizes-java.lang.String-}
```
public void setBubbleSizes(String value)
```


Ställer in bubbelförstoringsvärdena för diagramserien.

**Remarks**

Endast för [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) eller [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setColorVaried(boolean value) {#setColorVaried-boolean-}
```
public void setColorVaried(boolean value)
```


Representerar om färgen på punkterna varierar. Diagrammet måste innehålla endast en serie eller så är diagrammet ett cirkeldiagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDoughnutHoleSize(int value) {#setDoughnutHoleSize-int-}
```
public void setDoughnutHoleSize(int value)
```


Returnerar eller anger storleken på hålet i en donutdiagramgrupp. Hålets storlek uttrycks som en procentsats av diagrammets storlek, mellan 10 och 90 procent.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setExplosion(int value) {#setExplosion-int-}
```
public void setExplosion(int value)
```


Avståndet för en öppen pajskiva från mitten av pajdiagrammet uttrycks som en procentandel av pajens diameter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setFiltered(boolean value) {#setFiltered-boolean-}
```
public void setFiltered(boolean value)
```


Indikerar om serien är markerad eller filtrerad. Sant betyder att denna serie är filtrerad och den kommer inte att visas i diagrammet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFirstSliceAngle(short value) {#setFirstSliceAngle-short-}
```
public void setFirstSliceAngle(short value)
```


Ställer in vinkeln för den första sektorn i ett cirkel- eller munkdiagram, i grader (medurs från vertikalen). Gäller endast för cirkel-, 3‑D‑cirkel- och munkdiagram, med värden från 0 till 360.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | short |  |

### setGapWidth(short value) {#setGapWidth-short-}
```
public void setGapWidth(short value)
```


Returnerar eller anger utrymmet mellan stapel- eller kolumnkluster, som en procentandel av stapelns eller kolumnens bredd. Värdet för denna egenskap måste vara mellan 0 och 500.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | short |  |

### setHas3DEffect(boolean value) {#setHas3DEffect-boolean-}
```
public void setHas3DEffect(boolean value)
```


Sant om serien har ett tredimensionellt utseende.

**Remarks**

Gäller endast för [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) eller [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D)-diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHasDropLines(boolean value) {#setHasDropLines-boolean-}
```
public void setHasDropLines(boolean value)
```


Sant om diagrammet har droplinjer. Gäller endast för linjediagram eller områdesdiagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHasHiLoLines(boolean value) {#setHasHiLoLines-boolean-}
```
public void setHasHiLoLines(boolean value)
```


Sant om linjediagrammet har hög-låg-linjer. Gäller endast för linjediagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHasLeaderLines(boolean value) {#setHasLeaderLines-boolean-}
```
public void setHasLeaderLines(boolean value)
```


Sant om serien har ledarlinjer.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHasRadarAxisLabels(boolean value) {#setHasRadarAxisLabels-boolean-}
```
public void setHasRadarAxisLabels(boolean value)
```


Sant om ett radardiagram har kategorialetiketter på axeln. Gäller endast för radardiagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHasSeriesLines(boolean value) {#setHasSeriesLines-boolean-}
```
public void setHasSeriesLines(boolean value)
```


Sant om ett staplat kolumndiagram eller stapeldiagram har serielinjer eller om ett Pie of Pie-diagram eller Bar of Pie-diagram har anslutningslinjer mellan de två sektionerna. Gäller endast för staplade kolumndiagram, stapeldiagram, Pie of Pie-diagram eller Bar of Pie-diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHasUpDownBars(boolean value) {#setHasUpDownBars-boolean-}
```
public void setHasUpDownBars(boolean value)
```


Sant om ett linjediagram har upp- och nedåtriktade staplar. Gäller endast för linjediagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Ställer in namnet på dataserien.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOverlap(short value) {#setOverlap-short-}
```
public void setOverlap(short value)
```


Anger hur staplar och kolumner placeras. Kan vara ett värde mellan -100 och 100. Gäller endast för 2‑D stapeldiagram och 2‑D kolumndiagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | short |  |

### setPlotOnSecondAxis(boolean value) {#setPlotOnSecondAxis-boolean-}
```
public void setPlotOnSecondAxis(boolean value)
```


Indikerar om denna serie plottas på den andra värdeaxeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSecondPlotSize(short value) {#setSecondPlotSize-short-}
```
public void setSecondPlotSize(short value)
```


Returnerar eller anger storleken på den sekundära delen av antingen ett pie of pie-diagram eller ett bar of pie-diagram, som en procentsats av storleken på den primära pajen. Kan vara ett värde mellan 5 och 200.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | short |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Sant om serien har en skugga.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowNegativeBubbles(boolean value) {#setShowNegativeBubbles-boolean-}
```
public void setShowNegativeBubbles(boolean value)
```


Sant om negativa bubblor visas för diagramgruppen. Gäller endast för bubbeldiagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSizeRepresents(int value) {#setSizeRepresents-int-}
```
public void setSizeRepresents(int value)
```


Ställer in vad bubbelförstoringen representerar i ett bubbeldiagram.

Se [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

BubbleSizeRepresents.SizeIsArea betyder att värdet [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) är bubblans area. BubbleSizeRepresents.SizeIsWidth betyder att värdet [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) är bubblans bredd.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSmooth(boolean value) {#setSmooth-boolean-}
```
public void setSmooth(boolean value)
```


Representerar kurvutjämning. Sant om kurvutjämning är aktiverad för linjediagrammet eller spridningsdiagrammet. Gäller endast för linjediagram och spridningsdiagram med linjer.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSplitType(int value) {#setSplitType-int-}
```
public void setSplitType(int value)
```


Returnerar eller anger ett värde som bestämmer hur man avgör vilka datapunkter som finns i den andra pajen eller stapeln i ett paj‑i‑paj‑ eller stapel‑i‑paj‑diagram.

Se [ChartSplitType](../../com.aspose.cells/chartsplittype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSplitValue(double value) {#setSplitValue-double-}
```
public void setSplitValue(double value)
```


Returnerar eller anger ett värde som ska användas för att bestämma vilka datapunkter som finns i den andra pajen eller stapeln i ett paj‑i‑paj‑ eller stapel‑i‑paj‑diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Ställer in en dataserietyp.

Se [ChartType](../../com.aspose.cells/charttype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setValues(String value) {#setValues-java.lang.String-}
```
public void setValues(String value)
```


Representerar Y‑värdena för denna diagramserie.

**Remarks**

För att få de faktiska värdena (motsvarande varje punkt i denna serie) som definieras av denna egenskap, använd [getPointValues()](../../com.aspose.cells/series\#getPointValues--).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setValuesFormatCode(String value) {#setValuesFormatCode-java.lang.String-}
```
public void setValuesFormatCode(String value)
```


Representerar formatkoden för värdenas NumberList.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setXValues(String value) {#setXValues-java.lang.String-}
```
public void setXValues(String value)
```


Representerar X‑värdena för denna diagramserie.

**Remarks**

Endast för spridnings- och bubbeldiagram. Använd [SeriesCollection.getCategoryData()](../../com.aspose.cells/seriescollection\#getCategoryData--) för andra diagramtyper. [getCategoryValues()](../../com.aspose.cells/series\#getCategoryValues--) används för att hämta de faktiska kategorivärdena för denna serie.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setXValuesFormatCode(String value) {#setXValuesFormatCode-java.lang.String-}
```
public void setXValuesFormatCode(String value)
```


Representerar formatkoden för X‑värdenas NumberList.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

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

