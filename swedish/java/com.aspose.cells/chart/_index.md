---
title: "Diagram"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar objektet som representerar ett enskilt Excel-diagram."
type: docs
url: /sv/java/com.aspose.cells/chart/
---

**Inheritance:**
java.lang.Object
```
public class Chart
```

Inkapslar objektet som representerar ett enskilt Excel-diagram.

**Example**

Följande kod visar hur man skapar ett diagram med .NET-kod.

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
 
         	int chartIndex = sheet.getCharts().add(ChartType.COLUMN, 9, 9, 21, 15);
 
         	Chart chart = sheet.getCharts().get(chartIndex);
         chart.setChartDataRange("A1:B4", true);
         	chart.setShowLegend(true);
         	chart.getTitle().setText("Income Analysis");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [calculate()](#calculate--) | Beräknar de anpassade positionerna för plotområdet och axlarna om deras positioner tilldelas automatiskt. |
| [calculate(ChartCalculateOptions calculateOptions)](#calculate-com.aspose.cells.ChartCalculateOptions-) | Beräknar den anpassade positionen för plotområdet och axlarna om deras positioner tilldelas automatiskt, med Diagramberäkningsalternativ. |
| [changeTemplate(byte[] data)](#changeTemplate-byte---) | Ändra diagramtyp med en förinställd mall. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActualChartSize()](#getActualChartSize--) | Hämtar den faktiska storleken på diagrammet i pixelenheter. |
| [getActualSize()](#getActualSize--) | Hämtar den faktiska storleken på diagrammet i pixelenheter. |
| [getAutoScaling()](#getAutoScaling--) | Sant om Microsoft Excel skalar ett 3D-diagram så att det blir närmare i storlek det motsvarande 2D-diagrammet. |
| [getBackWall()](#getBackWall--) | Returnerar ett [getWalls()](../../com.aspose.cells/chart\#getWalls--)‑objekt som representerar bakväggen på ett 3D-diagram. |
| [getCategoryAxis()](#getCategoryAxis--) | Hämtar diagrammets X‑axel. |
| [getChartArea()](#getChartArea--) | Hämtar diagramområdet i kalkylbladet. |
| [getChartDataRange()](#getChartDataRange--) | Hämtar datakällans område för diagrammet. |
| [getChartDataTable()](#getChartDataTable--) | Representerar diagrammets datatabell. |
| [getChartObject()](#getChartObject--) | Representerar chartShape; |
| [getChartShape()](#getChartShape--) | Representerar chartShape; |
| [getClass()](#getClass--) |  |
| [getDepthPercent()](#getDepthPercent--) | Representerar djupet på ett 3‑D‑diagram som en procentandel av diagrammets bredd (mellan 20 och 2000 procent). |
| [getDisplayNaAsBlank()](#getDisplayNaAsBlank--) | Anger om \#N/A ska visas som ett tomt värde. |
| [getElevation()](#getElevation--) | Representerar höjden på 3‑D‑diagramvyn, i grader. |
| [getFilteredNSeries()](#getFilteredNSeries--) | Hämtar en [SeriesCollection](../../com.aspose.cells/seriescollection) samling som representerar dataserierna som filtreras i diagrammet. |
| [getFirstSliceAngle()](#getFirstSliceAngle--) | Hämtar vinkeln på den första paj- eller munkdiagramdelen, i grader (medurs från vertikal). |
| [getFloor()](#getFloor--) | Returnerar ett [getFloor()](../../com.aspose.cells/chart\#getFloor--)‑objekt som representerar väggarna i ett 3‑D‑diagram. |
| [getGapDepth()](#getGapDepth--) | Hämtar avståndet mellan dataserierna i ett 3‑D‑diagram, som en procentandel av markörens bredd. |
| [getGapWidth()](#getGapWidth--) | Returnerar eller anger avståndet mellan stapel‑ eller kolumnkluster, som en procentandel av stapelns eller kolumnens bredd. |
| [getHeightPercent()](#getHeightPercent--) | Returnerar eller anger höjden på ett 3‑D‑diagram som en procentandel av diagrammets bredd (mellan 5 och 500 procent). |
| [getHidePivotFieldButtons()](#getHidePivotFieldButtons--) | Anger om fältknapparna för pivottabellsdiagrammet ska döljas endast när diagrammet är en PivotChart. |
| [getIs3D()](#getIs3D--) | Anger om diagrammet är ett 3‑D‑diagram. |
| [getLegend()](#getLegend--) | Hämtar diagrammets förklaring. |
| [getLine()](#getLine--) | Hämtar linjen. |
| [getNSeries()](#getNSeries--) | Hämtar en [SeriesCollection](../../com.aspose.cells/seriescollection) samling som representerar dataserierna i diagrammet. |
| [getName()](#getName--) | Hämtar diagrammets namn. |
| [getPageSetup()](#getPageSetup--) | Representerar sidinställningsbeskrivningen i detta diagram. |
| [getPerspective()](#getPerspective--) | Returnerar eller anger perspektivet för three\u9225\u6178 dimensional diagramvyn. |
| [getPivotOptions()](#getPivotOptions--) | Specificerar pivåkontrollerna som visas i diagrammet |
| [getPivotSource()](#getPivotSource--) | Källan är data från pivottabellen. |
| [getPlacement()](#getPlacement--) | Representerar hur diagrammet är fäst vid cellerna under det. |
| [getPlotArea()](#getPlotArea--) | Hämtar diagrammets plotområde som inkluderar axelns tick‑etiketter. |
| [getPlotBy()](#getPlotBy--) | Hämtar om diagrammet plottas radvis eller kolumnvis. |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--) | Hämtar hur tomma celler ska plottas. |
| [getPlotVisibleCells()](#getPlotVisibleCells--) | Indikerar om endast plotens synliga celler. |
| [getPlotVisibleCellsOnly()](#getPlotVisibleCellsOnly--) | Indikerar om endast plotens synliga celler. |
| [getPrintSize()](#getPrintSize--) | Hämtar den utskrivna diagramstorleken. |
| [getRightAngleAxes()](#getRightAngleAxes--) | Sant om diagramaxlarna är i räta vinklar. |
| [getRotationAngle()](#getRotationAngle--) | Representerar rotationen av 3-D-diagramvyn (rotationen av plotområdet runt z-axeln, i grader). |
| [getSecondCategoryAxis()](#getSecondCategoryAxis--) | Hämtar diagrammets andra X-axel. |
| [getSecondValueAxis()](#getSecondValueAxis--) | Hämtar diagrammets andra Y-axel. |
| [getSeriesAxis()](#getSeriesAxis--) | Hämtar diagrammets serieaxel. |
| [getShapes()](#getShapes--) | Returnerar alla ritningsformer i detta diagram. |
| [getShowDataTable()](#getShowDataTable--) | Hämtar ett värde som indikerar om diagrammet visar en datatabell. |
| [getShowLegend()](#getShowLegend--) | Hämtar ett värde som indikerar om diagrammets förklaring kommer att visas. |
| [getSideWall()](#getSideWall--) | Returnerar ett [getWalls()](../../com.aspose.cells/chart\#getWalls--) objekt som representerar sidoväggen av ett 3-D-diagram. |
| [getSizeWithWindow()](#getSizeWithWindow--) | Sant om Microsoft Excel ändrar diagrammets storlek för att matcha storleken på diagrambladets fönster. |
| [getStyle()](#getStyle--) | Hämtar den inbyggda stilen. |
| [getSubTitle()](#getSubTitle--) | Hämtar diagrammets undertitel. |
| [getTitle()](#getTitle--) | Hämtar diagrammets titel. |
| [getType()](#getType--) | Hämtar diagrammets typ. |
| [getValueAxis()](#getValueAxis--) | Hämtar diagrammets Y-axel. |
| [getWalls()](#getWalls--) | Returnerar ett [getWalls()](../../com.aspose.cells/chart\#getWalls--) objekt som representerar väggarna i ett 3-D-diagram. |
| [getWallsAndGridlines2D()](#getWallsAndGridlines2D--) | Sant om rutnätslinjer ritas tvådimensionellt på ett 3-D-diagram. |
| [getWorksheet()](#getWorksheet--) | Hämtar arbetsbladet som innehåller detta diagram. |
| [hasAxis(int aixsType, boolean isPrimary)](#hasAxis-int-boolean-) | Returnerar vilka axlar som finns i diagrammet. |
| [hashCode()](#hashCode--) |  |
| [isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)](#isCellReferedByChart-int-int-int-) | Returnerar om cellen som diagrammet refererar till. |
| [isChartDataChanged()](#isChartDataChanged--) | Detekterar om ett diagrams datakälla har ändrats. |
| [isRectangularCornered()](#isRectangularCornered--) | Hämtar ett värde som indikerar om diagramområdet har rektangulära hörn. |
| [isReferedByChart(int rowIndex, int columnIndex)](#isReferedByChart-int-int-) | Returnerar om cellen refereras av diagrammet. |
| [move(int topRow, int leftColumn, int bottomRow, int rightColumn)](#move-int-int-int-int-) | Flyttar diagrammet till en angiven plats. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshPivotData()](#refreshPivotData--) | Uppdaterar diagrammets data från pivottabellen. |
| [setAutoScaling(boolean value)](#setAutoScaling-boolean-) | Sant om Microsoft Excel skalar ett 3D-diagram så att det blir närmare i storlek det motsvarande 2D-diagrammet. |
| [setChartDataRange(String area, boolean isVertical)](#setChartDataRange-java.lang.String-boolean-) | Anger dataområde för ett diagram. |
| [setDepthPercent(int value)](#setDepthPercent-int-) | Representerar djupet på ett 3‑D‑diagram som en procentandel av diagrammets bredd (mellan 20 och 2000 procent). |
| [setDisplayNaAsBlank(boolean value)](#setDisplayNaAsBlank-boolean-) | Anger om \#N/A ska visas som ett tomt värde. |
| [setElevation(int value)](#setElevation-int-) | Representerar höjden på 3‑D‑diagramvyn, i grader. |
| [setFirstSliceAngle(int value)](#setFirstSliceAngle-int-) | Ställer in vinkeln för den första sektorn i ett cirkeldiagram eller donutdiagram, i grader (medurs från vertikal). |
| [setGapDepth(int value)](#setGapDepth-int-) | Ställer in avståndet mellan dataserier i ett 3‑D‑diagram, som en procentandel av markörens bredd. |
| [setGapWidth(int value)](#setGapWidth-int-) | Returnerar eller anger avståndet mellan stapel‑ eller kolumnkluster, som en procentandel av stapelns eller kolumnens bredd. |
| [setHeightPercent(int value)](#setHeightPercent-int-) | Returnerar eller anger höjden på ett 3‑D‑diagram som en procentandel av diagrammets bredd (mellan 5 och 500 procent). |
| [setHidePivotFieldButtons(boolean value)](#setHidePivotFieldButtons-boolean-) | Anger om fältknapparna för pivottabellsdiagrammet ska döljas endast när diagrammet är en PivotChart. |
| [setName(String value)](#setName-java.lang.String-) | Ställer in diagrammets namn. |
| [setPerspective(short value)](#setPerspective-short-) | Returnerar eller anger perspektivet för three\u9225\u6178 dimensional diagramvyn. |
| [setPivotSource(String value)](#setPivotSource-java.lang.String-) | Källan är data från pivottabellen. |
| [setPlacement(int value)](#setPlacement-int-) | Representerar hur diagrammet är fäst vid cellerna under det. |
| [setPlotEmptyCellsType(int value)](#setPlotEmptyCellsType-int-) | Ställer in hur tomma celler ska plottas. |
| [setPlotVisibleCells(boolean value)](#setPlotVisibleCells-boolean-) | Indikerar om endast plotens synliga celler. |
| [setPlotVisibleCellsOnly(boolean value)](#setPlotVisibleCellsOnly-boolean-) | Indikerar om endast plotens synliga celler. |
| [setPrintSize(int value)](#setPrintSize-int-) | Ställer in den utskrivna diagramstorleken. |
| [setRectangularCornered(boolean value)](#setRectangularCornered-boolean-) | Ställer in ett värde som indikerar om diagramområdet har rektangulära hörn. |
| [setRightAngleAxes(boolean value)](#setRightAngleAxes-boolean-) | Sant om diagramaxlarna är i räta vinklar. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Representerar rotationen av 3-D-diagramvyn (rotationen av plotområdet runt z-axeln, i grader). |
| [setShowDataTable(boolean value)](#setShowDataTable-boolean-) | Ställer in ett värde som indikerar om diagrammet visar en datatabell. |
| [setShowLegend(boolean value)](#setShowLegend-boolean-) | Ställer in ett värde som indikerar om diagrammets förklaring ska visas. |
| [setSizeWithWindow(boolean value)](#setSizeWithWindow-boolean-) | Sant om Microsoft Excel ändrar diagrammets storlek för att matcha storleken på diagrambladets fönster. |
| [setStyle(int value)](#setStyle-int-) | Ställer in den inbyggda stilen. |
| [setType(int value)](#setType-int-) | Ställer in diagrammets typ. |
| [setWallsAndGridlines2D(boolean value)](#setWallsAndGridlines2D-boolean-) | Sant om rutnätslinjer ritas tvådimensionellt på ett 3-D-diagram. |
| [switchRowColumn()](#switchRowColumn--) | Växlar rad/kolumn. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | Skapar diagrammets bild och sparar den till en ström i det angivna formatet. |
| [toImage(String imageFile)](#toImage-java.lang.String-) | Skapar diagrammets bild och sparar den till en fil. |
| [toImage(String imageFile, ImageFormat imageFormat)](#toImage-java.lang.String-com.aspose.cells.ImageFormat-) | Skapar diagrammets bild och sparar den till en fil i det angivna formatet. |
| [toImage(String imageFile, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | Skapar diagrammets bild och sparar den till en fil. |
| [toImage(String imageFile, int imageType)](#toImage-java.lang.String-int-) | Skapar diagrammets bild och sparar den till en fil i den angivna bildtypen. |
| [toImage(String imageFile, long jpegQuality)](#toImage-java.lang.String-long-) | Skapar diagrammets bild och sparar den till en fil i JPEG‑formatet. |
| [toPdf(OutputStream stream)](#toPdf-java.io.OutputStream-) | Skapar diagrammets PDF och sparar den till en ström. |
| [toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)](#toPdf-java.io.OutputStream-float-float-int-int-) | Skapar diagrammets PDF och sparar den till en ström. |
| [toPdf(String fileName)](#toPdf-java.lang.String-) | Sparar diagrammet till en PDF‑fil. |
| [toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)](#toPdf-java.lang.String-float-float-int-int-) | Sparar diagrammet till en PDF‑fil. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### calculate() {#calculate--}
```
public void calculate()
```


Beräknar de anpassade positionerna för plotområdet och axlarna om deras positioner tilldelas automatiskt.

### calculate(ChartCalculateOptions calculateOptions) {#calculate-com.aspose.cells.ChartCalculateOptions-}
```
public void calculate(ChartCalculateOptions calculateOptions)
```


Beräknar den anpassade positionen för plotområdet och axlarna om deras positioner tilldelas automatiskt, med Diagramberäkningsalternativ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| calculateOptions | [ChartCalculateOptions](../../com.aspose.cells/chartcalculateoptions) |  |

### changeTemplate(byte[] data) {#changeTemplate-byte---}
```
public void changeTemplate(byte[] data)
```


Ändra diagramtyp med en förinställd mall.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| data | byte[] | Data för diagrammallfilen (.crtx). |

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
### getActualChartSize() {#getActualChartSize--}
```
public int[] getActualChartSize()
```


Hämtar den faktiska storleken på diagrammet i pixelenheter.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd i stället metoden Chart.getActualSize(). Denna egenskap kommer att tas bort 12 månader senare från och med juli 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int[] - Faktisk storlek i en array (bredd och höjd). [0] är bredd; [1] är höjd.
### getActualSize() {#getActualSize--}
```
public int[] getActualSize()
```


Hämtar den faktiska storleken på diagrammet i pixelenheter.

**Returns:**
int[] - Faktisk storlek i en array (bredd och höjd). [0] är bredd; [1] är höjd.
### getAutoScaling() {#getAutoScaling--}
```
public boolean getAutoScaling()
```


Sant om Microsoft Excel skalar ett 3‑D‑diagram så att det är närmare i storlek till motsvarande 2‑D‑diagram. Egenskapen RightAngleAxes måste vara Sant.

**Returns:**
boolean
### getBackWall() {#getBackWall--}
```
public Walls getBackWall()
```


Returnerar ett [getWalls()](../../com.aspose.cells/chart\#getWalls--)‑objekt som representerar bakväggen på ett 3D-diagram.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getCategoryAxis() {#getCategoryAxis--}
```
public Axis getCategoryAxis()
```


Hämtar diagrammets X‑axel.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getChartArea() {#getChartArea--}
```
public ChartArea getChartArea()
```


Hämtar diagramområdet i kalkylbladet.

**Returns:**
[ChartArea](../../com.aspose.cells/chartarea)
### getChartDataRange() {#getChartDataRange--}
```
public String getChartDataRange()
```


Hämtar datakällans område för diagrammet.

**Remarks**

Stöder endast intervall. Om Series.Values, Name och XValues finns i ett kontinuerligt intervall, returneras ett intervall som innehåller dem.

**Returns:**
java.lang.String - Datakällan.
### getChartDataTable() {#getChartDataTable--}
```
public ChartDataTable getChartDataTable()
```


Representerar diagrammets datatabell.

**Returns:**
[ChartDataTable](../../com.aspose.cells/chartdatatable)
### getChartObject() {#getChartObject--}
```
public ChartShape getChartObject()
```


Representerar chartShape;

**Returns:**
[ChartShape](../../com.aspose.cells/chartshape)
### getChartShape() {#getChartShape--}
```
public ChartShape getChartShape()
```


Representerar chartShape;

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen Aspose.Cells.Charts.Chart.ChartObject. Denna egenskap kommer att tas bort 12 månader senare sedan JANUARI 2012. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
[ChartShape](../../com.aspose.cells/chartshape)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDepthPercent() {#getDepthPercent--}
```
public int getDepthPercent()
```


Representerar djupet på ett 3‑D‑diagram som en procentandel av diagrammets bredd (mellan 20 och 2000 procent).

**Returns:**
int
### getDisplayNaAsBlank() {#getDisplayNaAsBlank--}
```
public boolean getDisplayNaAsBlank()
```


Anger om \#N/A ska visas som ett tomt värde.

**Returns:**
boolean
### getElevation() {#getElevation--}
```
public int getElevation()
```


Representerar höjden på 3‑D‑diagramvyn, i grader.

**Remarks**

Diagramhöjden är den höjd där du ser diagrammet, i grader. Standardvärdet är 15 för de flesta diagramtyper. Värdet för denna egenskap måste vara mellan -90 och 90, förutom för 3‑D‑stapeldiagram, där det måste vara mellan 0 och 44.

**Returns:**
int
### getFilteredNSeries() {#getFilteredNSeries--}
```
public SeriesCollection getFilteredNSeries()
```


Hämtar en [SeriesCollection](../../com.aspose.cells/seriescollection) samling som representerar dataserierna som filtreras i diagrammet.

**Returns:**
[SeriesCollection](../../com.aspose.cells/seriescollection)
### getFirstSliceAngle() {#getFirstSliceAngle--}
```
public int getFirstSliceAngle()
```


Hämtar vinkeln för den första paj- eller munkdiagramdelen, i grader (medurs från vertikal). Gäller endast för paj-, 3‑D‑paj- och munkdiagram, 0 till 360.

**Returns:**
int
### getFloor() {#getFloor--}
```
public Floor getFloor()
```


Returnerar ett [getFloor()](../../com.aspose.cells/chart\#getFloor--)‑objekt som representerar väggarna i ett 3‑D‑diagram.

**Remarks**

Denna egenskap gäller inte för 3‑D‑pajdiagram.

**Returns:**
[Floor](../../com.aspose.cells/floor)
### getGapDepth() {#getGapDepth--}
```
public int getGapDepth()
```


Hämtar avståndet mellan dataserierna i ett 3‑D‑diagram, som en procentandel av markörens bredd. Värdet för denna egenskap måste vara mellan 0 och 500.

**Returns:**
int
### getGapWidth() {#getGapWidth--}
```
public int getGapWidth()
```


Returnerar eller anger utrymmet mellan stapel- eller kolumnkluster, som en procentandel av stapelns eller kolumnens bredd. Värdet för denna egenskap måste vara mellan 0 och 500.

**Returns:**
int
### getHeightPercent() {#getHeightPercent--}
```
public int getHeightPercent()
```


Returnerar eller anger höjden på ett 3‑D‑diagram som en procentandel av diagrammets bredd (mellan 5 och 500 procent).

**Returns:**
int
### getHidePivotFieldButtons() {#getHidePivotFieldButtons--}
```
public boolean getHidePivotFieldButtons()
```


Anger om fältknapparna för pivottabellsdiagrammet ska döljas endast när diagrammet är en PivotChart.

**Returns:**
boolean
### getIs3D() {#getIs3D--}
```
public boolean getIs3D()
```


Anger om diagrammet är ett 3‑D‑diagram.

**Returns:**
boolean
### getLegend() {#getLegend--}
```
public Legend getLegend()
```


Hämtar diagrammets förklaring.

**Returns:**
[Legend](../../com.aspose.cells/legend)
### getLine() {#getLine--}
```
public Line getLine()
```


Hämtar linjen.

**Returns:**
[Line](../../com.aspose.cells/line)
### getNSeries() {#getNSeries--}
```
public SeriesCollection getNSeries()
```


Hämtar en [SeriesCollection](../../com.aspose.cells/seriescollection) samling som representerar dataserierna i diagrammet.

**Returns:**
[SeriesCollection](../../com.aspose.cells/seriescollection)
### getName() {#getName--}
```
public String getName()
```


Hämtar diagrammets namn.

**Returns:**
java.lang.String
### getPageSetup() {#getPageSetup--}
```
public PageSetup getPageSetup()
```


Representerar sidinställningsbeskrivningen i detta diagram.

**Returns:**
[PageSetup](../../com.aspose.cells/pagesetup)
### getPerspective() {#getPerspective--}
```
public short getPerspective()
```


Returnerar eller anger perspektivet för den three\\u9225\\u6178 dimensionella diagramvyn. Måste vara mellan 0 och 100. Denna egenskap ignoreras om egenskapen RightAngleAxes är Sant.

**Returns:**
short
### getPivotOptions() {#getPivotOptions--}
```
public PivotOptions getPivotOptions()
```


Specificerar pivåkontrollerna som visas i diagrammet

**Returns:**
[PivotOptions](../../com.aspose.cells/pivotoptions)
### getPivotSource() {#getPivotSource--}
```
public String getPivotSource()
```


Källan är data från pivottabellen. Om PivotSource inte är tom, är diagrammet ett PivotChart.

**Remarks**

Om pivottabellen "PivotTable1" i arbetsbladet "Sheet1" i filen "Book1.xls". pivotSource kan vara "[Book1.xls]Sheet1!PivotTable1" om diagrammet och pivottabellen inte finns i samma arbetsbok. Om du anger denna egenskap, förloras den tidigare datakällinställningen.

**Returns:**
java.lang.String
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


Representerar hur diagrammet är fäst vid cellerna under det.

Se [PlacementType](../../com.aspose.cells/placementtype).

**Returns:**
int
### getPlotArea() {#getPlotArea--}
```
public PlotArea getPlotArea()
```


Hämtar diagrammets plotområde som inkluderar axelns tick‑etiketter.

**Remarks**

**Returns:**
[PlotArea](../../com.aspose.cells/plotarea)
### getPlotBy() {#getPlotBy--}
```
public int getPlotBy()
```


Hämtar om diagrammet plottas radvis eller kolumnvis.

Se [PlotDataByType](../../com.aspose.cells/plotdatabytype).

**Returns:**
int
### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}
```
public int getPlotEmptyCellsType()
```


Hämtar hur tomma celler ska plottas.

Se [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Returns:**
int
### getPlotVisibleCells() {#getPlotVisibleCells--}
```
public boolean getPlotVisibleCells()
```


Indikerar om endast plotens synliga celler.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen PlotVisibleCellsOnly. Denna metod kommer att tas bort 12 månader senare sedan december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### getPlotVisibleCellsOnly() {#getPlotVisibleCellsOnly--}
```
public boolean getPlotVisibleCellsOnly()
```


Indikerar om endast plotens synliga celler.

**Returns:**
boolean
### getPrintSize() {#getPrintSize--}
```
public int getPrintSize()
```


Hämtar den utskrivna diagramstorleken.

Se [PrintSizeType](../../com.aspose.cells/printsizetype).

**Returns:**
int
### getRightAngleAxes() {#getRightAngleAxes--}
```
public boolean getRightAngleAxes()
```


Sant om diagramaxlarna är i räta vinklar. Gäller endast för 3‑D‑diagram (förutom Column3D och 3‑D‑pajdiagram).

**Remarks**

Om denna egenskap är Sant, ignoreras egenskapen Perspective.

**Returns:**
boolean
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Representerar rotationen av 3-D-diagramvyn (rotationen av plotområdet runt z-axeln, i grader).

**Remarks**

Värdet för denna egenskap måste vara mellan 0 och 360, förutom för 3‑D‑stapeldiagram, där värdet måste vara mellan 0 och 44. Standardvärdet är 20. Gäller endast för 3‑D‑diagram.

**Returns:**
int
### getSecondCategoryAxis() {#getSecondCategoryAxis--}
```
public Axis getSecondCategoryAxis()
```


Hämtar diagrammets andra X-axel.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getSecondValueAxis() {#getSecondValueAxis--}
```
public Axis getSecondValueAxis()
```


Hämtar diagrammets andra Y-axel.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getSeriesAxis() {#getSeriesAxis--}
```
public Axis getSeriesAxis()
```


Hämtar diagrammets serieaxel.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getShapes() {#getShapes--}
```
public ShapeCollection getShapes()
```


Returnerar alla ritningsformer i detta diagram.

**Returns:**
[ShapeCollection](../../com.aspose.cells/shapecollection)
### getShowDataTable() {#getShowDataTable--}
```
public boolean getShowDataTable()
```


Hämtar ett värde som indikerar om diagrammet visar en datatabell.

**Returns:**
boolean
### getShowLegend() {#getShowLegend--}
```
public boolean getShowLegend()
```


Hämtar ett värde som indikerar om diagramförklaringen ska visas. Standard är sant.

**Returns:**
boolean
### getSideWall() {#getSideWall--}
```
public Walls getSideWall()
```


Returnerar ett [getWalls()](../../com.aspose.cells/chart\#getWalls--) objekt som representerar sidoväggen av ett 3-D-diagram.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getSizeWithWindow() {#getSizeWithWindow--}
```
public boolean getSizeWithWindow()
```


Sant om Microsoft Excel ändrar diagrammets storlek för att matcha storleken på diagrambladets fönster.

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public int getStyle()
```


Hämtar den inbyggda stilen.

**Remarks**

Den bör vara mellan 1 och 48. Returnera -1 om den inte har satts.

**Returns:**
int
### getSubTitle() {#getSubTitle--}
```
public Title getSubTitle()
```


Hämtar diagrammets undertitel. Gäller endast för ODS‑filer.

**Returns:**
[Title](../../com.aspose.cells/title)
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Hämtar diagrammets titel.

**Returns:**
[Title](../../com.aspose.cells/title)
### getType() {#getType--}
```
public int getType()
```


Hämtar diagrammets typ.

Se [ChartType](../../com.aspose.cells/charttype).

**Returns:**
int
### getValueAxis() {#getValueAxis--}
```
public Axis getValueAxis()
```


Hämtar diagrammets Y-axel.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getWalls() {#getWalls--}
```
public Walls getWalls()
```


Returnerar ett [getWalls()](../../com.aspose.cells/chart\#getWalls--) objekt som representerar väggarna i ett 3-D-diagram.

**Remarks**

Denna egenskap gäller inte för 3‑D‑pajdiagram.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getWallsAndGridlines2D() {#getWallsAndGridlines2D--}
```
public boolean getWallsAndGridlines2D()
```


Sant om rutnätslinjer ritas tvådimensionellt på ett 3-D-diagram.

**Returns:**
boolean
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Hämtar arbetsbladet som innehåller detta diagram.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hasAxis(int aixsType, boolean isPrimary) {#hasAxis-int-boolean-}
```
public boolean hasAxis(int aixsType, boolean isPrimary)
```


Returnerar vilka axlar som finns i diagrammet.

**Remarks**

Vanligtvis har Pie, PieExploded, PiePie, PieBar, Pie3D, Pie3DExploded, Doughnut, DoughnutExploded ingen axel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| aixsType | int |  |
| isPrimary | boolean |  |

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex) {#isCellReferedByChart-int-int-int-}
```
public boolean isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)
```


Returnerar om cellen som diagrammet refererar till.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | int | Index -1 för bladet betyder kalkylbladet som innehåller det aktuella diagrammet. |
| rowIndex | int | Radindexet |
| columnIndex | int | Kolumnindexet |

**Returns:**
boolean -
### isChartDataChanged() {#isChartDataChanged--}
```
public boolean isChartDataChanged()
```


Detekterar om ett diagrams datakälla har ändrats.

**Remarks**

Metoden upptäcker förändringar i diagrammets datakälla innan diagrammet renderas till bildformat. Vid första anropet av Chart.toImage kommer diagrammets källdata (t.ex. XValuesParseData, ValuesParseData) att registreras. Innan du anropar Chart.toImage‑metoden igen, anropa IsChartDataChanged‑metoden för att kontrollera om diagrammet behöver renderas om.

**Returns:**
boolean - Returnerar true om diagrammet har ändrats, annars returneras false
### isRectangularCornered() {#isRectangularCornered--}
```
public boolean isRectangularCornered()
```


Hämtar ett värde som anger om diagramområdet har rektangulära hörn. Standardvärdet är true.

**Returns:**
boolean
### isReferedByChart(int rowIndex, int columnIndex) {#isReferedByChart-int-int-}
```
public boolean isReferedByChart(int rowIndex, int columnIndex)
```


Returnerar om cellen refereras av diagrammet.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället metoden IsCellReferedByChart(int,int,int). Denna metod kommer att tas bort 12 månader senare från och med april 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int | Radindexet |
| columnIndex | int | Kolumnindexet |

**Returns:**
boolean -
### move(int topRow, int leftColumn, int bottomRow, int rightColumn) {#move-int-int-int-int-}
```
public void move(int topRow, int leftColumn, int bottomRow, int rightColumn)
```


Flyttar diagrammet till en angiven plats.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| leftColumn | int | Övre vänstra kolumnindex. |
| bottomRow | int | Nedre högra radindex |
| rightColumn | int | Nedre högra kolumnindex |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshPivotData() {#refreshPivotData--}
```
public void refreshPivotData()
```


Uppdaterar diagrammets data från pivottabellen.

**Remarks**

Vi samlar in data från pivottabellens datakälla till pivottabellsrapporten. Denna metod används endast för att samla all data till ett pivottabellsdiagram.

### setAutoScaling(boolean value) {#setAutoScaling-boolean-}
```
public void setAutoScaling(boolean value)
```


Sant om Microsoft Excel skalar ett 3‑D‑diagram så att det är närmare i storlek till motsvarande 2‑D‑diagram. Egenskapen RightAngleAxes måste vara Sant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setChartDataRange(String area, boolean isVertical) {#setChartDataRange-java.lang.String-boolean-}
```
public void setChartDataRange(String area, boolean isVertical)
```


Anger dataområde för ett diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| area | java.lang.String | Anger värden som dataserien ska plottas från |
| isVertical | boolean | Anger om serierna ska plottas från ett cellvärdesintervall radvis eller kolumnvis. |

### setDepthPercent(int value) {#setDepthPercent-int-}
```
public void setDepthPercent(int value)
```


Representerar djupet på ett 3‑D‑diagram som en procentandel av diagrammets bredd (mellan 20 och 2000 procent).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setDisplayNaAsBlank(boolean value) {#setDisplayNaAsBlank-boolean-}
```
public void setDisplayNaAsBlank(boolean value)
```


Anger om \#N/A ska visas som ett tomt värde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setElevation(int value) {#setElevation-int-}
```
public void setElevation(int value)
```


Representerar höjden på 3‑D‑diagramvyn, i grader.

**Remarks**

Diagramhöjden är den höjd där du ser diagrammet, i grader. Standardvärdet är 15 för de flesta diagramtyper. Värdet för denna egenskap måste vara mellan -90 och 90, förutom för 3‑D‑stapeldiagram, där det måste vara mellan 0 och 44.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setFirstSliceAngle(int value) {#setFirstSliceAngle-int-}
```
public void setFirstSliceAngle(int value)
```


Ställer in vinkeln för den första sektorn i ett paj- eller donutdiagram, i grader (medurs från vertikal). Gäller endast för paj-, 3‑D‑paj- och donutdiagram, 0 till 360.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setGapDepth(int value) {#setGapDepth-int-}
```
public void setGapDepth(int value)
```


Ställer in avståndet mellan dataserierna i ett 3‑D‑diagram, som en procentandel av markörens bredd. Värdet för denna egenskap måste ligga mellan 0 och 500.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setGapWidth(int value) {#setGapWidth-int-}
```
public void setGapWidth(int value)
```


Returnerar eller anger utrymmet mellan stapel- eller kolumnkluster, som en procentandel av stapelns eller kolumnens bredd. Värdet för denna egenskap måste vara mellan 0 och 500.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setHeightPercent(int value) {#setHeightPercent-int-}
```
public void setHeightPercent(int value)
```


Returnerar eller anger höjden på ett 3‑D‑diagram som en procentandel av diagrammets bredd (mellan 5 och 500 procent).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setHidePivotFieldButtons(boolean value) {#setHidePivotFieldButtons-boolean-}
```
public void setHidePivotFieldButtons(boolean value)
```


Anger om fältknapparna för pivottabellsdiagrammet ska döljas endast när diagrammet är en PivotChart.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Ställer in diagrammets namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setPerspective(short value) {#setPerspective-short-}
```
public void setPerspective(short value)
```


Returnerar eller anger perspektivet för den three\\u9225\\u6178 dimensionella diagramvyn. Måste vara mellan 0 och 100. Denna egenskap ignoreras om egenskapen RightAngleAxes är Sant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | short |  |

### setPivotSource(String value) {#setPivotSource-java.lang.String-}
```
public void setPivotSource(String value)
```


Källan är data från pivottabellen. Om PivotSource inte är tom, är diagrammet ett PivotChart.

**Remarks**

Om pivottabellen "PivotTable1" i arbetsbladet "Sheet1" i filen "Book1.xls". pivotSource kan vara "[Book1.xls]Sheet1!PivotTable1" om diagrammet och pivottabellen inte finns i samma arbetsbok. Om du anger denna egenskap, förloras den tidigare datakällinställningen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Representerar hur diagrammet är fäst vid cellerna under det.

Se [PlacementType](../../com.aspose.cells/placementtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPlotEmptyCellsType(int value) {#setPlotEmptyCellsType-int-}
```
public void setPlotEmptyCellsType(int value)
```


Ställer in hur tomma celler ska plottas.

Se [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPlotVisibleCells(boolean value) {#setPlotVisibleCells-boolean-}
```
public void setPlotVisibleCells(boolean value)
```


Indikerar om endast plotens synliga celler.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen PlotVisibleCellsOnly. Denna metod kommer att tas bort 12 månader senare sedan december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPlotVisibleCellsOnly(boolean value) {#setPlotVisibleCellsOnly-boolean-}
```
public void setPlotVisibleCellsOnly(boolean value)
```


Indikerar om endast plotens synliga celler.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPrintSize(int value) {#setPrintSize-int-}
```
public void setPrintSize(int value)
```


Ställer in den utskrivna diagramstorleken.

Se [PrintSizeType](../../com.aspose.cells/printsizetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setRectangularCornered(boolean value) {#setRectangularCornered-boolean-}
```
public void setRectangularCornered(boolean value)
```


Ställer in ett värde som anger om diagramområdet har rektangulära hörn. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRightAngleAxes(boolean value) {#setRightAngleAxes-boolean-}
```
public void setRightAngleAxes(boolean value)
```


Sant om diagramaxlarna är i räta vinklar. Gäller endast för 3‑D‑diagram (förutom Column3D och 3‑D‑pajdiagram).

**Remarks**

Om denna egenskap är Sant, ignoreras egenskapen Perspective.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Representerar rotationen av 3-D-diagramvyn (rotationen av plotområdet runt z-axeln, i grader).

**Remarks**

Värdet för denna egenskap måste vara mellan 0 och 360, förutom för 3‑D‑stapeldiagram, där värdet måste vara mellan 0 och 44. Standardvärdet är 20. Gäller endast för 3‑D‑diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setShowDataTable(boolean value) {#setShowDataTable-boolean-}
```
public void setShowDataTable(boolean value)
```


Ställer in ett värde som indikerar om diagrammet visar en datatabell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowLegend(boolean value) {#setShowLegend-boolean-}
```
public void setShowLegend(boolean value)
```


Ställer in ett värde som anger om diagramförklaringen ska visas. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSizeWithWindow(boolean value) {#setSizeWithWindow-boolean-}
```
public void setSizeWithWindow(boolean value)
```


Sant om Microsoft Excel ändrar diagrammets storlek för att matcha storleken på diagrambladets fönster.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```


Ställer in den inbyggda stilen.

**Remarks**

Den bör vara mellan 1 och 48. Returnera -1 om den inte har satts.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Ställer in diagrammets typ.

Se [ChartType](../../com.aspose.cells/charttype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setWallsAndGridlines2D(boolean value) {#setWallsAndGridlines2D-boolean-}
```
public void setWallsAndGridlines2D(boolean value)
```


Sant om rutnätslinjer ritas tvådimensionellt på ett 3-D-diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### switchRowColumn() {#switchRowColumn--}
```
public boolean switchRowColumn()
```


Växlar rad/kolumn.

**Returns:**
boolean - False betyder att byte av rad/kolumn misslyckas.
### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


Skapar diagrammets bild och sparar den till en ström i det angivna formatet.

**Remarks**

Bildformatet specificeras med `options.ImageFormat`. Följande format stöds: ImageFormat.Bmp, ImageFormat.Gif, ImageFormat.Png, ImageFormat.Jpeg, ImageFormat.Tiff, ImageFormat.Emf.

Om bredden eller höjden är noll eller om diagrammet inte stöds enligt Supported Charts List, kommer denna metod inte att göra något. Se [Supported Charts List][] för mer information.


[Supported Charts List]: http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Utdatastreamen. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Ytterligare alternativ för bildskapande |

### toImage(String imageFile) {#toImage-java.lang.String-}
```
public void toImage(String imageFile)
```


Skapar diagrambilden och sparar den till en fil. Filnamnets filändelse bestämmer bildformatet.

**Remarks**

Bildformatet specificeras med filändelsen i filnamnet. Till exempel, om du anger "myfile.png", sparas bilden i PNG-format. Följande filändelser känns igen: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Om bredden eller höjden är noll eller om diagrammet inte stöds enligt Supported Charts List, kommer denna metod inte att göra något.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| imageFile | java.lang.String | Bildfilens namn med fullständig sökväg. |

### toImage(String imageFile, ImageFormat imageFormat) {#toImage-java.lang.String-com.aspose.cells.ImageFormat-}
```
public void toImage(String imageFile, ImageFormat imageFormat)
```


Skapar diagrammets bild och sparar den till en fil i det angivna formatet.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället metoden Chart.ToImage(string, ImageType). Denna egenskap kommer att tas bort 12 månader senare från och med juli 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| imageFile | java.lang.String | Bildfilens namn med fullständig sökväg. |
| imageFormat | [ImageFormat](../../com.aspose.cells/imageformat) | Formatet som bilden ska sparas i. |

### toImage(String imageFile, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String imageFile, ImageOrPrintOptions options)
```


Skapar diagrambilden och sparar den till en fil. Filnamnets filändelse bestämmer bildformatet.

**Remarks**

Bildformatet specificeras med filändelsen i filnamnet. Till exempel, om du anger "myfile.png", sparas bilden i PNG-format. Följande filändelser känns igen: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Om bredden eller höjden är noll eller om diagrammet inte stöds enligt Supported Charts List, kommer denna metod inte att göra något. Se [Supported Charts List][] för mer information.

**Example**

Sparar till Tiff med 300 dpi och CCITT4-komprimering.

```
         ImageOrPrintOptions options = new ImageOrPrintOptions();
         options.setHorizontalResolution(300);
         options.setVerticalResolution(300);
         options.setTiffCompression(TiffCompression.COMPRESSION_CCITT_4);
 
         Workbook book = new Workbook("test.xls");
         book.getWorksheets().get(0).getCharts().get(0).toImage("chart.Tiff", options);
```


[Supported Charts List]: http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| imageFile | java.lang.String | Bildfilens namn med fullständig sökväg. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Ytterligare alternativ för bildskapande |

### toImage(String imageFile, int imageType) {#toImage-java.lang.String-int-}
```
public void toImage(String imageFile, int imageType)
```


Skapar diagrammets bild och sparar den till en fil i den angivna bildtypen.

**Remarks**

Bildtypen specificeras med `imageType`. Följande typer stöds: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Om bredden eller höjden är noll eller om diagrammet inte stöds enligt Supported Charts List, kommer denna metod inte att göra något.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| imageFile | java.lang.String | Bildfilens namn med fullständig sökväg. |
| imageType | int | [ImageType](../../com.aspose.cells/imagetype). Bildtypen som ska användas för att spara bilden. |

### toImage(String imageFile, long jpegQuality) {#toImage-java.lang.String-long-}
```
public void toImage(String imageFile, long jpegQuality)
```


Skapar diagrammets bild och sparar den till en fil i JPEG‑formatet.

**Remarks**

Om bredden eller höjden är noll eller diagrammet inte stöds enligt Supported Charts List, kommer den här metoden inte göra någonting. OBS: Den här metoden är nu föråldrad. Använd istället ToImage(string,ImageOrPrintOptions)-metoden med angiven kvalitet. Denna metod kommer att tas bort 12 månader senare från och med mars 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| imageFile | java.lang.String | Bildfilens namn med fullständig sökväg. |
| jpegQuality | long | Jpeg-kvalitet. |

### toPdf(OutputStream stream) {#toPdf-java.io.OutputStream-}
```
public void toPdf(OutputStream stream)
```


Skapar diagrammets PDF och sparar den till en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Utdatastreamen. |

### toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType) {#toPdf-java.io.OutputStream-float-float-int-int-}
```
public void toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)
```


Skapar diagrammets PDF och sparar den till en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Utdatastreamen. |
| desiredPageWidth | float | Den önskade sidbredden i tum. |
| desiredPageHeight | float | Den önskade sidhöjden i tum. |
| hAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Diagrammets horisontella justeringstyp på den utgående sidan. |
| vAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Diagrammets vertikala justeringstyp på den utgående sidan. |

### toPdf(String fileName) {#toPdf-java.lang.String-}
```
public void toPdf(String fileName)
```


Sparar diagrammet till en PDF‑fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | pdf-filnamnet med fullständig sökväg |

### toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType) {#toPdf-java.lang.String-float-float-int-int-}
```
public void toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)
```


Sparar diagrammet till en PDF‑fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | pdf-filnamnet med fullständig sökväg |
| desiredPageWidth | float | Den önskade sidbredden i tum. |
| desiredPageHeight | float | Den önskade sidhöjden i tum. |
| hAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Diagrammets horisontella justeringstyp på den utgående sidan. |
| vAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Diagrammets vertikala justeringstyp på den utgående sidan. |

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

