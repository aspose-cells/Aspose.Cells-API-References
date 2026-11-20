---
title: "Grafico"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta un singolo grafico Excel."
type: docs
url: /it/java/com.aspose.cells/chart/
---

**Inheritance:**
java.lang.Object
```
public class Chart
```

Incapsula l'oggetto che rappresenta un singolo grafico Excel.

**Example**

Il codice seguente mostra come creare un grafico con codice .NET.

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
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [calculate()](#calculate--) | Calcola le posizioni personalizzate dell'area del grafico e degli assi se le loro posizioni sono assegnate automaticamente. |
| [calculate(ChartCalculateOptions calculateOptions)](#calculate-com.aspose.cells.ChartCalculateOptions-) | Calcola la posizione personalizzata dell'area del grafico e degli assi se le loro posizioni sono assegnate automaticamente, con le Opzioni di Calcolo del Grafico. |
| [changeTemplate(byte[] data)](#changeTemplate-byte---) | Cambia il tipo di grafico con un modello predefinito. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActualChartSize()](#getActualChartSize--) | Ottiene le dimensioni effettive del grafico in unità di pixel. |
| [getActualSize()](#getActualSize--) | Ottiene le dimensioni effettive del grafico in unità di pixel. |
| [getAutoScaling()](#getAutoScaling--) | Vero se Microsoft Excel scala un grafico 3D in modo che sia più vicino in dimensioni al grafico 2D equivalente. |
| [getBackWall()](#getBackWall--) | Restituisce un oggetto [getWalls()](../../com.aspose.cells/chart\#getWalls--) che rappresenta la parete posteriore di un grafico 3D. |
| [getCategoryAxis()](#getCategoryAxis--) | Ottiene l'asse X del grafico. |
| [getChartArea()](#getChartArea--) | Ottiene l'area del grafico nel foglio di lavoro. |
| [getChartDataRange()](#getChartDataRange--) | Ottiene l'intervallo della fonte dati del grafico. |
| [getChartDataTable()](#getChartDataTable--) | Rappresenta la tabella dei dati del grafico. |
| [getChartObject()](#getChartObject--) | Rappresenta il chartShape; |
| [getChartShape()](#getChartShape--) | Rappresenta il chartShape; |
| [getClass()](#getClass--) |  |
| [getDepthPercent()](#getDepthPercent--) | Rappresenta la profondità di un grafico 3-D come percentuale della larghezza del grafico (tra il 20% e il 2000%). |
| [getDisplayNaAsBlank()](#getDisplayNaAsBlank--) | Indica se visualizzare \#N/A come valore vuoto. |
| [getElevation()](#getElevation--) | Rappresenta l'elevazione della visualizzazione del grafico 3-D, in gradi. |
| [getFilteredNSeries()](#getFilteredNSeries--) | Ottiene una collezione [SeriesCollection](../../com.aspose.cells/seriescollection) che rappresenta le serie di dati filtrate nel grafico. |
| [getFirstSliceAngle()](#getFirstSliceAngle--) | Ottiene l'angolo della prima fetta di grafico a torta o a ciambella, in gradi (in senso orario dal verticale). |
| [getFloor()](#getFloor--) | Restituisce un oggetto [getFloor()](../../com.aspose.cells/chart\#getFloor--) che rappresenta le pareti di un grafico 3-D. |
| [getGapDepth()](#getGapDepth--) | Ottiene la distanza tra le serie di dati in un grafico 3-D, come percentuale della larghezza del marcatore. |
| [getGapWidth()](#getGapWidth--) | Restituisce o imposta lo spazio tra i raggruppamenti di barre o colonne, come percentuale della larghezza della barra o della colonna. |
| [getHeightPercent()](#getHeightPercent--) | Restituisce o imposta l'altezza di un grafico 3-D come percentuale della larghezza del grafico (tra il 5% e il 500%). |
| [getHidePivotFieldButtons()](#getHidePivotFieldButtons--) | Indica se nascondere i pulsanti dei campi del grafico pivot solo quando il grafico è un PivotChart. |
| [getIs3D()](#getIs3D--) | Indica se il grafico è un grafico 3D. |
| [getLegend()](#getLegend--) | Ottiene la legenda del grafico. |
| [getLine()](#getLine--) | Ottiene la linea. |
| [getNSeries()](#getNSeries--) | Ottiene una collezione [SeriesCollection](../../com.aspose.cells/seriescollection) che rappresenta le serie di dati nel grafico. |
| [getName()](#getName--) | Ottiene il nome del grafico. |
| [getPageSetup()](#getPageSetup--) | Rappresenta la descrizione dell'impostazione pagina in questo grafico. |
| [getPerspective()](#getPerspective--) | Restituisce o imposta la prospettiva per la visualizzazione del grafico tridimensionale three\u9225\u6178. |
| [getPivotOptions()](#getPivotOptions--) | Specifica i controlli pivot che appaiono sul grafico |
| [getPivotSource()](#getPivotSource--) | La fonte è i dati della tabella pivot. |
| [getPlacement()](#getPlacement--) | Rappresenta il modo in cui il grafico è collegato alle celle sottostanti. |
| [getPlotArea()](#getPlotArea--) | Ottiene l'area di tracciamento del grafico che include le etichette dei tic dell'asse. |
| [getPlotBy()](#getPlotBy--) | Ottiene se il tracciato è per riga o colonna. |
| [getPlotEmptyCellsType()](#getPlotEmptyCellsType--) | Ottiene come tracciare le celle vuote. |
| [getPlotVisibleCells()](#getPlotVisibleCells--) | Indica se tracciare solo le celle visibili. |
| [getPlotVisibleCellsOnly()](#getPlotVisibleCellsOnly--) | Indica se tracciare solo le celle visibili. |
| [getPrintSize()](#getPrintSize--) | Ottiene le dimensioni della grafica stampata. |
| [getRightAngleAxes()](#getRightAngleAxes--) | Vero se gli assi del grafico sono perpendicolari. |
| [getRotationAngle()](#getRotationAngle--) | Rappresenta la rotazione della vista del grafico 3-D (la rotazione dell'area del tracciato attorno all'asse z, in gradi). |
| [getSecondCategoryAxis()](#getSecondCategoryAxis--) | Ottiene il secondo asse X del grafico. |
| [getSecondValueAxis()](#getSecondValueAxis--) | Ottiene il secondo asse Y del grafico. |
| [getSeriesAxis()](#getSeriesAxis--) | Ottiene l'asse delle serie del grafico. |
| [getShapes()](#getShapes--) | Restituisce tutte le forme di disegno in questo grafico. |
| [getShowDataTable()](#getShowDataTable--) | Ottiene un valore che indica se il grafico visualizza una tabella dati. |
| [getShowLegend()](#getShowLegend--) | Ottiene un valore che indica se la legenda del grafico verrà visualizzata. |
| [getSideWall()](#getSideWall--) | Restituisce un oggetto [getWalls()](../../com.aspose.cells/chart\#getWalls--) che rappresenta la parete laterale di un grafico 3-D. |
| [getSizeWithWindow()](#getSizeWithWindow--) | Vero se Microsoft Excel ridimensiona il grafico per corrispondere alle dimensioni della finestra del foglio del grafico. |
| [getStyle()](#getStyle--) | Ottiene lo stile incorporato. |
| [getSubTitle()](#getSubTitle--) | Ottiene il sottotitolo del grafico. |
| [getTitle()](#getTitle--) | Ottiene il titolo del grafico. |
| [getType()](#getType--) | Ottiene il tipo di un grafico. |
| [getValueAxis()](#getValueAxis--) | Ottiene l'asse Y del grafico. |
| [getWalls()](#getWalls--) | Restituisce un oggetto [getWalls()](../../com.aspose.cells/chart\#getWalls--) che rappresenta le pareti di un grafico 3-D. |
| [getWallsAndGridlines2D()](#getWallsAndGridlines2D--) | Vero se le linee della griglia sono disegnate bidimensionalmente su un grafico 3-D. |
| [getWorksheet()](#getWorksheet--) | Ottiene il foglio di lavoro che contiene questo grafico. |
| [hasAxis(int aixsType, boolean isPrimary)](#hasAxis-int-boolean-) | Restituisce quali assi esistono nel grafico. |
| [hashCode()](#hashCode--) |  |
| [isCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)](#isCellReferedByChart-int-int-int-) | Restituisce se la cella a cui fa riferimento il grafico. |
| [isChartDataChanged()](#isChartDataChanged--) | Rileva se la fonte dati di un grafico è cambiata. |
| [isRectangularCornered()](#isRectangularCornered--) | Ottiene un valore che indica se l'area del grafico ha angoli rettangolari. |
| [isReferedByChart(int rowIndex, int columnIndex)](#isReferedByChart-int-int-) | Restituisce se la cella è riferita dal grafico. |
| [move(int topRow, int leftColumn, int bottomRow, int rightColumn)](#move-int-int-int-int-) | Sposta il grafico in una posizione specificata. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshPivotData()](#refreshPivotData--) | Aggiorna i dati del grafico dalla tabella pivot. |
| [setAutoScaling(boolean value)](#setAutoScaling-boolean-) | Vero se Microsoft Excel scala un grafico 3D in modo che sia più vicino in dimensioni al grafico 2D equivalente. |
| [setChartDataRange(String area, boolean isVertical)](#setChartDataRange-java.lang.String-boolean-) | Specifica l'intervallo di dati per un grafico. |
| [setDepthPercent(int value)](#setDepthPercent-int-) | Rappresenta la profondità di un grafico 3-D come percentuale della larghezza del grafico (tra il 20% e il 2000%). |
| [setDisplayNaAsBlank(boolean value)](#setDisplayNaAsBlank-boolean-) | Indica se visualizzare \#N/A come valore vuoto. |
| [setElevation(int value)](#setElevation-int-) | Rappresenta l'elevazione della visualizzazione del grafico 3-D, in gradi. |
| [setFirstSliceAngle(int value)](#setFirstSliceAngle-int-) | Imposta l'angolo della prima fetta di un grafico a torta o a ciambella, in gradi (in senso orario dalla verticale). |
| [setGapDepth(int value)](#setGapDepth-int-) | Imposta la distanza tra le serie di dati in un grafico 3-D, come percentuale della larghezza del marcatore. |
| [setGapWidth(int value)](#setGapWidth-int-) | Restituisce o imposta lo spazio tra i raggruppamenti di barre o colonne, come percentuale della larghezza della barra o della colonna. |
| [setHeightPercent(int value)](#setHeightPercent-int-) | Restituisce o imposta l'altezza di un grafico 3-D come percentuale della larghezza del grafico (tra il 5% e il 500%). |
| [setHidePivotFieldButtons(boolean value)](#setHidePivotFieldButtons-boolean-) | Indica se nascondere i pulsanti dei campi del grafico pivot solo quando il grafico è un PivotChart. |
| [setName(String value)](#setName-java.lang.String-) | Imposta il nome del grafico. |
| [setPerspective(short value)](#setPerspective-short-) | Restituisce o imposta la prospettiva per la visualizzazione del grafico tridimensionale three\u9225\u6178. |
| [setPivotSource(String value)](#setPivotSource-java.lang.String-) | La fonte è i dati della tabella pivot. |
| [setPlacement(int value)](#setPlacement-int-) | Rappresenta il modo in cui il grafico è collegato alle celle sottostanti. |
| [setPlotEmptyCellsType(int value)](#setPlotEmptyCellsType-int-) | Imposta come tracciare le celle vuote. |
| [setPlotVisibleCells(boolean value)](#setPlotVisibleCells-boolean-) | Indica se tracciare solo le celle visibili. |
| [setPlotVisibleCellsOnly(boolean value)](#setPlotVisibleCellsOnly-boolean-) | Indica se tracciare solo le celle visibili. |
| [setPrintSize(int value)](#setPrintSize-int-) | Imposta la dimensione stampata del grafico. |
| [setRectangularCornered(boolean value)](#setRectangularCornered-boolean-) | Imposta un valore che indica se l'area del grafico ha angoli rettangolari. |
| [setRightAngleAxes(boolean value)](#setRightAngleAxes-boolean-) | Vero se gli assi del grafico sono perpendicolari. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Rappresenta la rotazione della vista del grafico 3-D (la rotazione dell'area del tracciato attorno all'asse z, in gradi). |
| [setShowDataTable(boolean value)](#setShowDataTable-boolean-) | Imposta un valore che indica se il grafico visualizza una tabella dati. |
| [setShowLegend(boolean value)](#setShowLegend-boolean-) | Imposta un valore che indica se la legenda del grafico verrà visualizzata. |
| [setSizeWithWindow(boolean value)](#setSizeWithWindow-boolean-) | Vero se Microsoft Excel ridimensiona il grafico per corrispondere alle dimensioni della finestra del foglio del grafico. |
| [setStyle(int value)](#setStyle-int-) | Imposta lo stile predefinito. |
| [setType(int value)](#setType-int-) | Imposta il tipo di un grafico. |
| [setWallsAndGridlines2D(boolean value)](#setWallsAndGridlines2D-boolean-) | Vero se le linee della griglia sono disegnate bidimensionalmente su un grafico 3-D. |
| [switchRowColumn()](#switchRowColumn--) | Scambia riga/colonna. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | Crea l'immagine del grafico e la salva in uno stream nel formato specificato. |
| [toImage(String imageFile)](#toImage-java.lang.String-) | Crea l'immagine del grafico e la salva in un file. |
| [toImage(String imageFile, ImageFormat imageFormat)](#toImage-java.lang.String-com.aspose.cells.ImageFormat-) | Crea l'immagine del grafico e la salva in un file nel formato specificato. |
| [toImage(String imageFile, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | Crea l'immagine del grafico e la salva in un file. |
| [toImage(String imageFile, int imageType)](#toImage-java.lang.String-int-) | Crea l'immagine del grafico e la salva in un file nel tipo di immagine specificato. |
| [toImage(String imageFile, long jpegQuality)](#toImage-java.lang.String-long-) | Crea l'immagine del grafico e la salva in un file nel formato JPEG. |
| [toPdf(OutputStream stream)](#toPdf-java.io.OutputStream-) | Crea il PDF del grafico e lo salva in uno stream. |
| [toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)](#toPdf-java.io.OutputStream-float-float-int-int-) | Crea il PDF del grafico e lo salva in uno stream. |
| [toPdf(String fileName)](#toPdf-java.lang.String-) | Salva il grafico in un file PDF. |
| [toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)](#toPdf-java.lang.String-float-float-int-int-) | Salva il grafico in un file PDF. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### calculate() {#calculate--}
```
public void calculate()
```


Calcola le posizioni personalizzate dell'area del grafico e degli assi se le loro posizioni sono assegnate automaticamente.

### calculate(ChartCalculateOptions calculateOptions) {#calculate-com.aspose.cells.ChartCalculateOptions-}
```
public void calculate(ChartCalculateOptions calculateOptions)
```


Calcola la posizione personalizzata dell'area del grafico e degli assi se le loro posizioni sono assegnate automaticamente, con le Opzioni di Calcolo del Grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| calculateOptions | [ChartCalculateOptions](../../com.aspose.cells/chartcalculateoptions) |  |

### changeTemplate(byte[] data) {#changeTemplate-byte---}
```
public void changeTemplate(byte[] data)
```


Cambia il tipo di grafico con un modello predefinito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dati | byte[] | I dati del file modello di grafico (.crtx). |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getActualChartSize() {#getActualChartSize--}
```
public int[] getActualChartSize()
```


Ottiene le dimensioni effettive del grafico in unità di pixel.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo Chart.getActualSize(). Questa proprietà sarà rimossa 12 mesi dopo a partire da luglio 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int[] - Dimensione reale in un array (larghezza e altezza). [0] è la larghezza; [1] è l'altezza.
### getActualSize() {#getActualSize--}
```
public int[] getActualSize()
```


Ottiene le dimensioni effettive del grafico in unità di pixel.

**Returns:**
int[] - Dimensione reale in un array (larghezza e altezza). [0] è la larghezza; [1] è l'altezza.
### getAutoScaling() {#getAutoScaling--}
```
public boolean getAutoScaling()
```


Vero se Microsoft Excel scala un grafico 3-D in modo che sia più vicino in dimensione al grafico 2-D equivalente. La proprietà RightAngleAxes deve essere Vero.

**Returns:**
boolean
### getBackWall() {#getBackWall--}
```
public Walls getBackWall()
```


Restituisce un oggetto [getWalls()](../../com.aspose.cells/chart\#getWalls--) che rappresenta la parete posteriore di un grafico 3D.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getCategoryAxis() {#getCategoryAxis--}
```
public Axis getCategoryAxis()
```


Ottiene l'asse X del grafico.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getChartArea() {#getChartArea--}
```
public ChartArea getChartArea()
```


Ottiene l'area del grafico nel foglio di lavoro.

**Returns:**
[ChartArea](../../com.aspose.cells/chartarea)
### getChartDataRange() {#getChartDataRange--}
```
public String getChartDataRange()
```


Ottiene l'intervallo della fonte dati del grafico.

**Remarks**

Supporta solo intervalli. Se Series.Values, Name e XValues sono in un intervallo continuo, verrà restituito un intervallo che li contiene.

**Returns:**
java.lang.String - La fonte dei dati.
### getChartDataTable() {#getChartDataTable--}
```
public ChartDataTable getChartDataTable()
```


Rappresenta la tabella dei dati del grafico.

**Returns:**
[ChartDataTable](../../com.aspose.cells/chartdatatable)
### getChartObject() {#getChartObject--}
```
public ChartShape getChartObject()
```


Rappresenta il chartShape;

**Returns:**
[ChartShape](../../com.aspose.cells/chartshape)
### getChartShape() {#getChartShape--}
```
public ChartShape getChartShape()
```


Rappresenta il chartShape;

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà **Aspose.Cells.Charts.Chart.ChartObject**. Questa proprietà sarà rimossa 12 mesi dopo a partire da gennaio 2012. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

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


Rappresenta la profondità di un grafico 3-D come percentuale della larghezza del grafico (tra il 20% e il 2000%).

**Returns:**
int
### getDisplayNaAsBlank() {#getDisplayNaAsBlank--}
```
public boolean getDisplayNaAsBlank()
```


Indica se visualizzare \#N/A come valore vuoto.

**Returns:**
boolean
### getElevation() {#getElevation--}
```
public int getElevation()
```


Rappresenta l'elevazione della visualizzazione del grafico 3-D, in gradi.

**Remarks**

L'elevazione del grafico è l'altezza a cui visualizzi il grafico, in gradi. Il valore predefinito è 15 per la maggior parte dei tipi di grafico. Il valore di questa proprietà deve essere compreso tra -90 e 90, eccetto per i grafici a barre 3-D, dove deve essere compreso tra 0 e 44.

**Returns:**
int
### getFilteredNSeries() {#getFilteredNSeries--}
```
public SeriesCollection getFilteredNSeries()
```


Ottiene una collezione [SeriesCollection](../../com.aspose.cells/seriescollection) che rappresenta le serie di dati filtrate nel grafico.

**Returns:**
[SeriesCollection](../../com.aspose.cells/seriescollection)
### getFirstSliceAngle() {#getFirstSliceAngle--}
```
public int getFirstSliceAngle()
```


Restituisce l'angolo della prima fetta di grafico a torta o di grafico a ciambella, in gradi (in senso orario dal verticale). Si applica solo a grafici a torta, a torta 3-D e a ciambella, da 0 a 360.

**Returns:**
int
### getFloor() {#getFloor--}
```
public Floor getFloor()
```


Restituisce un oggetto [getFloor()](../../com.aspose.cells/chart\#getFloor--) che rappresenta le pareti di un grafico 3-D.

**Remarks**

Questa proprietà non si applica ai grafici a torta 3-D.

**Returns:**
[Floor](../../com.aspose.cells/floor)
### getGapDepth() {#getGapDepth--}
```
public int getGapDepth()
```


Restituisce la distanza tra le serie di dati in un grafico 3-D, come percentuale della larghezza del marcatore. Il valore di questa proprietà deve essere compreso tra 0 e 500.

**Returns:**
int
### getGapWidth() {#getGapWidth--}
```
public int getGapWidth()
```


Restituisce o imposta lo spazio tra i raggruppamenti di barre o colonne, come percentuale della larghezza della barra o della colonna. Il valore di questa proprietà deve essere compreso tra 0 e 500.

**Returns:**
int
### getHeightPercent() {#getHeightPercent--}
```
public int getHeightPercent()
```


Restituisce o imposta l'altezza di un grafico 3-D come percentuale della larghezza del grafico (tra il 5% e il 500%).

**Returns:**
int
### getHidePivotFieldButtons() {#getHidePivotFieldButtons--}
```
public boolean getHidePivotFieldButtons()
```


Indica se nascondere i pulsanti dei campi del grafico pivot solo quando il grafico è un PivotChart.

**Returns:**
boolean
### getIs3D() {#getIs3D--}
```
public boolean getIs3D()
```


Indica se il grafico è un grafico 3D.

**Returns:**
boolean
### getLegend() {#getLegend--}
```
public Legend getLegend()
```


Ottiene la legenda del grafico.

**Returns:**
[Legend](../../com.aspose.cells/legend)
### getLine() {#getLine--}
```
public Line getLine()
```


Ottiene la linea.

**Returns:**
[Line](../../com.aspose.cells/line)
### getNSeries() {#getNSeries--}
```
public SeriesCollection getNSeries()
```


Ottiene una collezione [SeriesCollection](../../com.aspose.cells/seriescollection) che rappresenta le serie di dati nel grafico.

**Returns:**
[SeriesCollection](../../com.aspose.cells/seriescollection)
### getName() {#getName--}
```
public String getName()
```


Ottiene il nome del grafico.

**Returns:**
java.lang.String
### getPageSetup() {#getPageSetup--}
```
public PageSetup getPageSetup()
```


Rappresenta la descrizione dell'impostazione pagina in questo grafico.

**Returns:**
[PageSetup](../../com.aspose.cells/pagesetup)
### getPerspective() {#getPerspective--}
```
public short getPerspective()
```


Restituisce o imposta la prospettiva per la visualizzazione del grafico tridimensionale. Deve essere compreso tra 0 e 100. Questa proprietà è ignorata se la proprietà RightAngleAxes è True.

**Returns:**
short
### getPivotOptions() {#getPivotOptions--}
```
public PivotOptions getPivotOptions()
```


Specifica i controlli pivot che appaiono sul grafico

**Returns:**
[PivotOptions](../../com.aspose.cells/pivotoptions)
### getPivotSource() {#getPivotSource--}
```
public String getPivotSource()
```


La fonte è i dati della tabella pivot. Se PivotSource non è vuoto, il grafico è un PivotChart.

**Remarks**

Se la tabella pivot "PivotTable1" nel foglio di lavoro "Sheet1" nel file "Book1.xls". Il pivotSource potrebbe essere "[Book1.xls]Sheet1!PivotTable1" se il grafico e la tabella pivot non si trovano nella stessa cartella di lavoro. Se imposti questa proprietà, l'impostazione precedente della fonte dati verrà persa.

**Returns:**
java.lang.String
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


Rappresenta il modo in cui il grafico è collegato alle celle sottostanti.

Vedi [PlacementType](../../com.aspose.cells/placementtype).

**Returns:**
int
### getPlotArea() {#getPlotArea--}
```
public PlotArea getPlotArea()
```


Ottiene l'area di tracciamento del grafico che include le etichette dei tic dell'asse.

**Remarks**

**Returns:**
[PlotArea](../../com.aspose.cells/plotarea)
### getPlotBy() {#getPlotBy--}
```
public int getPlotBy()
```


Ottiene se il tracciato è per riga o colonna.

Vedi [PlotDataByType](../../com.aspose.cells/plotdatabytype).

**Returns:**
int
### getPlotEmptyCellsType() {#getPlotEmptyCellsType--}
```
public int getPlotEmptyCellsType()
```


Ottiene come tracciare le celle vuote.

Vedi [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Returns:**
int
### getPlotVisibleCells() {#getPlotVisibleCells--}
```
public boolean getPlotVisibleCells()
```


Indica se tracciare solo le celle visibili.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà **PlotVisibleCellsOnly**. Questo metodo sarà rimosso 12 mesi dopo a partire da dicembre 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
boolean
### getPlotVisibleCellsOnly() {#getPlotVisibleCellsOnly--}
```
public boolean getPlotVisibleCellsOnly()
```


Indica se tracciare solo le celle visibili.

**Returns:**
boolean
### getPrintSize() {#getPrintSize--}
```
public int getPrintSize()
```


Ottiene le dimensioni della grafica stampata.

Vedi [PrintSizeType](../../com.aspose.cells/printsizetype).

**Returns:**
int
### getRightAngleAxes() {#getRightAngleAxes--}
```
public boolean getRightAngleAxes()
```


Vero se gli assi del grafico sono a angolo retto. Si applica solo ai grafici 3-D (eccetto Column3D e grafici a torta 3-D).

**Remarks**

Se questa proprietà è Vero, la proprietà Perspective è ignorata.

**Returns:**
boolean
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Rappresenta la rotazione della vista del grafico 3-D (la rotazione dell'area del tracciato attorno all'asse z, in gradi).

**Remarks**

Il valore di questa proprietà deve essere compreso tra 0 e 360, eccetto per i grafici a barre 3-D, dove il valore deve essere compreso tra 0 e 44. Il valore predefinito è 20. Si applica solo ai grafici 3-D.

**Returns:**
int
### getSecondCategoryAxis() {#getSecondCategoryAxis--}
```
public Axis getSecondCategoryAxis()
```


Ottiene il secondo asse X del grafico.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getSecondValueAxis() {#getSecondValueAxis--}
```
public Axis getSecondValueAxis()
```


Ottiene il secondo asse Y del grafico.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getSeriesAxis() {#getSeriesAxis--}
```
public Axis getSeriesAxis()
```


Ottiene l'asse delle serie del grafico.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getShapes() {#getShapes--}
```
public ShapeCollection getShapes()
```


Restituisce tutte le forme di disegno in questo grafico.

**Returns:**
[ShapeCollection](../../com.aspose.cells/shapecollection)
### getShowDataTable() {#getShowDataTable--}
```
public boolean getShowDataTable()
```


Ottiene un valore che indica se il grafico visualizza una tabella dati.

**Returns:**
boolean
### getShowLegend() {#getShowLegend--}
```
public boolean getShowLegend()
```


Restituisce un valore che indica se la legenda del grafico verrà visualizzata. Il valore predefinito è vero.

**Returns:**
boolean
### getSideWall() {#getSideWall--}
```
public Walls getSideWall()
```


Restituisce un oggetto [getWalls()](../../com.aspose.cells/chart\#getWalls--) che rappresenta la parete laterale di un grafico 3-D.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getSizeWithWindow() {#getSizeWithWindow--}
```
public boolean getSizeWithWindow()
```


Vero se Microsoft Excel ridimensiona il grafico per corrispondere alle dimensioni della finestra del foglio del grafico.

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public int getStyle()
```


Ottiene lo stile incorporato.

**Remarks**

Deve essere compreso tra 1 e 48. Restituisce -1 se non è impostato.

**Returns:**
int
### getSubTitle() {#getSubTitle--}
```
public Title getSubTitle()
```


Restituisce il sottotitolo del grafico. Si applica solo ai file ODS.

**Returns:**
[Title](../../com.aspose.cells/title)
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Ottiene il titolo del grafico.

**Returns:**
[Title](../../com.aspose.cells/title)
### getType() {#getType--}
```
public int getType()
```


Ottiene il tipo di un grafico.

Vedi [ChartType](../../com.aspose.cells/charttype).

**Returns:**
int
### getValueAxis() {#getValueAxis--}
```
public Axis getValueAxis()
```


Ottiene l'asse Y del grafico.

**Returns:**
[Axis](../../com.aspose.cells/axis)
### getWalls() {#getWalls--}
```
public Walls getWalls()
```


Restituisce un oggetto [getWalls()](../../com.aspose.cells/chart\#getWalls--) che rappresenta le pareti di un grafico 3-D.

**Remarks**

Questa proprietà non si applica ai grafici a torta 3-D.

**Returns:**
[Walls](../../com.aspose.cells/walls)
### getWallsAndGridlines2D() {#getWallsAndGridlines2D--}
```
public boolean getWallsAndGridlines2D()
```


Vero se le linee della griglia sono disegnate bidimensionalmente su un grafico 3-D.

**Returns:**
boolean
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Ottiene il foglio di lavoro che contiene questo grafico.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hasAxis(int aixsType, boolean isPrimary) {#hasAxis-int-boolean-}
```
public boolean hasAxis(int aixsType, boolean isPrimary)
```


Restituisce quali assi esistono nel grafico.

**Remarks**

Normalmente, Pie, PieExploded, PiePie, PieBar, Pie3D, Pie3DExploded, Doughnut, DoughnutExploded non hanno assi.

**Parameters:**
| Parametro | Tipo | Descrizione |
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


Restituisce se la cella a cui fa riferimento il grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | int | L'indice del foglio -1 indica il foglio di lavoro che contiene il grafico corrente. |
| rowIndex | int | L'indice della riga |
| columnIndex | int | L'indice della colonna |

**Returns:**
boolean -
### isChartDataChanged() {#isChartDataChanged--}
```
public boolean isChartDataChanged()
```


Rileva se la fonte dati di un grafico è cambiata.

**Remarks**

Il metodo rileva le modifiche nella fonte dati del grafico prima di renderizzare il grafico in formato immagine. Alla prima chiamata a Chart.toImage, i dati di origine del grafico (ad es. XValuesParseData, ValuesParseData) verranno registrati. Prima di chiamare nuovamente il metodo Chart.toImage, chiamare il metodo IsChartDataChanged per verificare se il grafico necessita di un nuovo rendering.

**Returns:**
boolean - Restituisce true se il grafico è cambiato, altrimenti restituisce false
### isRectangularCornered() {#isRectangularCornered--}
```
public boolean isRectangularCornered()
```


Restituisce un valore che indica se l'area del grafico ha angoli rettangolari. Il valore predefinito è true.

**Returns:**
boolean
### isReferedByChart(int rowIndex, int columnIndex) {#isReferedByChart-int-int-}
```
public boolean isReferedByChart(int rowIndex, int columnIndex)
```


Restituisce se la cella è riferita dal grafico.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo IsCellReferedByChart(int,int,int). Questo metodo sarà rimosso 12 mesi dopo, a partire da aprile 2023. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | L'indice della riga |
| columnIndex | int | L'indice della colonna |

**Returns:**
boolean -
### move(int topRow, int leftColumn, int bottomRow, int rightColumn) {#move-int-int-int-int-}
```
public void move(int topRow, int leftColumn, int bottomRow, int rightColumn)
```


Sposta il grafico in una posizione specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| bottomRow | int | Indice della riga in basso a destra |
| rightColumn | int | Indice della colonna in basso a destra |

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


Aggiorna i dati del grafico dalla tabella pivot.

**Remarks**

Raccoglieremo i dati dalla fonte dati pivot al report della tabella pivot. Questo metodo è usato solo per raccogliere tutti i dati in un grafico pivot.

### setAutoScaling(boolean value) {#setAutoScaling-boolean-}
```
public void setAutoScaling(boolean value)
```


Vero se Microsoft Excel scala un grafico 3-D in modo che sia più vicino in dimensione al grafico 2-D equivalente. La proprietà RightAngleAxes deve essere Vero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setChartDataRange(String area, boolean isVertical) {#setChartDataRange-java.lang.String-boolean-}
```
public void setChartDataRange(String area, boolean isVertical)
```


Specifica l'intervallo di dati per un grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| area | java.lang.String | Specifica i valori da cui tracciare la serie di dati |
| isVertical | boolean | Specifica se tracciare la serie da un intervallo di valori di celle per riga o per colonna. |

### setDepthPercent(int value) {#setDepthPercent-int-}
```
public void setDepthPercent(int value)
```


Rappresenta la profondità di un grafico 3-D come percentuale della larghezza del grafico (tra il 20% e il 2000%).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setDisplayNaAsBlank(boolean value) {#setDisplayNaAsBlank-boolean-}
```
public void setDisplayNaAsBlank(boolean value)
```


Indica se visualizzare \#N/A come valore vuoto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setElevation(int value) {#setElevation-int-}
```
public void setElevation(int value)
```


Rappresenta l'elevazione della visualizzazione del grafico 3-D, in gradi.

**Remarks**

L'elevazione del grafico è l'altezza a cui visualizzi il grafico, in gradi. Il valore predefinito è 15 per la maggior parte dei tipi di grafico. Il valore di questa proprietà deve essere compreso tra -90 e 90, eccetto per i grafici a barre 3-D, dove deve essere compreso tra 0 e 44.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setFirstSliceAngle(int value) {#setFirstSliceAngle-int-}
```
public void setFirstSliceAngle(int value)
```


Imposta l'angolo della prima fetta di grafico a torta o di grafico a ciambella, in gradi (orario dalla verticale). Si applica solo a grafici a torta, a torta 3D e a ciambella, da 0 a 360.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setGapDepth(int value) {#setGapDepth-int-}
```
public void setGapDepth(int value)
```


Imposta la distanza tra le serie di dati in un grafico 3D, come percentuale della larghezza del marcatore. Il valore di questa proprietà deve essere compreso tra 0 e 500.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setGapWidth(int value) {#setGapWidth-int-}
```
public void setGapWidth(int value)
```


Restituisce o imposta lo spazio tra i raggruppamenti di barre o colonne, come percentuale della larghezza della barra o della colonna. Il valore di questa proprietà deve essere compreso tra 0 e 500.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setHeightPercent(int value) {#setHeightPercent-int-}
```
public void setHeightPercent(int value)
```


Restituisce o imposta l'altezza di un grafico 3-D come percentuale della larghezza del grafico (tra il 5% e il 500%).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setHidePivotFieldButtons(boolean value) {#setHidePivotFieldButtons-boolean-}
```
public void setHidePivotFieldButtons(boolean value)
```


Indica se nascondere i pulsanti dei campi del grafico pivot solo quando il grafico è un PivotChart.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Imposta il nome del grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setPerspective(short value) {#setPerspective-short-}
```
public void setPerspective(short value)
```


Restituisce o imposta la prospettiva per la visualizzazione del grafico tridimensionale. Deve essere compreso tra 0 e 100. Questa proprietà è ignorata se la proprietà RightAngleAxes è True.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | short |  |

### setPivotSource(String value) {#setPivotSource-java.lang.String-}
```
public void setPivotSource(String value)
```


La fonte è i dati della tabella pivot. Se PivotSource non è vuoto, il grafico è un PivotChart.

**Remarks**

Se la tabella pivot "PivotTable1" nel foglio di lavoro "Sheet1" nel file "Book1.xls". Il pivotSource potrebbe essere "[Book1.xls]Sheet1!PivotTable1" se il grafico e la tabella pivot non si trovano nella stessa cartella di lavoro. Se imposti questa proprietà, l'impostazione precedente della fonte dati verrà persa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Rappresenta il modo in cui il grafico è collegato alle celle sottostanti.

Vedi [PlacementType](../../com.aspose.cells/placementtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPlotEmptyCellsType(int value) {#setPlotEmptyCellsType-int-}
```
public void setPlotEmptyCellsType(int value)
```


Imposta come tracciare le celle vuote.

Vedi [PlotEmptyCellsType](../../com.aspose.cells/plotemptycellstype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPlotVisibleCells(boolean value) {#setPlotVisibleCells-boolean-}
```
public void setPlotVisibleCells(boolean value)
```


Indica se tracciare solo le celle visibili.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà **PlotVisibleCellsOnly**. Questo metodo sarà rimosso 12 mesi dopo a partire da dicembre 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPlotVisibleCellsOnly(boolean value) {#setPlotVisibleCellsOnly-boolean-}
```
public void setPlotVisibleCellsOnly(boolean value)
```


Indica se tracciare solo le celle visibili.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPrintSize(int value) {#setPrintSize-int-}
```
public void setPrintSize(int value)
```


Imposta la dimensione stampata del grafico.

Vedi [PrintSizeType](../../com.aspose.cells/printsizetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setRectangularCornered(boolean value) {#setRectangularCornered-boolean-}
```
public void setRectangularCornered(boolean value)
```


Imposta un valore che indica se l'area del grafico ha angoli rettangolari. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRightAngleAxes(boolean value) {#setRightAngleAxes-boolean-}
```
public void setRightAngleAxes(boolean value)
```


Vero se gli assi del grafico sono a angolo retto. Si applica solo ai grafici 3-D (eccetto Column3D e grafici a torta 3-D).

**Remarks**

Se questa proprietà è Vero, la proprietà Perspective è ignorata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Rappresenta la rotazione della vista del grafico 3-D (la rotazione dell'area del tracciato attorno all'asse z, in gradi).

**Remarks**

Il valore di questa proprietà deve essere compreso tra 0 e 360, eccetto per i grafici a barre 3-D, dove il valore deve essere compreso tra 0 e 44. Il valore predefinito è 20. Si applica solo ai grafici 3-D.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setShowDataTable(boolean value) {#setShowDataTable-boolean-}
```
public void setShowDataTable(boolean value)
```


Imposta un valore che indica se il grafico visualizza una tabella dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowLegend(boolean value) {#setShowLegend-boolean-}
```
public void setShowLegend(boolean value)
```


Imposta un valore che indica se la legenda del grafico verrà visualizzata. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSizeWithWindow(boolean value) {#setSizeWithWindow-boolean-}
```
public void setSizeWithWindow(boolean value)
```


Vero se Microsoft Excel ridimensiona il grafico per corrispondere alle dimensioni della finestra del foglio del grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```


Imposta lo stile predefinito.

**Remarks**

Deve essere compreso tra 1 e 48. Restituisce -1 se non è impostato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Imposta il tipo di un grafico.

Vedi [ChartType](../../com.aspose.cells/charttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setWallsAndGridlines2D(boolean value) {#setWallsAndGridlines2D-boolean-}
```
public void setWallsAndGridlines2D(boolean value)
```


Vero se le linee della griglia sono disegnate bidimensionalmente su un grafico 3-D.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### switchRowColumn() {#switchRowColumn--}
```
public boolean switchRowColumn()
```


Scambia riga/colonna.

**Returns:**
boolean - False indica che lo scambio riga/colonna fallisce.
### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


Crea l'immagine del grafico e la salva in uno stream nel formato specificato.

**Remarks**

Il formato dell'immagine è specificato utilizzando `options.ImageFormat`. I seguenti formati sono supportati: ImageFormat.Bmp, ImageFormat.Gif, ImageFormat.Png, ImageFormat.Jpeg, ImageFormat.Tiff, ImageFormat.Emf.

Se la larghezza o l'altezza è zero o il grafico non è supportato secondo l'Elenco dei grafici supportati, questo metodo non farà nulla. Si prega di consultare [Supported Charts List][] per maggiori dettagli.


[Supported Charts List]: http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso di output. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Opzioni aggiuntive per la creazione dell'immagine |

### toImage(String imageFile) {#toImage-java.lang.String-}
```
public void toImage(String imageFile)
```


Crea l'immagine del grafico e la salva in un file. L'estensione del nome file determina il formato dell'immagine.

**Remarks**

Il formato dell'immagine è specificato utilizzando l'estensione del nome file. Ad esempio, se specifichi "myfile.png", l'immagine verrà salvata nel formato PNG. Le seguenti estensioni di file sono riconosciute: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Se la larghezza o l'altezza è zero o il grafico non è supportato secondo l'Elenco dei grafici supportati, questo metodo non farà nulla.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| imageFile | java.lang.String | Il nome file dell'immagine con percorso completo. |

### toImage(String imageFile, ImageFormat imageFormat) {#toImage-java.lang.String-com.aspose.cells.ImageFormat-}
```
public void toImage(String imageFile, ImageFormat imageFormat)
```


Crea l'immagine del grafico e la salva in un file nel formato specificato.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo Chart.ToImage(string, ImageType). Questa proprietà sarà rimossa 12 mesi dopo, a partire da luglio 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| imageFile | java.lang.String | Il nome file dell'immagine con percorso completo. |
| imageFormat | [ImageFormat](../../com.aspose.cells/imageformat) | Il formato in cui salvare l'immagine. |

### toImage(String imageFile, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String imageFile, ImageOrPrintOptions options)
```


Crea l'immagine del grafico e la salva in un file. L'estensione del nome file determina il formato dell'immagine.

**Remarks**

Il formato dell'immagine è specificato utilizzando l'estensione del nome file. Ad esempio, se specifichi "myfile.png", l'immagine verrà salvata nel formato PNG. Le seguenti estensioni di file sono riconosciute: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Se la larghezza o l'altezza è zero o il grafico non è supportato secondo l'Elenco dei grafici supportati, questo metodo non farà nulla. Si prega di consultare [Supported Charts List][] per maggiori dettagli.

**Example**

Salva in Tiff con 300 dpi e compressione CCITT4.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| imageFile | java.lang.String | Il nome file dell'immagine con percorso completo. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Opzioni aggiuntive per la creazione dell'immagine |

### toImage(String imageFile, int imageType) {#toImage-java.lang.String-int-}
```
public void toImage(String imageFile, int imageType)
```


Crea l'immagine del grafico e la salva in un file nel tipo di immagine specificato.

**Remarks**

Il tipo dell'immagine è specificato usando `imageType`. I seguenti tipi sono supportati: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Se la larghezza o l'altezza è zero o il grafico non è supportato secondo l'Elenco dei grafici supportati, questo metodo non farà nulla.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| imageFile | java.lang.String | Il nome file dell'immagine con percorso completo. |
| imageType | int | [ImageType](../../com.aspose.cells/imagetype). Il tipo di immagine in cui salvare l'immagine. |

### toImage(String imageFile, long jpegQuality) {#toImage-java.lang.String-long-}
```
public void toImage(String imageFile, long jpegQuality)
```


Crea l'immagine del grafico e la salva in un file nel formato JPEG.

**Remarks**

Se la larghezza o l'altezza è zero o il grafico non è supportato secondo l'Elenco dei grafici supportati, questo metodo non farà nulla. NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo ToImage(string,ImageOrPrintOptions) con la qualità specificata. Questo metodo sarà rimosso 12 mesi dopo, a partire da marzo 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| imageFile | java.lang.String | Il nome file dell'immagine con percorso completo. |
| jpegQuality | long | Qualità JPEG. |

### toPdf(OutputStream stream) {#toPdf-java.io.OutputStream-}
```
public void toPdf(OutputStream stream)
```


Crea il PDF del grafico e lo salva in uno stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso di output. |

### toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType) {#toPdf-java.io.OutputStream-float-float-int-int-}
```
public void toPdf(OutputStream stream, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)
```


Crea il PDF del grafico e lo salva in uno stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso di output. |
| desiredPageWidth | float | La larghezza della pagina desiderata in pollici. |
| desiredPageHeight | float | L'altezza della pagina desiderata in pollici. |
| hAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Il tipo di allineamento orizzontale del grafico nella pagina di output. |
| vAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Il tipo di allineamento verticale del grafico nella pagina di output. |

### toPdf(String fileName) {#toPdf-java.lang.String-}
```
public void toPdf(String fileName)
```


Salva il grafico in un file PDF.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | il nome del file pdf con percorso completo |

### toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType) {#toPdf-java.lang.String-float-float-int-int-}
```
public void toPdf(String fileName, float desiredPageWidth, float desiredPageHeight, int hAlignmentType, int vAlignmentType)
```


Salva il grafico in un file PDF.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | il nome del file pdf con percorso completo |
| desiredPageWidth | float | La larghezza della pagina desiderata in pollici. |
| desiredPageHeight | float | L'altezza della pagina desiderata in pollici. |
| hAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Il tipo di allineamento orizzontale del grafico nella pagina di output. |
| vAlignmentType | int | [PageLayoutAlignmentType](../../com.aspose.cells/pagelayoutalignmenttype). Il tipo di allineamento verticale del grafico nella pagina di output. |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

