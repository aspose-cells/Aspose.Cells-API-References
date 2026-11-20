---
title: "Series"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta una singola serie di dati in un grafico."
type: docs
url: /it/java/com.aspose.cells/series/
---

**Inheritance:**
java.lang.Object
```
public class Series
```

Incapsula l'oggetto che rappresenta una singola serie di dati in un grafico.

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
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Rappresenta l'area di sfondo dell'oggetto Series. |
| [getBar3DShapeType()](#getBar3DShapeType--) | Ottiene il tipo di forma 3D utilizzato con il grafico a barre o colonne 3D. |
| [getBorder()](#getBorder--) | Rappresenta il bordo di un oggetto Series. |
| [getBubbleScale()](#getBubbleScale--) | Ottiene il fattore di scala per le bolle nel gruppo di grafico specificato. |
| [getBubbleSizeRepresents()](#getBubbleSizeRepresents--) | Ottiene cosa rappresenta la dimensione della bolla in un grafico a bolle. |
| [getBubbleSizes()](#getBubbleSizes--) | Ottiene i valori della dimensione delle bolle della serie del grafico. |
| [getCachedCategoryValues()](#getCachedCategoryValues--) | Ottiene i valori di categoria memorizzati nella cache per la serie |
| [getCachedValues()](#getCachedValues--) | Ottiene i valori memorizzati nella cache per la serie |
| [getCategoryValues()](#getCategoryValues--) | Ottiene i valori di categoria effettivi utilizzati per tracciare ogni punto di questa serie nel grafico. |
| [getClass()](#getClass--) |  |
| [getCountOfDataValues()](#getCountOfDataValues--) | Ottiene il numero dei valori dei dati. |
| [getDataLabels()](#getDataLabels--) | Rappresenta l'oggetto DataLabels per l'ASeries specificato. |
| [getDisplayName()](#getDisplayName--) | Ottiene il nome della serie che viene visualizzato nel grafico. |
| [getDoughnutHoleSize()](#getDoughnutHoleSize--) | Restituisce o imposta la dimensione del foro in un gruppo di grafico a ciambella. |
| [getDownBars()](#getDownBars--) | Restituisce un oggetto [DropBars](../../com.aspose.cells/dropbars) che rappresenta le barre discendenti su un grafico a linee. |
| [getDropLines()](#getDropLines--) | Restituisce un oggetto [Line](../../com.aspose.cells/line) che rappresenta le linee di discesa per una serie sul grafico a linee o a aree. |
| [getExplosion()](#getExplosion--) | La distanza di una fetta di torta aperta dal centro del grafico a torta è espressa come percentuale del diametro della torta. |
| [getFirstSliceAngle()](#getFirstSliceAngle--) | Ottiene l'angolo della prima fetta di grafico a torta o a ciambella, in gradi (in senso orario dal verticale). |
| [getGapWidth()](#getGapWidth--) | Restituisce o imposta lo spazio tra i raggruppamenti di barre o colonne, come percentuale della larghezza della barra o della colonna. |
| [getHas3DEffect()](#getHas3DEffect--) | Vero se la serie ha un aspetto tridimensionale. |
| [getHiLoLines()](#getHiLoLines--) | Restituisce un oggetto HiLoLines che rappresenta le linee alto-basso per una serie su un grafico a linee. |
| [getLayoutProperties()](#getLayoutProperties--) | Rappresenta le proprietà del layout. |
| [getLeaderLines()](#getLeaderLines--) | Rappresenta le linee guida su un grafico. |
| [getLegendEntry()](#getLegendEntry--) | Ottiene la voce della legenda in base a questa serie. |
| [getMarker()](#getMarker--) | Ottiene il [getMarker()](../../com.aspose.cells/series\#getMarker--). |
| [getName()](#getName--) | Ottiene il nome della serie di dati. |
| [getOverlap()](#getOverlap--) | Specifica come sono posizionate le barre e le colonne. |
| [getPlotOnSecondAxis()](#getPlotOnSecondAxis--) | Indica se questa serie è tracciata sul secondo asse dei valori. |
| [getPointValues()](#getPointValues--) | Ottiene i valori effettivi utilizzati per tracciare ogni punto di questa serie nel grafico. |
| [getPoints()](#getPoints--) | Ottiene la raccolta di punti in una serie in un grafico. |
| [getSecondPlotSize()](#getSecondPlotSize--) | Restituisce o imposta la dimensione della sezione secondaria di un grafico a torta di torta o di un grafico a barra di torta, come percentuale della dimensione della torta primaria. |
| [getSeriesLines()](#getSeriesLines--) | Restituisce un oggetto SeriesLines che rappresenta le linee di serie per un grafico a barre impilate o a colonne impilate. |
| [getShadow()](#getShadow--) | Vero se la serie ha un'ombra. |
| [getShapeProperties()](#getShapeProperties--) | Ottiene l'oggetto [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) che contiene le proprietà visive della forma della Serie. |
| [getShowNegativeBubbles()](#getShowNegativeBubbles--) | Vero se le bolle negative sono visualizzate per il gruppo del grafico. |
| [getSizeRepresents()](#getSizeRepresents--) | Ottiene cosa rappresenta la dimensione della bolla in un grafico a bolle. |
| [getSmooth()](#getSmooth--) | Rappresenta l'ammorbidimento della curva. |
| [getSplitType()](#getSplitType--) | Restituisce o imposta un valore che determina quali punti dati sono nella seconda torta o barra in un grafico a torta di torta o a barra di torta. |
| [getSplitValue()](#getSplitValue--) | Restituisce o imposta un valore da utilizzare per determinare quali punti dati sono nella seconda torta o barra in un grafico a torta di torta o a barra di torta. |
| [getTrendLines()](#getTrendLines--) | Restituisce tutte le linee di tendenza di questa serie. |
| [getType()](#getType--) | Ottiene il tipo di una serie di dati. |
| [getUpBars()](#getUpBars--) | Restituisce un oggetto DropBars che rappresenta le barre ascendenti in un grafico a linee. |
| [getValues()](#getValues--) | Rappresenta i valori Y di questa serie di grafico. |
| [getValuesFormatCode()](#getValuesFormatCode--) | Rappresenta il codice di formato della NumberList dei Valori. |
| [getXErrorBar()](#getXErrorBar--) | Rappresenta la barra di errore in direzione X della serie. |
| [getXValues()](#getXValues--) | Rappresenta i valori X di questa serie di grafico. |
| [getXValuesFormatCode()](#getXValuesFormatCode--) | Rappresenta il codice di formato della NumberList dei Valori X. |
| [getYErrorBar()](#getYErrorBar--) | Rappresenta la barra di errore in direzione Y della serie. |
| [hasDropLines()](#hasDropLines--) | Vero se il grafico ha linee di discesa. |
| [hasHiLoLines()](#hasHiLoLines--) | Vero se il grafico a linee ha linee alto-basso. |
| [hasLeaderLines()](#hasLeaderLines--) | Vero se la serie ha linee guida. |
| [hasRadarAxisLabels()](#hasRadarAxisLabels--) | Vero se un grafico radar ha etichette dell'asse delle categorie. |
| [hasSeriesLines()](#hasSeriesLines--) | Vero se un grafico a colonne impilate o a barre ha linee di serie o se un grafico Pie of Pie o Bar of Pie ha linee di collegamento tra le due sezioni. |
| [hasUpDownBars()](#hasUpDownBars--) | Vero se un grafico a linee ha barre superiori e inferiori. |
| [hashCode()](#hashCode--) |  |
| [isAutoSplit()](#isAutoSplit--) | Indica se il valore soglia è automatico. |
| [isColorVaried()](#isColorVaried--) | Rappresenta se il colore dei punti è variabile. |
| [isFiltered()](#isFiltered--) | Indica se la serie è selezionata o filtrata. |
| [isVerticalValues()](#isVerticalValues--) | Indica se l'origine dati è verticale. |
| [move(int count)](#move-int-) | Sposta la serie verso l'alto o verso il basso. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBar3DShapeType(int value)](#setBar3DShapeType-int-) | Imposta il tipo di forma 3D utilizzato con il grafico a barre o colonne 3D. |
| [setBubbleScale(int value)](#setBubbleScale-int-) | Imposta il fattore di scala per le bolle nel gruppo di grafico specificato. |
| [setBubbleSizeRepresents(int value)](#setBubbleSizeRepresents-int-) | Ottiene cosa rappresenta la dimensione della bolla in un grafico a bolle. |
| [setBubbleSizes(String value)](#setBubbleSizes-java.lang.String-) | Imposta i valori di dimensione delle bolle della serie di grafico. |
| [setColorVaried(boolean value)](#setColorVaried-boolean-) | Rappresenta se il colore dei punti è variabile. |
| [setDoughnutHoleSize(int value)](#setDoughnutHoleSize-int-) | Restituisce o imposta la dimensione del foro in un gruppo di grafico a ciambella. |
| [setExplosion(int value)](#setExplosion-int-) | La distanza di una fetta di torta aperta dal centro del grafico a torta è espressa come percentuale del diametro della torta. |
| [setFiltered(boolean value)](#setFiltered-boolean-) | Indica se la serie è selezionata o filtrata. |
| [setFirstSliceAngle(short value)](#setFirstSliceAngle-short-) | Imposta l'angolo della prima fetta di un grafico a torta o a ciambella, in gradi (in senso orario dalla verticale). |
| [setGapWidth(short value)](#setGapWidth-short-) | Restituisce o imposta lo spazio tra i raggruppamenti di barre o colonne, come percentuale della larghezza della barra o della colonna. |
| [setHas3DEffect(boolean value)](#setHas3DEffect-boolean-) | Vero se la serie ha un aspetto tridimensionale. |
| [setHasDropLines(boolean value)](#setHasDropLines-boolean-) | Vero se il grafico ha linee di discesa. |
| [setHasHiLoLines(boolean value)](#setHasHiLoLines-boolean-) | Vero se il grafico a linee ha linee alto-basso. |
| [setHasLeaderLines(boolean value)](#setHasLeaderLines-boolean-) | Vero se la serie ha linee guida. |
| [setHasRadarAxisLabels(boolean value)](#setHasRadarAxisLabels-boolean-) | Vero se un grafico radar ha etichette dell'asse delle categorie. |
| [setHasSeriesLines(boolean value)](#setHasSeriesLines-boolean-) | Vero se un grafico a colonne impilate o a barre ha linee di serie o se un grafico Pie of Pie o Bar of Pie ha linee di collegamento tra le due sezioni. |
| [setHasUpDownBars(boolean value)](#setHasUpDownBars-boolean-) | Vero se un grafico a linee ha barre superiori e inferiori. |
| [setName(String value)](#setName-java.lang.String-) | Imposta il nome della serie di dati. |
| [setOverlap(short value)](#setOverlap-short-) | Specifica come sono posizionate le barre e le colonne. |
| [setPlotOnSecondAxis(boolean value)](#setPlotOnSecondAxis-boolean-) | Indica se questa serie è tracciata sul secondo asse dei valori. |
| [setSecondPlotSize(short value)](#setSecondPlotSize-short-) | Restituisce o imposta la dimensione della sezione secondaria di un grafico a torta di torta o di un grafico a barra di torta, come percentuale della dimensione della torta primaria. |
| [setShadow(boolean value)](#setShadow-boolean-) | Vero se la serie ha un'ombra. |
| [setShowNegativeBubbles(boolean value)](#setShowNegativeBubbles-boolean-) | Vero se le bolle negative sono visualizzate per il gruppo del grafico. |
| [setSizeRepresents(int value)](#setSizeRepresents-int-) | Imposta cosa rappresenta la dimensione della bolla in un grafico a bolle. |
| [setSmooth(boolean value)](#setSmooth-boolean-) | Rappresenta l'ammorbidimento della curva. |
| [setSplitType(int value)](#setSplitType-int-) | Restituisce o imposta un valore che determina quali punti dati sono nella seconda torta o barra in un grafico a torta di torta o a barra di torta. |
| [setSplitValue(double value)](#setSplitValue-double-) | Restituisce o imposta un valore da utilizzare per determinare quali punti dati sono nella seconda torta o barra in un grafico a torta di torta o a barra di torta. |
| [setType(int value)](#setType-int-) | Imposta il tipo di una serie di dati. |
| [setValues(String value)](#setValues-java.lang.String-) | Rappresenta i valori Y di questa serie di grafico. |
| [setValuesFormatCode(String value)](#setValuesFormatCode-java.lang.String-) | Rappresenta il codice di formato della NumberList dei Valori. |
| [setXValues(String value)](#setXValues-java.lang.String-) | Rappresenta i valori X di questa serie di grafico. |
| [setXValuesFormatCode(String value)](#setXValuesFormatCode-java.lang.String-) | Rappresenta il codice di formato della NumberList dei Valori X. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getArea() {#getArea--}
```
public Area getArea()
```


Rappresenta l'area di sfondo dell'oggetto Series.

**Returns:**
[Area](../../com.aspose.cells/area)
### getBar3DShapeType() {#getBar3DShapeType--}
```
public int getBar3DShapeType()
```


Ottiene il tipo di forma 3D utilizzato con il grafico a barre o colonne 3D.

Vedi [Bar3DShapeType](../../com.aspose.cells/bar3dshapetype).

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Rappresenta il bordo di un oggetto Series.

**Returns:**
[Line](../../com.aspose.cells/line)
### getBubbleScale() {#getBubbleScale--}
```
public int getBubbleScale()
```


Restituisce il fattore di scala per le bolle nel gruppo di grafico specificato. Può essere un valore intero da 0 (zero) a 300, corrispondente a una percentuale della dimensione predefinita. Si applica solo ai grafici a bolle.

**Returns:**
int
### getBubbleSizeRepresents() {#getBubbleSizeRepresents--}
```
public int getBubbleSizeRepresents()
```


Ottiene cosa rappresenta la dimensione della bolla in un grafico a bolle.

Vedi [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Aspose.Cells.Charts.Series.SizeRepresents. Questa proprietà sarà rimossa 12 mesi dopo, a partire da GENNAIO 2012. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### getBubbleSizes() {#getBubbleSizes--}
```
public String getBubbleSizes()
```


Ottiene i valori della dimensione delle bolle della serie del grafico.

**Remarks**

Solo per [ChartType.BUBBLE](../../com.aspose.cells/charttype#BUBBLE) o [ChartType.BUBBLE_3_D](../../com.aspose.cells/charttype#BUBBLE-3-D).

**Returns:**
java.lang.String
### getCachedCategoryValues() {#getCachedCategoryValues--}
```
public ArrayList getCachedCategoryValues()
```


Ottiene i valori di categoria memorizzati nella cache per la serie

**Remarks**

NOTA: Questa proprietà è attualmente solo per uso interno. Verrà modificata o rimossa nella prossima versione.

**Returns:**
java.util.ArrayList
### getCachedValues() {#getCachedValues--}
```
public ArrayList getCachedValues()
```


Ottiene i valori memorizzati nella cache per la serie

**Remarks**

NOTA: Questa proprietà è attualmente solo per uso interno. Verrà modificata o rimossa nella prossima versione.

**Returns:**
java.util.ArrayList
### getCategoryValues() {#getCategoryValues--}
```
public ChartDataValue[][] getCategoryValues()
```


Ottiene i valori di categoria effettivi utilizzati per tracciare ogni punto di questa serie nel grafico.

**Remarks**

Questa proprietà fornisce un modo comodo per ottenere i valori effettivi corrispondenti ai dati definiti da [getXValues()](../../com.aspose.cells/series#getXValues--), specialmente quando l'origine dati specificata è un collegamento esterno, una formula, ...ecc.

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


Ottiene il numero dei valori dei dati.

**Returns:**
int
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


Rappresenta l'oggetto DataLabels per l'ASeries specificato.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Ottiene il nome della serie che viene visualizzato nel grafico.

**Returns:**
java.lang.String
### getDoughnutHoleSize() {#getDoughnutHoleSize--}
```
public int getDoughnutHoleSize()
```


Restituisce o imposta la dimensione del foro in un gruppo di grafico a ciambella. La dimensione del foro è espressa come percentuale della dimensione del grafico, tra il 10% e il 90%.

**Returns:**
int
### getDownBars() {#getDownBars--}
```
public DropBars getDownBars()
```


Restituisce un oggetto [DropBars](../../com.aspose.cells/dropbars) che rappresenta le barre discendenti su un grafico a linee. Si applica solo ai grafici a linee.

**Returns:**
[DropBars](../../com.aspose.cells/dropbars)
### getDropLines() {#getDropLines--}
```
public Line getDropLines()
```


Restituisce un oggetto [Line](../../com.aspose.cells/line) che rappresenta le linee di discesa per una serie sul grafico a linee o a aree. Si applica solo ai grafici a linee o a aree.

**Returns:**
[Line](../../com.aspose.cells/line)
### getExplosion() {#getExplosion--}
```
public int getExplosion()
```


La distanza di una fetta di torta aperta dal centro del grafico a torta è espressa come percentuale del diametro della torta.

**Returns:**
int
### getFirstSliceAngle() {#getFirstSliceAngle--}
```
public short getFirstSliceAngle()
```


Restituisce l'angolo della prima fetta di grafico a torta o a ciambella, in gradi (orario dalla verticale). Si applica solo ai grafici a torta, a torta 3D e a ciambella, con valori da 0 a 360.

**Returns:**
short
### getGapWidth() {#getGapWidth--}
```
public short getGapWidth()
```


Restituisce o imposta lo spazio tra i raggruppamenti di barre o colonne, come percentuale della larghezza della barra o della colonna. Il valore di questa proprietà deve essere compreso tra 0 e 500.

**Returns:**
short
### getHas3DEffect() {#getHas3DEffect--}
```
public boolean getHas3DEffect()
```


Vero se la serie ha un aspetto tridimensionale.

**Remarks**

Si applica solo ai grafici [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) o [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Returns:**
boolean
### getHiLoLines() {#getHiLoLines--}
```
public Line getHiLoLines()
```


Restituisce un oggetto HiLoLines che rappresenta le linee alto-basso per una serie in un grafico a linee. Si applica solo ai grafici a linee.

**Returns:**
[Line](../../com.aspose.cells/line)
### getLayoutProperties() {#getLayoutProperties--}
```
public SeriesLayoutProperties getLayoutProperties()
```


Rappresenta le proprietà del layout.

**Returns:**
[SeriesLayoutProperties](../../com.aspose.cells/serieslayoutproperties)
### getLeaderLines() {#getLeaderLines--}
```
public Line getLeaderLines()
```


Rappresenta le linee guida in un grafico. Le linee guida collegano le etichette dei dati ai punti dati. Questo oggetto non è una collezione; non esiste un oggetto che rappresenti una singola linea guida.

**Returns:**
[Line](../../com.aspose.cells/line)
### getLegendEntry() {#getLegendEntry--}
```
public LegendEntry getLegendEntry()
```


Ottiene la voce della legenda in base a questa serie.

**Returns:**
[LegendEntry](../../com.aspose.cells/legendentry)
### getMarker() {#getMarker--}
```
public Marker getMarker()
```


Ottiene il [getMarker()](../../com.aspose.cells/series\#getMarker--).

**Returns:**
[Marker](../../com.aspose.cells/marker)
### getName() {#getName--}
```
public String getName()
```


Ottiene il nome della serie di dati.

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


Specifica come sono posizionati barre e colonne. Può essere un valore compreso tra -100 e 100. Si applica solo ai grafici a barre 2-D e a colonne 2-D.

**Returns:**
short
### getPlotOnSecondAxis() {#getPlotOnSecondAxis--}
```
public boolean getPlotOnSecondAxis()
```


Indica se questa serie è tracciata sul secondo asse dei valori.

**Returns:**
boolean
### getPointValues() {#getPointValues--}
```
public ChartDataValue[] getPointValues()
```


Ottiene i valori effettivi utilizzati per tracciare ogni punto di questa serie nel grafico.

**Remarks**

Questa proprietà offre un modo comodo per ottenere i valori effettivi corrispondenti ai dati definiti da [getValues()](../../com.aspose.cells/series\#getValues--), soprattutto quando la fonte dati specificata è un collegamento esterno, una formula, ...ecc.

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


Ottiene la raccolta di punti in una serie in un grafico.

**Remarks**

Quando il grafico è Pie of Pie o Bar of Pie, l'ultimo punto è il punto "altro" nella prima sezione della torta.

**Returns:**
[ChartPointCollection](../../com.aspose.cells/chartpointcollection)
### getSecondPlotSize() {#getSecondPlotSize--}
```
public short getSecondPlotSize()
```


Restituisce o imposta la dimensione della sezione secondaria di un grafico Pie of Pie o Bar of Pie, come percentuale della dimensione della torta primaria. Può essere un valore da 5 a 200.

**Returns:**
short
### getSeriesLines() {#getSeriesLines--}
```
public Line getSeriesLines()
```


Restituisce un oggetto SeriesLines che rappresenta le linee di serie per un grafico a barre impilate o a colonne impilate. Si applica solo ai grafici a barre impilate e a colonne impilate.

**Returns:**
[Line](../../com.aspose.cells/line)
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Vero se la serie ha un'ombra.

**Returns:**
boolean
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Ottiene l'oggetto [ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection) che contiene le proprietà visive della forma della Serie.

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShowNegativeBubbles() {#getShowNegativeBubbles--}
```
public boolean getShowNegativeBubbles()
```


Vero se le bolle negative sono visualizzate per il gruppo di grafico. Valido solo per i grafici a bolle.

**Returns:**
boolean
### getSizeRepresents() {#getSizeRepresents--}
```
public int getSizeRepresents()
```


Ottiene cosa rappresenta la dimensione della bolla in un grafico a bolle.

Vedi [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

BubbleSizeRepresents.SizeIsArea indica che il valore [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) è l'area della bolla. BubbleSizeRepresents.SizeIsWidth indica che il valore [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) è la larghezza della bolla.

**Returns:**
int
### getSmooth() {#getSmooth--}
```
public boolean getSmooth()
```


Rappresenta l'ammorbidimento della curva. Vero se l'ammorbidimento della curva è attivato per il grafico a linee o a dispersione. Si applica solo ai grafici a linee e ai grafici a dispersione con linee.

**Returns:**
boolean
### getSplitType() {#getSplitType--}
```
public int getSplitType()
```


Restituisce o imposta un valore che determina quali punti dati sono nella seconda torta o barra in un grafico a torta di torta o a barra di torta.

Vedi [ChartSplitType](../../com.aspose.cells/chartsplittype).

**Returns:**
int
### getSplitValue() {#getSplitValue--}
```
public double getSplitValue()
```


Restituisce o imposta un valore da utilizzare per determinare quali punti dati sono nella seconda torta o barra in un grafico a torta di torta o a barra di torta.

**Returns:**
double
### getTrendLines() {#getTrendLines--}
```
public TrendlineCollection getTrendLines()
```


Restituisce tutte le linee di tendenza di questa serie.

**Returns:**
[TrendlineCollection](../../com.aspose.cells/trendlinecollection)
### getType() {#getType--}
```
public int getType()
```


Ottiene il tipo di una serie di dati.

Vedi [ChartType](../../com.aspose.cells/charttype).

**Returns:**
int
### getUpBars() {#getUpBars--}
```
public DropBars getUpBars()
```


Restituisce un oggetto DropBars che rappresenta le barre ascendenti in un grafico a linee. Si applica solo ai grafici a linee.

**Returns:**
[DropBars](../../com.aspose.cells/dropbars)
### getValues() {#getValues--}
```
public String getValues()
```


Rappresenta i valori Y di questa serie di grafico.

**Remarks**

Per ottenere i valori effettivi (corrispondenti a ogni punto di questa serie) definiti da questa proprietà, utilizzare [getPointValues()](../../com.aspose.cells/series\#getPointValues--).

**Returns:**
java.lang.String
### getValuesFormatCode() {#getValuesFormatCode--}
```
public String getValuesFormatCode()
```


Rappresenta il codice di formato della NumberList dei Valori.

**Returns:**
java.lang.String
### getXErrorBar() {#getXErrorBar--}
```
public ErrorBar getXErrorBar()
```


Rappresenta la barra di errore in direzione X della serie.

**Returns:**
[ErrorBar](../../com.aspose.cells/errorbar)
### getXValues() {#getXValues--}
```
public String getXValues()
```


Rappresenta i valori X di questa serie di grafico.

**Remarks**

Solo per i grafici Scatter e Bubble. Utilizzare [SeriesCollection.getCategoryData()](../../com.aspose.cells/seriescollection\#getCategoryData--) per altri tipi di grafici; [getCategoryValues()](../../com.aspose.cells/series\#getCategoryValues--) è usato per ottenere i valori di categoria effettivi di questa serie.

**Returns:**
java.lang.String
### getXValuesFormatCode() {#getXValuesFormatCode--}
```
public String getXValuesFormatCode()
```


Rappresenta il codice di formato della NumberList dei Valori X.

**Returns:**
java.lang.String
### getYErrorBar() {#getYErrorBar--}
```
public ErrorBar getYErrorBar()
```


Rappresenta la barra di errore in direzione Y della serie.

**Returns:**
[ErrorBar](../../com.aspose.cells/errorbar)
### hasDropLines() {#hasDropLines--}
```
public boolean hasDropLines()
```


Vero se il grafico ha linee di discesa. Si applica solo ai grafici a linee o a area.

**Returns:**
boolean
### hasHiLoLines() {#hasHiLoLines--}
```
public boolean hasHiLoLines()
```


Vero se il grafico a linee ha linee alto-basso. Si applica solo ai grafici a linee.

**Returns:**
boolean
### hasLeaderLines() {#hasLeaderLines--}
```
public boolean hasLeaderLines()
```


Vero se la serie ha linee guida.

**Returns:**
boolean
### hasRadarAxisLabels() {#hasRadarAxisLabels--}
```
public boolean hasRadarAxisLabels()
```


Vero se un grafico radar ha etichette dell'asse delle categorie. Si applica solo ai grafici radar.

**Returns:**
boolean
### hasSeriesLines() {#hasSeriesLines--}
```
public boolean hasSeriesLines()
```


Vero se un grafico a colonne impilate o a barre ha linee di serie o se un grafico Pie of Pie o Bar of Pie ha linee di collegamento tra le due sezioni. Si applica solo a grafici a colonne impilate, a barre, Pie of Pie o Bar of Pie.

**Returns:**
boolean
### hasUpDownBars() {#hasUpDownBars--}
```
public boolean hasUpDownBars()
```


Vero se un grafico a linee ha barre ascendenti e discendenti. Si applica solo ai grafici a linee.

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


Indica se il valore soglia è automatico.

**Returns:**
boolean
### isColorVaried() {#isColorVaried--}
```
public boolean isColorVaried()
```


Rappresenta se il colore dei punti è variabile. Il grafico deve contenere una sola serie o essere un grafico a torta.

**Returns:**
boolean
### isFiltered() {#isFiltered--}
```
public boolean isFiltered()
```


Indica se la serie è selezionata o filtrata. Vero indica che questa serie è filtrata e non verrà visualizzata nel grafico.

**Returns:**
boolean
### isVerticalValues() {#isVerticalValues--}
```
public boolean isVerticalValues()
```


Indica se l'origine dati è verticale.

**Returns:**
boolean
### move(int count) {#move-int-}
```
public void move(int count)
```


Sposta la serie verso l'alto o verso il basso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| count | int | Il numero di spostamenti verso l'alto o verso il basso. Sposta la serie verso l'alto se questo valore è inferiore a zero; sposta la serie verso il basso se è superiore a zero. |

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


Imposta il tipo di forma 3D utilizzato con il grafico a barre o colonne 3D.

Vedi [Bar3DShapeType](../../com.aspose.cells/bar3dshapetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBubbleScale(int value) {#setBubbleScale-int-}
```
public void setBubbleScale(int value)
```


Imposta il fattore di scala per le bolle nel gruppo di grafico specificato. Può essere un valore intero da 0 (zero) a 300, corrispondente a una percentuale della dimensione predefinita. Si applica solo ai grafici a bolle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBubbleSizeRepresents(int value) {#setBubbleSizeRepresents-int-}
```
public void setBubbleSizeRepresents(int value)
```


Ottiene cosa rappresenta la dimensione della bolla in un grafico a bolle.

Vedi [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Aspose.Cells.Charts.Series.SizeRepresents. Questa proprietà sarà rimossa 12 mesi dopo, a partire da GENNAIO 2012. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBubbleSizes(String value) {#setBubbleSizes-java.lang.String-}
```
public void setBubbleSizes(String value)
```


Imposta i valori di dimensione delle bolle della serie di grafico.

**Remarks**

Solo per [ChartType.BUBBLE](../../com.aspose.cells/charttype#BUBBLE) o [ChartType.BUBBLE_3_D](../../com.aspose.cells/charttype#BUBBLE-3-D).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setColorVaried(boolean value) {#setColorVaried-boolean-}
```
public void setColorVaried(boolean value)
```


Rappresenta se il colore dei punti è variabile. Il grafico deve contenere una sola serie o essere un grafico a torta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDoughnutHoleSize(int value) {#setDoughnutHoleSize-int-}
```
public void setDoughnutHoleSize(int value)
```


Restituisce o imposta la dimensione del foro in un gruppo di grafico a ciambella. La dimensione del foro è espressa come percentuale della dimensione del grafico, tra il 10% e il 90%.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setExplosion(int value) {#setExplosion-int-}
```
public void setExplosion(int value)
```


La distanza di una fetta di torta aperta dal centro del grafico a torta è espressa come percentuale del diametro della torta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setFiltered(boolean value) {#setFiltered-boolean-}
```
public void setFiltered(boolean value)
```


Indica se la serie è selezionata o filtrata. Vero indica che questa serie è filtrata e non verrà visualizzata nel grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFirstSliceAngle(short value) {#setFirstSliceAngle-short-}
```
public void setFirstSliceAngle(short value)
```


Imposta l'angolo della prima fetta di grafico a torta o di grafico a ciambella, in gradi (in senso orario dalla verticale). Si applica solo a grafici a torta, a torta 3D e a ciambella, con valori da 0 a 360.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | short |  |

### setGapWidth(short value) {#setGapWidth-short-}
```
public void setGapWidth(short value)
```


Restituisce o imposta lo spazio tra i raggruppamenti di barre o colonne, come percentuale della larghezza della barra o della colonna. Il valore di questa proprietà deve essere compreso tra 0 e 500.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | short |  |

### setHas3DEffect(boolean value) {#setHas3DEffect-boolean-}
```
public void setHas3DEffect(boolean value)
```


Vero se la serie ha un aspetto tridimensionale.

**Remarks**

Si applica solo ai grafici [ChartType.BUBBLE](../../com.aspose.cells/charttype\#BUBBLE) o [ChartType.BUBBLE\_3\_D](../../com.aspose.cells/charttype\#BUBBLE-3-D).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHasDropLines(boolean value) {#setHasDropLines-boolean-}
```
public void setHasDropLines(boolean value)
```


Vero se il grafico ha linee di discesa. Si applica solo ai grafici a linee o a area.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHasHiLoLines(boolean value) {#setHasHiLoLines-boolean-}
```
public void setHasHiLoLines(boolean value)
```


Vero se il grafico a linee ha linee alto-basso. Si applica solo ai grafici a linee.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHasLeaderLines(boolean value) {#setHasLeaderLines-boolean-}
```
public void setHasLeaderLines(boolean value)
```


Vero se la serie ha linee guida.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHasRadarAxisLabels(boolean value) {#setHasRadarAxisLabels-boolean-}
```
public void setHasRadarAxisLabels(boolean value)
```


Vero se un grafico radar ha etichette dell'asse delle categorie. Si applica solo ai grafici radar.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHasSeriesLines(boolean value) {#setHasSeriesLines-boolean-}
```
public void setHasSeriesLines(boolean value)
```


Vero se un grafico a colonne impilate o a barre ha linee di serie o se un grafico Pie of Pie o Bar of Pie ha linee di collegamento tra le due sezioni. Si applica solo a grafici a colonne impilate, a barre, Pie of Pie o Bar of Pie.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHasUpDownBars(boolean value) {#setHasUpDownBars-boolean-}
```
public void setHasUpDownBars(boolean value)
```


Vero se un grafico a linee ha barre ascendenti e discendenti. Si applica solo ai grafici a linee.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Imposta il nome della serie di dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOverlap(short value) {#setOverlap-short-}
```
public void setOverlap(short value)
```


Specifica come sono posizionati barre e colonne. Può essere un valore compreso tra -100 e 100. Si applica solo ai grafici a barre 2-D e a colonne 2-D.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | short |  |

### setPlotOnSecondAxis(boolean value) {#setPlotOnSecondAxis-boolean-}
```
public void setPlotOnSecondAxis(boolean value)
```


Indica se questa serie è tracciata sul secondo asse dei valori.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSecondPlotSize(short value) {#setSecondPlotSize-short-}
```
public void setSecondPlotSize(short value)
```


Restituisce o imposta la dimensione della sezione secondaria di un grafico Pie of Pie o Bar of Pie, come percentuale della dimensione della torta primaria. Può essere un valore da 5 a 200.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | short |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Vero se la serie ha un'ombra.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowNegativeBubbles(boolean value) {#setShowNegativeBubbles-boolean-}
```
public void setShowNegativeBubbles(boolean value)
```


Vero se le bolle negative sono visualizzate per il gruppo di grafico. Valido solo per i grafici a bolle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSizeRepresents(int value) {#setSizeRepresents-int-}
```
public void setSizeRepresents(int value)
```


Imposta cosa rappresenta la dimensione della bolla in un grafico a bolle.

Vedi [BubbleSizeRepresents](../../com.aspose.cells/bubblesizerepresents).

**Remarks**

BubbleSizeRepresents.SizeIsArea indica che il valore [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) è l'area della bolla. BubbleSizeRepresents.SizeIsWidth indica che il valore [getBubbleSizes()](../../com.aspose.cells/series\#getBubbleSizes--) è la larghezza della bolla.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSmooth(boolean value) {#setSmooth-boolean-}
```
public void setSmooth(boolean value)
```


Rappresenta l'ammorbidimento della curva. Vero se l'ammorbidimento della curva è attivato per il grafico a linee o a dispersione. Si applica solo ai grafici a linee e ai grafici a dispersione con linee.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSplitType(int value) {#setSplitType-int-}
```
public void setSplitType(int value)
```


Restituisce o imposta un valore che determina quali punti dati sono nella seconda torta o barra in un grafico a torta di torta o a barra di torta.

Vedi [ChartSplitType](../../com.aspose.cells/chartsplittype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSplitValue(double value) {#setSplitValue-double-}
```
public void setSplitValue(double value)
```


Restituisce o imposta un valore da utilizzare per determinare quali punti dati sono nella seconda torta o barra in un grafico a torta di torta o a barra di torta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Imposta il tipo di una serie di dati.

Vedi [ChartType](../../com.aspose.cells/charttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setValues(String value) {#setValues-java.lang.String-}
```
public void setValues(String value)
```


Rappresenta i valori Y di questa serie di grafico.

**Remarks**

Per ottenere i valori effettivi (corrispondenti a ogni punto di questa serie) definiti da questa proprietà, utilizzare [getPointValues()](../../com.aspose.cells/series\#getPointValues--).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setValuesFormatCode(String value) {#setValuesFormatCode-java.lang.String-}
```
public void setValuesFormatCode(String value)
```


Rappresenta il codice di formato della NumberList dei Valori.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setXValues(String value) {#setXValues-java.lang.String-}
```
public void setXValues(String value)
```


Rappresenta i valori X di questa serie di grafico.

**Remarks**

Solo per i grafici Scatter e Bubble. Utilizzare [SeriesCollection.getCategoryData()](../../com.aspose.cells/seriescollection\#getCategoryData--) per altri tipi di grafici; [getCategoryValues()](../../com.aspose.cells/series\#getCategoryValues--) è usato per ottenere i valori di categoria effettivi di questa serie.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setXValuesFormatCode(String value) {#setXValuesFormatCode-java.lang.String-}
```
public void setXValuesFormatCode(String value)
```


Rappresenta il codice di formato della NumberList dei Valori X.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

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

