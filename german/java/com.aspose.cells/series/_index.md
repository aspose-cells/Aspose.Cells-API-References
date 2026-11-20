---
title: "Series"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Objekt, das eine einzelne Datenreihe in einem Diagramm darstellt."
type: docs
url: /de/java/com.aspose.cells/series/
---

**Inheritance:**
java.lang.Object
```
public class Series
```

Kapselt das Objekt, das eine einzelne Datenreihe in einem Diagramm darstellt.

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
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Stellt den Hintergrundbereich des Series-Objekts dar. |
| [getBar3DShapeType()](#getBar3DShapeType--) | Liefert den 3D-Formtyp, der mit dem 3‑D‑Balken‑ oder Säulendiagramm verwendet wird. |
| [getBorder()](#getBorder--) | Stellt den Rand eines Series-Objekts dar. |
| [getBubbleScale()](#getBubbleScale--) | Liefert den Skalierungsfaktor für Blasen in der angegebenen Diagrammgruppe. |
| [getBubbleSizeRepresents()](#getBubbleSizeRepresents--) | Liefert, was die Blasengröße in einem Blasendiagramm darstellt. |
| [getBubbleSizes()](#getBubbleSizes--) | Liefert die Blasengrößenwerte der Diagrammserie. |
| [getCachedCategoryValues()](#getCachedCategoryValues--) | Liefert die zwischengespeicherten Kategorienwerte für die Serie |
| [getCachedValues()](#getCachedValues--) | Liefert die zwischengespeicherten Werte für die Serie |
| [getCategoryValues()](#getCategoryValues--) | Liefert die tatsächlichen Kategorienwerte, die zum Plotten jedes Punktes dieser Serie im Diagramm verwendet werden. |
| [getClass()](#getClass--) |  |
| [getCountOfDataValues()](#getCountOfDataValues--) | Liefert die Anzahl der Datenwerte. |
| [getDataLabels()](#getDataLabels--) | Stellt das DataLabels-Objekt für die angegebene ASeries dar. |
| [getDisplayName()](#getDisplayName--) | Liefert den Namen der Serie, der im Diagramm angezeigt wird. |
| [getDoughnutHoleSize()](#getDoughnutHoleSize--) | Gibt die Größe des Lochs in einer Donut-Diagrammgruppe zurück oder legt sie fest. |
| [getDownBars()](#getDownBars--) | Gibt ein [DropBars](../../com.aspose.cells/dropbars)-Objekt zurück, das die Abwärtsbalken in einem Liniendiagramm darstellt. |
| [getDropLines()](#getDropLines--) | Gibt ein [Line](../../com.aspose.cells/line)-Objekt zurück, das die Falllinien für eine Serie im Liniendiagramm oder Flächendiagramm darstellt. |
| [getExplosion()](#getExplosion--) | Der Abstand eines offenen Kuchensegments vom Zentrum des Kuchendiagramms wird als Prozentsatz des Durchmessers des Kuchens angegeben. |
| [getFirstSliceAngle()](#getFirstSliceAngle--) | Ruft den Winkel des ersten Kuchen- oder Donut-Diagrammsegments in Grad ab (im Uhrzeigersinn von vertikal aus). |
| [getGapWidth()](#getGapWidth--) | Gibt den Abstand zwischen Balken‑ oder Säulen‑Clustern zurück oder setzt ihn, als Prozentsatz der Balken‑ oder Säulenbreite. |
| [getHas3DEffect()](#getHas3DEffect--) | Wahr, wenn die Serie ein dreidimensionales Erscheinungsbild hat. |
| [getHiLoLines()](#getHiLoLines--) | Gibt ein HiLoLines-Objekt zurück, das die Hoch‑Niedrig‑Linien für eine Serie in einem Liniendiagramm darstellt. |
| [getLayoutProperties()](#getLayoutProperties--) | Stellt die Eigenschaften des Layouts dar. |
| [getLeaderLines()](#getLeaderLines--) | Stellt Führungslinien in einem Diagramm dar. |
| [getLegendEntry()](#getLegendEntry--) | Liefert den Legendeeintrag gemäß dieser Serie. |
| [getMarker()](#getMarker--) | Liefert die [getMarker()](../../com.aspose.cells/series\#getMarker--). |
| [getName()](#getName--) | Liest den Namen der Datenreihe. |
| [getOverlap()](#getOverlap--) | Gibt an, wie Balken und Säulen positioniert werden. |
| [getPlotOnSecondAxis()](#getPlotOnSecondAxis--) | Zeigt an, ob diese Reihe auf der zweiten Werteachse dargestellt wird. |
| [getPointValues()](#getPointValues--) | Liest die tatsächlichen Werte, die zum Plotten jedes Punktes dieser Reihe im Diagramm verwendet werden. |
| [getPoints()](#getPoints--) | Liest die Sammlung von Punkten in einer Reihe eines Diagramms. |
| [getSecondPlotSize()](#getSecondPlotSize--) | Gibt die Größe des sekundären Abschnitts eines Kreis‑im‑Kreis‑Diagramms oder Balken‑im‑Kreis‑Diagramms zurück oder legt sie fest, als Prozentsatz der Größe des primären Kreises. |
| [getSeriesLines()](#getSeriesLines--) | Gibt ein SeriesLines‑Objekt zurück, das die Serienlinien für ein gestapeltes Balken‑ oder Säulendiagramm darstellt. |
| [getShadow()](#getShadow--) | True, wenn die Serie einen Schatten hat. |
| [getShapeProperties()](#getShapeProperties--) | Liest das [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)-Objekt, das die visuellen Formeigenschaften der Serie enthält. |
| [getShowNegativeBubbles()](#getShowNegativeBubbles--) | True, wenn negative Blasen für die Diagrammgruppe angezeigt werden. |
| [getSizeRepresents()](#getSizeRepresents--) | Liefert, was die Blasengröße in einem Blasendiagramm darstellt. |
| [getSmooth()](#getSmooth--) | Stellt die Kurvenglättung dar. |
| [getSplitType()](#getSplitType--) | Gibt einen Wert zurück oder legt ihn fest, der bestimmt, welche Datenpunkte im zweiten Kreis oder Balken eines Kreis‑im‑Kreis‑ bzw. Balken‑im‑Kreis‑Diagramms liegen. |
| [getSplitValue()](#getSplitValue--) | Gibt einen Wert zurück oder legt ihn fest, der zur Bestimmung verwendet wird, welche Datenpunkte im zweiten Kreis oder Balken eines Kreis‑im‑Kreis‑ bzw. Balken‑im‑Kreis‑Diagramms liegen. |
| [getTrendLines()](#getTrendLines--) | Gibt alle Trendlinien dieser Serie zurück. |
| [getType()](#getType--) | Liest den Typ einer Datenreihe. |
| [getUpBars()](#getUpBars--) | Gibt ein DropBars‑Objekt zurück, das die Aufwärtsbalken in einem Liniendiagramm darstellt. |
| [getValues()](#getValues--) | Stellt die Y‑Werte dieser Diagrammreihe dar. |
| [getValuesFormatCode()](#getValuesFormatCode--) | Stellt den Formatcode der Werte‑NumberList dar. |
| [getXErrorBar()](#getXErrorBar--) | Stellt die X‑Richtungs-Fehlerbalken der Serie dar. |
| [getXValues()](#getXValues--) | Stellt die X‑Werte dieser Diagrammreihe dar. |
| [getXValuesFormatCode()](#getXValuesFormatCode--) | Stellt den Formatcode der X‑Werte‑NumberList dar. |
| [getYErrorBar()](#getYErrorBar--) | Stellt die Y‑Richtungs-Fehlerbalken der Serie dar. |
| [hasDropLines()](#hasDropLines--) | True, wenn das Diagramm Falllinien hat. |
| [hasHiLoLines()](#hasHiLoLines--) | True, wenn das Liniendiagramm Hoch‑Tief‑Linien hat. |
| [hasLeaderLines()](#hasLeaderLines--) | True, wenn die Serie Führungslinien hat. |
| [hasRadarAxisLabels()](#hasRadarAxisLabels--) | Wahr, wenn ein Radar-Diagramm Kategorienachsenbeschriftungen hat. |
| [hasSeriesLines()](#hasSeriesLines--) | Wahr, wenn ein gestapeltes Säulen‑Diagramm oder Balken‑Diagramm Serienlinien hat oder wenn ein Pie‑of‑Pie‑Diagramm oder Bar‑of‑Pie‑Diagramm Verbindungslinien zwischen den beiden Abschnitten hat. |
| [hasUpDownBars()](#hasUpDownBars--) | Wahr, wenn ein Liniendiagramm Auf‑ und Ab‑Balken hat. |
| [hashCode()](#hashCode--) |  |
| [isAutoSplit()](#isAutoSplit--) | Gibt an, ob der Schwellenwert automatisch ist. |
| [isColorVaried()](#isColorVaried--) | Gibt an, ob die Farbe der Punkte variiert wird. |
| [isFiltered()](#isFiltered--) | Gibt an, ob die Serie ausgewählt oder gefiltert ist. |
| [isVerticalValues()](#isVerticalValues--) | Gibt an, ob die Datenquelle vertikal ist. |
| [move(int count)](#move-int-) | Verschiebt die Serie nach oben oder unten. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBar3DShapeType(int value)](#setBar3DShapeType-int-) | Legt den 3D‑Formtyp fest, der mit dem 3‑D‑Balken‑ oder Säulendiagramm verwendet wird. |
| [setBubbleScale(int value)](#setBubbleScale-int-) | Legt den Skalierungsfaktor für Blasen in der angegebenen Diagrammgruppe fest. |
| [setBubbleSizeRepresents(int value)](#setBubbleSizeRepresents-int-) | Liefert, was die Blasengröße in einem Blasendiagramm darstellt. |
| [setBubbleSizes(String value)](#setBubbleSizes-java.lang.String-) | Legt die Blasengrößenwerte der Diagrammserie fest. |
| [setColorVaried(boolean value)](#setColorVaried-boolean-) | Gibt an, ob die Farbe der Punkte variiert wird. |
| [setDoughnutHoleSize(int value)](#setDoughnutHoleSize-int-) | Gibt die Größe des Lochs in einer Donut-Diagrammgruppe zurück oder legt sie fest. |
| [setExplosion(int value)](#setExplosion-int-) | Der Abstand eines offenen Kuchensegments vom Zentrum des Kuchendiagramms wird als Prozentsatz des Durchmessers des Kuchens angegeben. |
| [setFiltered(boolean value)](#setFiltered-boolean-) | Gibt an, ob die Serie ausgewählt oder gefiltert ist. |
| [setFirstSliceAngle(short value)](#setFirstSliceAngle-short-) | Legt den Winkel des ersten Kuchendiagramm‑ oder Donutdiagramm‑Scheibchens in Grad fest (im Uhrzeigersinn von vertikal aus). |
| [setGapWidth(short value)](#setGapWidth-short-) | Gibt den Abstand zwischen Balken‑ oder Säulen‑Clustern zurück oder setzt ihn, als Prozentsatz der Balken‑ oder Säulenbreite. |
| [setHas3DEffect(boolean value)](#setHas3DEffect-boolean-) | Wahr, wenn die Serie ein dreidimensionales Erscheinungsbild hat. |
| [setHasDropLines(boolean value)](#setHasDropLines-boolean-) | True, wenn das Diagramm Falllinien hat. |
| [setHasHiLoLines(boolean value)](#setHasHiLoLines-boolean-) | True, wenn das Liniendiagramm Hoch‑Tief‑Linien hat. |
| [setHasLeaderLines(boolean value)](#setHasLeaderLines-boolean-) | True, wenn die Serie Führungslinien hat. |
| [setHasRadarAxisLabels(boolean value)](#setHasRadarAxisLabels-boolean-) | Wahr, wenn ein Radar-Diagramm Kategorienachsenbeschriftungen hat. |
| [setHasSeriesLines(boolean value)](#setHasSeriesLines-boolean-) | Wahr, wenn ein gestapeltes Säulen‑Diagramm oder Balken‑Diagramm Serienlinien hat oder wenn ein Pie‑of‑Pie‑Diagramm oder Bar‑of‑Pie‑Diagramm Verbindungslinien zwischen den beiden Abschnitten hat. |
| [setHasUpDownBars(boolean value)](#setHasUpDownBars-boolean-) | Wahr, wenn ein Liniendiagramm Auf‑ und Ab‑Balken hat. |
| [setName(String value)](#setName-java.lang.String-) | Legt den Namen der Datenserie fest. |
| [setOverlap(short value)](#setOverlap-short-) | Gibt an, wie Balken und Säulen positioniert werden. |
| [setPlotOnSecondAxis(boolean value)](#setPlotOnSecondAxis-boolean-) | Zeigt an, ob diese Reihe auf der zweiten Werteachse dargestellt wird. |
| [setSecondPlotSize(short value)](#setSecondPlotSize-short-) | Gibt die Größe des sekundären Abschnitts eines Kreis‑im‑Kreis‑Diagramms oder Balken‑im‑Kreis‑Diagramms zurück oder legt sie fest, als Prozentsatz der Größe des primären Kreises. |
| [setShadow(boolean value)](#setShadow-boolean-) | True, wenn die Serie einen Schatten hat. |
| [setShowNegativeBubbles(boolean value)](#setShowNegativeBubbles-boolean-) | True, wenn negative Blasen für die Diagrammgruppe angezeigt werden. |
| [setSizeRepresents(int value)](#setSizeRepresents-int-) | Legt fest, was die Blasengröße in einem Blasendiagramm darstellt. |
| [setSmooth(boolean value)](#setSmooth-boolean-) | Stellt die Kurvenglättung dar. |
| [setSplitType(int value)](#setSplitType-int-) | Gibt einen Wert zurück oder legt ihn fest, der bestimmt, welche Datenpunkte im zweiten Kreis oder Balken eines Kreis‑im‑Kreis‑ bzw. Balken‑im‑Kreis‑Diagramms liegen. |
| [setSplitValue(double value)](#setSplitValue-double-) | Gibt einen Wert zurück oder legt ihn fest, der zur Bestimmung verwendet wird, welche Datenpunkte im zweiten Kreis oder Balken eines Kreis‑im‑Kreis‑ bzw. Balken‑im‑Kreis‑Diagramms liegen. |
| [setType(int value)](#setType-int-) | Legt den Typ einer Datenserie fest. |
| [setValues(String value)](#setValues-java.lang.String-) | Stellt die Y‑Werte dieser Diagrammreihe dar. |
| [setValuesFormatCode(String value)](#setValuesFormatCode-java.lang.String-) | Stellt den Formatcode der Werte‑NumberList dar. |
| [setXValues(String value)](#setXValues-java.lang.String-) | Stellt die X‑Werte dieser Diagrammreihe dar. |
| [setXValuesFormatCode(String value)](#setXValuesFormatCode-java.lang.String-) | Stellt den Formatcode der X‑Werte‑NumberList dar. |
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
### getArea() {#getArea--}
```
public Area getArea()
```


Stellt den Hintergrundbereich des Series-Objekts dar.

**Returns:**
[Area](../../com.aspose.cells/area)
### getBar3DShapeType() {#getBar3DShapeType--}
```
public int getBar3DShapeType()
```


Liefert den 3D-Formtyp, der mit dem 3‑D‑Balken‑ oder Säulendiagramm verwendet wird.

Siehe [Bar3DShapeType](../../com.aspose.cells/bar3dshapetype).

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Stellt den Rand eines Series-Objekts dar.

**Returns:**
[Line](../../com.aspose.cells/line)
### getBubbleScale() {#getBubbleScale--}
```
public int getBubbleScale()
```


Liefert den Skalierungsfaktor für Blasen in der angegebenen Diagrammgruppe. Er kann ein ganzzahliger Wert von 0 (null) bis 300 sein, was einem Prozentsatz der Standardgröße entspricht. Gilt nur für Blasendiagramme.

**Returns:**
int
### getBubbleSizeRepresents() {#getBubbleSizeRepresents--}
```
public int getBubbleSizeRepresents()
```


Liefert, was die Blasengröße in einem Blasendiagramm darstellt.

Siehe [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft Aspose.Cells.Charts.Series.SizeRepresents. Diese Eigenschaft wird 12 Monate nach JANUAR 2012 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben könnten.

**Returns:**
int
### getBubbleSizes() {#getBubbleSizes--}
```
public String getBubbleSizes()
```


Liefert die Blasengrößenwerte der Diagrammserie.

**Remarks**

Nur für [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) oder [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Returns:**
java.lang.String
### getCachedCategoryValues() {#getCachedCategoryValues--}
```
public ArrayList getCachedCategoryValues()
```


Liefert die zwischengespeicherten Kategorienwerte für die Serie

**Remarks**

HINWEIS: Diese Eigenschaft ist derzeit nur für den internen Gebrauch bestimmt. Sie wird in der nächsten Version geändert oder entfernt werden.

**Returns:**
java.util.ArrayList
### getCachedValues() {#getCachedValues--}
```
public ArrayList getCachedValues()
```


Liefert die zwischengespeicherten Werte für die Serie

**Remarks**

HINWEIS: Diese Eigenschaft ist derzeit nur für den internen Gebrauch bestimmt. Sie wird in der nächsten Version geändert oder entfernt werden.

**Returns:**
java.util.ArrayList
### getCategoryValues() {#getCategoryValues--}
```
public ChartDataValue[][] getCategoryValues()
```


Liefert die tatsächlichen Kategorienwerte, die zum Plotten jedes Punktes dieser Serie im Diagramm verwendet werden.

**Remarks**

Diese Eigenschaft bietet eine bequeme Möglichkeit, die tatsächlichen Werte zu erhalten, die den durch [getXValues()](../../com.aspose.cells/series\#getXValues--) definierten Daten entsprechen, insbesondere wenn die angegebene Datenquelle ein externer Link, eine Formel usw. ist.

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


Liefert die Anzahl der Datenwerte.

**Returns:**
int
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


Stellt das DataLabels-Objekt für die angegebene ASeries dar.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Liefert den Namen der Serie, der im Diagramm angezeigt wird.

**Returns:**
java.lang.String
### getDoughnutHoleSize() {#getDoughnutHoleSize--}
```
public int getDoughnutHoleSize()
```


Gibt die Größe des Lochs in einer Donut‑Diagrammgruppe zurück oder legt sie fest. Die Lochgröße wird als Prozentsatz der Diagrammgröße angegeben, zwischen 10 % und 90 %.

**Returns:**
int
### getDownBars() {#getDownBars--}
```
public DropBars getDownBars()
```


Gibt ein [DropBars](../../com.aspose.cells/dropbars)-Objekt zurück, das die Abwärtsbalken in einem Liniendiagramm darstellt. Gilt nur für Liniendiagramme.

**Returns:**
[DropBars](../../com.aspose.cells/dropbars)
### getDropLines() {#getDropLines--}
```
public Line getDropLines()
```


Gibt ein [Line](../../com.aspose.cells/line)-Objekt zurück, das die Verbindungslinien für eine Serie im Liniendiagramm oder Flächendiagramm darstellt. Gilt nur für Liniendiagramme oder Flächendiagramme.

**Returns:**
[Line](../../com.aspose.cells/line)
### getExplosion() {#getExplosion--}
```
public int getExplosion()
```


Der Abstand eines offenen Kuchensegments vom Zentrum des Kuchendiagramms wird als Prozentsatz des Durchmessers des Kuchens angegeben.

**Returns:**
int
### getFirstSliceAngle() {#getFirstSliceAngle--}
```
public short getFirstSliceAngle()
```


Ermittelt den Winkel des ersten Kuchen- oder Donut-Diagrammsegments in Grad (im Uhrzeigersinn von vertikal aus). Gilt nur für Kuchen-, 3‑D‑Kuchen- und Donutdiagramme mit Werten von 0 bis 360.

**Returns:**
short
### getGapWidth() {#getGapWidth--}
```
public short getGapWidth()
```


Gibt den Abstand zwischen Balken‑ oder Säulen‑Clustern zurück oder legt ihn fest, als Prozentsatz der Balken‑ oder Säulenbreite. Der Wert dieser Property muss zwischen 0 und 500 liegen.

**Returns:**
short
### getHas3DEffect() {#getHas3DEffect--}
```
public boolean getHas3DEffect()
```


Wahr, wenn die Serie ein dreidimensionales Erscheinungsbild hat.

**Remarks**

Gilt nur für [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) oder [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D) Diagramme.

**Returns:**
boolean
### getHiLoLines() {#getHiLoLines--}
```
public Line getHiLoLines()
```


Gibt ein HiLoLines‑Objekt zurück, das die Hoch‑Niedrig‑Linien für eine Serie in einem Liniendiagramm darstellt. Gilt nur für Liniendiagramme.

**Returns:**
[Line](../../com.aspose.cells/line)
### getLayoutProperties() {#getLayoutProperties--}
```
public SeriesLayoutProperties getLayoutProperties()
```


Stellt die Eigenschaften des Layouts dar.

**Returns:**
[SeriesLayoutProperties](../../com.aspose.cells/serieslayoutproperties)
### getLeaderLines() {#getLeaderLines--}
```
public Line getLeaderLines()
```


Stellt Führungs‑Linien in einem Diagramm dar. Führungs‑Linien verbinden Datenbeschriftungen mit Datenpunkten. Dieses Objekt ist keine Sammlung; es gibt kein Objekt, das eine einzelne Führungs‑Linie darstellt.

**Returns:**
[Line](../../com.aspose.cells/line)
### getLegendEntry() {#getLegendEntry--}
```
public LegendEntry getLegendEntry()
```


Liefert den Legendeeintrag gemäß dieser Serie.

**Returns:**
[LegendEntry](../../com.aspose.cells/legendentry)
### getMarker() {#getMarker--}
```
public Marker getMarker()
```


Liefert die [getMarker()](../../com.aspose.cells/series\#getMarker--).

**Returns:**
[Marker](../../com.aspose.cells/marker)
### getName() {#getName--}
```
public String getName()
```


Liest den Namen der Datenreihe.

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


Gibt an, wie Balken und Säulen positioniert werden. Kann ein Wert zwischen -100 und 100 sein. Gilt nur für 2‑D‑Balken‑ und 2‑D‑Säulendiagramme.

**Returns:**
short
### getPlotOnSecondAxis() {#getPlotOnSecondAxis--}
```
public boolean getPlotOnSecondAxis()
```


Zeigt an, ob diese Reihe auf der zweiten Werteachse dargestellt wird.

**Returns:**
boolean
### getPointValues() {#getPointValues--}
```
public ChartDataValue[] getPointValues()
```


Liest die tatsächlichen Werte, die zum Plotten jedes Punktes dieser Reihe im Diagramm verwendet werden.

**Remarks**

Diese Eigenschaft bietet eine bequeme Möglichkeit, die tatsächlichen Werte zu erhalten, die den durch [getValues()](../../com.aspose.cells/series\#getValues--) definierten Daten entsprechen, insbesondere wenn die angegebene Datenquelle ein externer Link, eine Formel usw. ist.

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


Liest die Sammlung von Punkten in einer Reihe eines Diagramms.

**Remarks**

Wenn das Diagramm ein Pie‑of‑Pie‑ oder Bar‑of‑Pie‑Diagramm ist, ist der letzte Punkt ein anderer Punkt im ersten Kuchendiagramm.

**Returns:**
[ChartPointCollection](../../com.aspose.cells/chartpointcollection)
### getSecondPlotSize() {#getSecondPlotSize--}
```
public short getSecondPlotSize()
```


Gibt die Größe des sekundären Abschnitts eines Pie‑of‑Pie‑ oder Bar‑of‑Pie‑Diagramms zurück oder legt sie fest, als Prozentsatz der Größe des primären Kuchens. Kann ein Wert von 5 bis 200 sein.

**Returns:**
short
### getSeriesLines() {#getSeriesLines--}
```
public Line getSeriesLines()
```


Gibt ein SeriesLines‑Objekt zurück, das die Serienlinien für ein gestapeltes Balken‑ oder Säulendiagramm darstellt. Gilt nur für gestapelte Balken‑ und Säulendiagramme.

**Returns:**
[Line](../../com.aspose.cells/line)
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


True, wenn die Serie einen Schatten hat.

**Returns:**
boolean
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Liest das [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)-Objekt, das die visuellen Formeigenschaften der Serie enthält.

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShowNegativeBubbles() {#getShowNegativeBubbles--}
```
public boolean getShowNegativeBubbles()
```


True, wenn negative Blasen für die Diagrammgruppe angezeigt werden. Nur für Blasendiagramme gültig.

**Returns:**
boolean
### getSizeRepresents() {#getSizeRepresents--}
```
public int getSizeRepresents()
```


Liefert, was die Blasengröße in einem Blasendiagramm darstellt.

Siehe [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

BubbleSizeRepresents.SizeIsArea bedeutet, dass der Wert [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) die Fläche der Blase ist. BubbleSizeRepresents.SizeIsWidth bedeutet, dass der Wert [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) die Breite der Blase ist.

**Returns:**
int
### getSmooth() {#getSmooth--}
```
public boolean getSmooth()
```


Stellt Kurvenglättung dar. True, wenn die Kurvenglättung für das Liniendiagramm oder Streudiagramm aktiviert ist. Gilt nur für Liniendiagramme und Streudiagramme mit Linien.

**Returns:**
boolean
### getSplitType() {#getSplitType--}
```
public int getSplitType()
```


Gibt einen Wert zurück oder legt ihn fest, der bestimmt, welche Datenpunkte im zweiten Kreis oder Balken eines Kreis‑im‑Kreis‑ bzw. Balken‑im‑Kreis‑Diagramms liegen.

Siehe [ChartSplitType](../../com.aspose.cells/chartsplittype).

**Returns:**
int
### getSplitValue() {#getSplitValue--}
```
public double getSplitValue()
```


Gibt einen Wert zurück oder legt ihn fest, der zur Bestimmung verwendet wird, welche Datenpunkte im zweiten Kreis oder Balken eines Kreis‑im‑Kreis‑ bzw. Balken‑im‑Kreis‑Diagramms liegen.

**Returns:**
double
### getTrendLines() {#getTrendLines--}
```
public TrendlineCollection getTrendLines()
```


Gibt alle Trendlinien dieser Serie zurück.

**Returns:**
[TrendlineCollection](../../com.aspose.cells/trendlinecollection)
### getType() {#getType--}
```
public int getType()
```


Liest den Typ einer Datenreihe.

Siehe [ChartType](../../com.aspose.cells/charttype).

**Returns:**
int
### getUpBars() {#getUpBars--}
```
public DropBars getUpBars()
```


Gibt ein DropBars‑Objekt zurück, das die Aufwärtsbalken in einem Liniendiagramm darstellt. Gilt nur für Liniendiagramme.

**Returns:**
[DropBars](../../com.aspose.cells/dropbars)
### getValues() {#getValues--}
```
public String getValues()
```


Stellt die Y‑Werte dieser Diagrammreihe dar.

**Remarks**

Um die tatsächlichen Werte (die jedem Punkt dieser Serie entsprechen), die durch diese Eigenschaft definiert werden, zu erhalten, verwenden Sie bitte [getPointValues()](../../com.aspose.cells/series\#getPointValues--).

**Returns:**
java.lang.String
### getValuesFormatCode() {#getValuesFormatCode--}
```
public String getValuesFormatCode()
```


Stellt den Formatcode der Werte‑NumberList dar.

**Returns:**
java.lang.String
### getXErrorBar() {#getXErrorBar--}
```
public ErrorBar getXErrorBar()
```


Stellt die X‑Richtungs-Fehlerbalken der Serie dar.

**Returns:**
[ErrorBar](../../com.aspose.cells/errorbar)
### getXValues() {#getXValues--}
```
public String getXValues()
```


Stellt die X‑Werte dieser Diagrammreihe dar.

**Remarks**

Nur für Streu‑ und Blasendiagramme. Bitte verwenden Sie [SeriesCollection.getCategoryData()](../../com.aspose.cells/seriescollection\#getCategoryData--) für andere Diagrammtypen; [getCategoryValues()](../../com.aspose.cells/series\#getCategoryValues--) wird verwendet, um die tatsächlichen Kategorienwerte dieser Serie zu erhalten.

**Returns:**
java.lang.String
### getXValuesFormatCode() {#getXValuesFormatCode--}
```
public String getXValuesFormatCode()
```


Stellt den Formatcode der X‑Werte‑NumberList dar.

**Returns:**
java.lang.String
### getYErrorBar() {#getYErrorBar--}
```
public ErrorBar getYErrorBar()
```


Stellt die Y‑Richtungs-Fehlerbalken der Serie dar.

**Returns:**
[ErrorBar](../../com.aspose.cells/errorbar)
### hasDropLines() {#hasDropLines--}
```
public boolean hasDropLines()
```


True, wenn das Diagramm Drop‑Lines hat. Gilt nur für Liniendiagramme oder Flächendiagramme.

**Returns:**
boolean
### hasHiLoLines() {#hasHiLoLines--}
```
public boolean hasHiLoLines()
```


True, wenn das Liniendiagramm Hoch‑Niedrig‑Linien hat. Gilt nur für Liniendiagramme.

**Returns:**
boolean
### hasLeaderLines() {#hasLeaderLines--}
```
public boolean hasLeaderLines()
```


True, wenn die Serie Führungslinien hat.

**Returns:**
boolean
### hasRadarAxisLabels() {#hasRadarAxisLabels--}
```
public boolean hasRadarAxisLabels()
```


True, wenn ein Radar‑Diagramm Kategorienachsenbeschriftungen hat. Gilt nur für Radar‑Diagramme.

**Returns:**
boolean
### hasSeriesLines() {#hasSeriesLines--}
```
public boolean hasSeriesLines()
```


Wahr, wenn ein gestapeltes Säulendiagramm oder Balkendiagramm Serienlinien hat oder wenn ein Pie of Pie‑Diagramm oder Bar of Pie‑Diagramm Verbindungslinien zwischen den beiden Abschnitten hat. Gilt nur für gestapelte Säulendiagramme, Balkendiagramme, Pie of Pie‑Diagramme oder Bar of Pie‑Diagramme.

**Returns:**
boolean
### hasUpDownBars() {#hasUpDownBars--}
```
public boolean hasUpDownBars()
```


Wahr, wenn ein Liniendiagramm Auf‑ und Ab‑Balken hat. Gilt nur für Liniendiagramme.

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


Gibt an, ob der Schwellenwert automatisch ist.

**Returns:**
boolean
### isColorVaried() {#isColorVaried--}
```
public boolean isColorVaried()
```


Gibt an, ob die Farbe der Punkte variiert ist. Das Diagramm muss nur eine Serie enthalten oder dieses Diagramm ist ein Kreisdiagramm.

**Returns:**
boolean
### isFiltered() {#isFiltered--}
```
public boolean isFiltered()
```


Gibt an, ob die Serie ausgewählt oder gefiltert ist. Wahr bedeutet, dass diese Serie gefiltert ist und nicht im Diagramm angezeigt wird.

**Returns:**
boolean
### isVerticalValues() {#isVerticalValues--}
```
public boolean isVerticalValues()
```


Gibt an, ob die Datenquelle vertikal ist.

**Returns:**
boolean
### move(int count) {#move-int-}
```
public void move(int count)
```


Verschiebt die Serie nach oben oder unten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Anzahl | int | Die Anzahl der Auf‑ oder Abbewegungen. Verschieben Sie die Serie nach oben, wenn dieser Wert kleiner als Null ist; verschieben Sie die Serie nach unten, wenn dieser Wert größer als Null ist. |

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


Legt den 3D‑Formtyp fest, der mit dem 3‑D‑Balken‑ oder Säulendiagramm verwendet wird.

Siehe [Bar3DShapeType](../../com.aspose.cells/bar3dshapetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setBubbleScale(int value) {#setBubbleScale-int-}
```
public void setBubbleScale(int value)
```


Legt den Skalierungsfaktor für Blasen in der angegebenen Diagrammgruppe fest. Er kann ein ganzzahliger Wert von 0 (null) bis 300 sein, was einem Prozentsatz der Standardgröße entspricht. Gilt nur für Blasendiagramme.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setBubbleSizeRepresents(int value) {#setBubbleSizeRepresents-int-}
```
public void setBubbleSizeRepresents(int value)
```


Liefert, was die Blasengröße in einem Blasendiagramm darstellt.

Siehe [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft Aspose.Cells.Charts.Series.SizeRepresents. Diese Eigenschaft wird 12 Monate nach JANUAR 2012 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setBubbleSizes(String value) {#setBubbleSizes-java.lang.String-}
```
public void setBubbleSizes(String value)
```


Legt die Blasengrößenwerte der Diagrammserie fest.

**Remarks**

Nur für [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) oder [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setColorVaried(boolean value) {#setColorVaried-boolean-}
```
public void setColorVaried(boolean value)
```


Gibt an, ob die Farbe der Punkte variiert ist. Das Diagramm muss nur eine Serie enthalten oder dieses Diagramm ist ein Kreisdiagramm.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDoughnutHoleSize(int value) {#setDoughnutHoleSize-int-}
```
public void setDoughnutHoleSize(int value)
```


Gibt die Größe des Lochs in einer Donut‑Diagrammgruppe zurück oder legt sie fest. Die Lochgröße wird als Prozentsatz der Diagrammgröße angegeben, zwischen 10 % und 90 %.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setExplosion(int value) {#setExplosion-int-}
```
public void setExplosion(int value)
```


Der Abstand eines offenen Kuchensegments vom Zentrum des Kuchendiagramms wird als Prozentsatz des Durchmessers des Kuchens angegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setFiltered(boolean value) {#setFiltered-boolean-}
```
public void setFiltered(boolean value)
```


Gibt an, ob die Serie ausgewählt oder gefiltert ist. Wahr bedeutet, dass diese Serie gefiltert ist und nicht im Diagramm angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFirstSliceAngle(short value) {#setFirstSliceAngle-short-}
```
public void setFirstSliceAngle(short value)
```


Legt den Winkel des ersten Kuchen‑ oder Donut‑Diagrammsegments in Grad fest (im Uhrzeigersinn von vertikal aus). Gilt nur für Kuchen-, 3‑D‑Kuchen‑ und Donut‑Diagramme, mit Werten von 0 bis 360.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | short |  |

### setGapWidth(short value) {#setGapWidth-short-}
```
public void setGapWidth(short value)
```


Gibt den Abstand zwischen Balken‑ oder Säulen‑Clustern zurück oder legt ihn fest, als Prozentsatz der Balken‑ oder Säulenbreite. Der Wert dieser Property muss zwischen 0 und 500 liegen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | short |  |

### setHas3DEffect(boolean value) {#setHas3DEffect-boolean-}
```
public void setHas3DEffect(boolean value)
```


Wahr, wenn die Serie ein dreidimensionales Erscheinungsbild hat.

**Remarks**

Gilt nur für [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) oder [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D) Diagramme.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHasDropLines(boolean value) {#setHasDropLines-boolean-}
```
public void setHasDropLines(boolean value)
```


True, wenn das Diagramm Drop‑Lines hat. Gilt nur für Liniendiagramme oder Flächendiagramme.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHasHiLoLines(boolean value) {#setHasHiLoLines-boolean-}
```
public void setHasHiLoLines(boolean value)
```


True, wenn das Liniendiagramm Hoch‑Niedrig‑Linien hat. Gilt nur für Liniendiagramme.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHasLeaderLines(boolean value) {#setHasLeaderLines-boolean-}
```
public void setHasLeaderLines(boolean value)
```


True, wenn die Serie Führungslinien hat.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHasRadarAxisLabels(boolean value) {#setHasRadarAxisLabels-boolean-}
```
public void setHasRadarAxisLabels(boolean value)
```


True, wenn ein Radar‑Diagramm Kategorienachsenbeschriftungen hat. Gilt nur für Radar‑Diagramme.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHasSeriesLines(boolean value) {#setHasSeriesLines-boolean-}
```
public void setHasSeriesLines(boolean value)
```


Wahr, wenn ein gestapeltes Säulendiagramm oder Balkendiagramm Serienlinien hat oder wenn ein Pie of Pie‑Diagramm oder Bar of Pie‑Diagramm Verbindungslinien zwischen den beiden Abschnitten hat. Gilt nur für gestapelte Säulendiagramme, Balkendiagramme, Pie of Pie‑Diagramme oder Bar of Pie‑Diagramme.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHasUpDownBars(boolean value) {#setHasUpDownBars-boolean-}
```
public void setHasUpDownBars(boolean value)
```


Wahr, wenn ein Liniendiagramm Auf‑ und Ab‑Balken hat. Gilt nur für Liniendiagramme.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Legt den Namen der Datenserie fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOverlap(short value) {#setOverlap-short-}
```
public void setOverlap(short value)
```


Gibt an, wie Balken und Säulen positioniert werden. Kann ein Wert zwischen -100 und 100 sein. Gilt nur für 2‑D‑Balken‑ und 2‑D‑Säulendiagramme.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | short |  |

### setPlotOnSecondAxis(boolean value) {#setPlotOnSecondAxis-boolean-}
```
public void setPlotOnSecondAxis(boolean value)
```


Zeigt an, ob diese Reihe auf der zweiten Werteachse dargestellt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSecondPlotSize(short value) {#setSecondPlotSize-short-}
```
public void setSecondPlotSize(short value)
```


Gibt die Größe des sekundären Abschnitts eines Pie‑of‑Pie‑ oder Bar‑of‑Pie‑Diagramms zurück oder legt sie fest, als Prozentsatz der Größe des primären Kuchens. Kann ein Wert von 5 bis 200 sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | short |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


True, wenn die Serie einen Schatten hat.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowNegativeBubbles(boolean value) {#setShowNegativeBubbles-boolean-}
```
public void setShowNegativeBubbles(boolean value)
```


True, wenn negative Blasen für die Diagrammgruppe angezeigt werden. Nur für Blasendiagramme gültig.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSizeRepresents(int value) {#setSizeRepresents-int-}
```
public void setSizeRepresents(int value)
```


Legt fest, was die Blasengröße in einem Blasendiagramm darstellt.

Siehe [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

BubbleSizeRepresents.SizeIsArea bedeutet, dass der Wert [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) die Fläche der Blase ist. BubbleSizeRepresents.SizeIsWidth bedeutet, dass der Wert [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) die Breite der Blase ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setSmooth(boolean value) {#setSmooth-boolean-}
```
public void setSmooth(boolean value)
```


Stellt Kurvenglättung dar. True, wenn die Kurvenglättung für das Liniendiagramm oder Streudiagramm aktiviert ist. Gilt nur für Liniendiagramme und Streudiagramme mit Linien.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSplitType(int value) {#setSplitType-int-}
```
public void setSplitType(int value)
```


Gibt einen Wert zurück oder legt ihn fest, der bestimmt, welche Datenpunkte im zweiten Kreis oder Balken eines Kreis‑im‑Kreis‑ bzw. Balken‑im‑Kreis‑Diagramms liegen.

Siehe [ChartSplitType](../../com.aspose.cells/chartsplittype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setSplitValue(double value) {#setSplitValue-double-}
```
public void setSplitValue(double value)
```


Gibt einen Wert zurück oder legt ihn fest, der zur Bestimmung verwendet wird, welche Datenpunkte im zweiten Kreis oder Balken eines Kreis‑im‑Kreis‑ bzw. Balken‑im‑Kreis‑Diagramms liegen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Legt den Typ einer Datenserie fest.

Siehe [ChartType](../../com.aspose.cells/charttype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setValues(String value) {#setValues-java.lang.String-}
```
public void setValues(String value)
```


Stellt die Y‑Werte dieser Diagrammreihe dar.

**Remarks**

Um die tatsächlichen Werte (die jedem Punkt dieser Serie entsprechen), die durch diese Eigenschaft definiert werden, zu erhalten, verwenden Sie bitte [getPointValues()](../../com.aspose.cells/series\#getPointValues--).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setValuesFormatCode(String value) {#setValuesFormatCode-java.lang.String-}
```
public void setValuesFormatCode(String value)
```


Stellt den Formatcode der Werte‑NumberList dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setXValues(String value) {#setXValues-java.lang.String-}
```
public void setXValues(String value)
```


Stellt die X‑Werte dieser Diagrammreihe dar.

**Remarks**

Nur für Streu‑ und Blasendiagramme. Bitte verwenden Sie [SeriesCollection.getCategoryData()](../../com.aspose.cells/seriescollection\#getCategoryData--) für andere Diagrammtypen; [getCategoryValues()](../../com.aspose.cells/series\#getCategoryValues--) wird verwendet, um die tatsächlichen Kategorienwerte dieser Serie zu erhalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setXValuesFormatCode(String value) {#setXValuesFormatCode-java.lang.String-}
```
public void setXValuesFormatCode(String value)
```


Stellt den Formatcode der X‑Werte‑NumberList dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

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

