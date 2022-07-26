---
title: Series
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Incapsula loggetto che rappresenta una singola serie di dati in un grafico.
type: docs
weight: 820
url: /it/net/aspose.cells.charts/series/
---
## Series class

Incapsula l'oggetto che rappresenta una singola serie di dati in un grafico.

```csharp
public class Series
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Area](../../aspose.cells.charts/series/area) { get; } | Rappresenta l'area di sfondo dell'oggetto Serie. |
| [Bar3DShapeType](../../aspose.cells.charts/series/bar3dshapetype) { get; set; } | Ottiene o imposta il tipo di forma 3D utilizzato con la barra 3D o l'istogramma. |
| [Border](../../aspose.cells.charts/series/border) { get; } | Rappresenta il bordo dell'oggetto Serie. |
| [BubbleScale](../../aspose.cells.charts/series/bubblescale) { get; set; } | Ottiene o imposta il fattore di scala per le bolle nel gruppo di grafici specificato. Può essere un valore intero compreso tra 0 (zero) e 300, corrispondente a una percentuale della dimensione predefinita. Si applica solo ai grafici a bolle. |
| [BubbleSizes](../../aspose.cells.charts/series/bubblesizes) { get; set; } | Ottiene o imposta i valori delle dimensioni delle bolle della serie di grafici. |
| [CountOfDataValues](../../aspose.cells.charts/series/countofdatavalues) { get; } | Ottiene il numero dei valori dei dati. |
| [DataLabels](../../aspose.cells.charts/series/datalabels) { get; } | Rappresenta l'oggetto DataLabels per l'ASeries specificato. |
| [DisplayName](../../aspose.cells.charts/series/displayname) { get; } | Ottiene il nome della serie visualizzato nel grafico del grafico. |
| [DoughnutHoleSize](../../aspose.cells.charts/series/doughnutholesize) { get; set; } | Restituisce o imposta la dimensione del foro in un gruppo di grafici ad anello. La dimensione del foro è espressa come percentuale della dimensione del grafico, tra il 10 e il 90 percento. |
| [DownBars](../../aspose.cells.charts/series/downbars) { get; } | Restituisce a[`DropBars`](../dropbars) oggetto che rappresenta le barre in basso su un grafico a linee. Si applica solo ai grafici a linee. |
| [DropLines](../../aspose.cells.charts/series/droplines) { get; } | Restituisce a[`Line`](../../aspose.cells.drawing/line) oggetto che rappresenta le linee di discesa per una serie nel grafico a linee o ad area. Si applica solo al grafico a linee o ai grafici ad area. |
| [Explosion](../../aspose.cells.charts/series/explosion) { get; set; } | La distanza di una fetta a torta aperta dal centro del grafico a torta è espressa come percentuale del diametro della torta. |
| [FirstSliceAngle](../../aspose.cells.charts/series/firstsliceangle) { get; set; } | Ottiene o imposta l'angolo della prima fetta del grafico a torta oa ciambella, in gradi (in senso orario dalla verticale). Si applica solo a grafici a torta, a torta 3D e ad anello, da 0 a 360. |
| [GapWidth](../../aspose.cells.charts/series/gapwidth) { get; set; } | Restituisce o imposta lo spazio tra i cluster di barre o colonne, come percentuale della larghezza della barra o della colonna. Il valore di questa proprietà deve essere compreso tra 0 e 500. |
| [Has3DEffect](../../aspose.cells.charts/series/has3deffect) { get; set; } | Vero se la serie ha un aspetto tridimensionale. Si applica solo ai grafici a bolle. |
| [HasDropLines](../../aspose.cells.charts/series/hasdroplines) { get; set; } | Vero se il grafico ha linee di discesa. Si applica solo al grafico a linee o ai grafici ad area. |
| [HasHiLoLines](../../aspose.cells.charts/series/hashilolines) { get; set; } | Vero se il grafico a linee ha linee alto-basso. Si applica solo ai grafici a linee. |
| [HasLeaderLines](../../aspose.cells.charts/series/hasleaderlines) { get; set; } | Vero se la serie ha linee guida. |
| [HasRadarAxisLabels](../../aspose.cells.charts/series/hasradaraxislabels) { get; set; } | Vero se un grafico radar ha etichette degli assi di categoria. Si applica solo alle carte radar. |
| [HasSeriesLines](../../aspose.cells.charts/series/hasserieslines) { get; set; } | Vero se un istogramma o un grafico a barre in pila ha linee di serie o se un grafico a torta o un grafico a barre a torta ha linee di collegamento tra le due sezioni. Si applica solo a istogrammi in pila, grafici a barre, grafici a torta o grafici a barre di torta. |
| [HasUpDownBars](../../aspose.cells.charts/series/hasupdownbars) { get; set; } | Vero se un grafico a linee ha barre su e giù. Si applica solo ai grafici a linee. |
| [HiLoLines](../../aspose.cells.charts/series/hilolines) { get; } | Restituisce un oggetto HiLoLines che rappresenta le linee alto-basso per una serie su un grafico a linee. Si applica solo ai grafici a linee. |
| [IsAutoSplit](../../aspose.cells.charts/series/isautosplit) { get; } | Indica se il valore di soglia è automatico. |
| [IsColorVaried](../../aspose.cells.charts/series/iscolorvaried) { get; set; } | Rappresenta se il colore dei punti è variato. Il grafico deve contenere solo una serie. |
| [IsVerticalValues](../../aspose.cells.charts/series/isverticalvalues) { get; } | Indica se l'origine dati è verticale. |
| [LayoutProperties](../../aspose.cells.charts/series/layoutproperties) { get; } | Rappresenta le proprietà del layout. |
| [LeaderLines](../../aspose.cells.charts/series/leaderlines) { get; } | Rappresenta le linee guida su un grafico. Le linee guida collegano le etichette dati ai punti dati. Questo oggetto non è una raccolta; non c'è nessun oggetto che rappresenti una singola linea guida. |
| [LegendEntry](../../aspose.cells.charts/series/legendentry) { get; } | Ottiene la voce della legenda in base a questa serie. |
| [Marker](../../aspose.cells.charts/series/marker) { get; } | Ottiene il[`marcatore`](./marker) . |
| [Name](../../aspose.cells.charts/series/name) { get; set; } | Ottiene o imposta il nome della serie di dati. |
| [Overlap](../../aspose.cells.charts/series/overlap) { get; set; } | Specifica come sono posizionate le barre e le colonne. Può essere un valore compreso tra – 100 e 100. Si applica solo a istogrammi 2D e istogrammi 2D. |
| [PlotOnSecondAxis](../../aspose.cells.charts/series/plotonsecondaxis) { get; set; } | Indica se questa serie è tracciata sul secondo asse dei valori. |
| [Points](../../aspose.cells.charts/series/points) { get; } | Ottiene la raccolta di punti in una serie in un grafico. |
| [SecondPlotSize](../../aspose.cells.charts/series/secondplotsize) { get; set; } | Restituisce o imposta la dimensione della sezione secondaria di un grafico a torta o di una barra di grafico a torta, come percentuale della dimensione della torta primaria. Può essere un valore compreso tra 5 e 200. |
| [SeriesLines](../../aspose.cells.charts/series/serieslines) { get; } | Restituisce un oggetto SeriesLines che rappresenta le linee della serie per un grafico a barre in pila o un istogramma a colonne in pila. Si applica solo a istogrammi a barre in pila e istogrammi in pila. |
| [Shadow](../../aspose.cells.charts/series/shadow) { get; set; } | Vero se la serie ha un'ombra. |
| [ShapeProperties](../../aspose.cells.charts/series/shapeproperties) { get; } | Ottiene il oggetto che contiene le proprietà della forma visiva della serie. |
| [ShowNegativeBubbles](../../aspose.cells.charts/series/shownegativebubbles) { get; set; } | Vero se vengono visualizzate bolle negative per il gruppo di grafici. Valido solo per grafici a bolle. |
| [SizeRepresents](../../aspose.cells.charts/series/sizerepresents) { get; set; } | Ottiene o imposta ciò che la dimensione della bolla rappresenta su un grafico a bolle. |
| [Smooth](../../aspose.cells.charts/series/smooth) { get; set; } | Rappresenta l'arrotondamento della curva. Vero se l'arrotondamento della curva è attivato per il grafico a linee o a dispersione. Si applica solo a linee e a dispersione collegati da grafici a linee. |
| [SplitType](../../aspose.cells.charts/series/splittype) { get; set; } | Restituisce o imposta un valore che indica come determinare quali punti dati si trovano nella seconda torta o barra su una torta di torta o barra di grafico a torta. |
| [SplitValue](../../aspose.cells.charts/series/splitvalue) { get; set; } | Restituisce o imposta un valore che deve essere utilizzato per determinare quali punti dati si trovano nella seconda torta o barra su una torta di torta o barra di grafico a torta. |
| [TrendLines](../../aspose.cells.charts/series/trendlines) { get; } | Restituisce un oggetto che rappresenta una raccolta di tutte le linee di tendenza per la serie. |
| [Type](../../aspose.cells.charts/series/type) { get; set; } | Ottiene o imposta il tipo di una serie di dati. |
| [UpBars](../../aspose.cells.charts/series/upbars) { get; } | Restituisce un oggetto DropBars che rappresenta le barre in alto su un grafico a linee. Si applica solo ai grafici a linee. |
| [Values](../../aspose.cells.charts/series/values) { get; set; } | Rappresenta i dati della serie di grafici. |
| [ValuesFormatCode](../../aspose.cells.charts/series/valuesformatcode) { get; set; } | Rappresenta il codice formato dell'elenco numeri di valori. |
| [XErrorBar](../../aspose.cells.charts/series/xerrorbar) { get; } | Rappresenta la barra di errore di direzione X della serie. |
| [XValues](../../aspose.cells.charts/series/xvalues) { get; set; } | Rappresenta i valori x della serie di grafici. |
| [YErrorBar](../../aspose.cells.charts/series/yerrorbar) { get; } | Rappresenta la barra di errore della direzione Y della serie. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Move](../../aspose.cells.charts/series/move)(int) | Sposta la serie in alto o in basso. |

### Esempi

```csharp

[C#]

//Creazione di un'istanza di un oggetto cartella di lavoro
Workbook workbook = new Workbook();
//Aggiunta di un nuovo foglio di lavoro all'oggetto Excel
int sheetIndex = workbook.Worksheets.Add();
//Ottenere il riferimento del foglio di lavoro appena aggiunto passando il relativo indice del foglio
Worksheet worksheet = workbook.Worksheets[sheetIndex];
//Aggiunta di un valore di esempio alla cella "A1".
worksheet.Cells["A1"].PutValue(50);
//Aggiunta di un valore di esempio alla cella "A2".
worksheet.Cells["A2"].PutValue(100);
//Aggiunta di un valore di esempio alla cella "A3".
worksheet.Cells["A3"].PutValue(150);
//Aggiunta di un valore di esempio alla cella "A4".
worksheet.Cells["A4"].PutValue(200);
//Aggiunta di un valore di esempio alla cella "B1".
worksheet.Cells["B1"].PutValue(60);
//Aggiunta di un valore di esempio alla cella "B2".
worksheet.Cells["B2"].PutValue(32);
//Aggiunta di un valore di esempio alla cella "B3".
worksheet.Cells["B3"].PutValue(50);
//Aggiunta di un valore di esempio alla cella "B4".
worksheet.Cells["B4"].PutValue(40);
//Aggiunta di un valore di esempio alla cella "C1" come dati di categoria
worksheet.Cells["C1"].PutValue("Q1");
//Aggiunta di un valore di esempio alla cella "C2" come dati di categoria
worksheet.Cells["C2"].PutValue("Q2");
//Aggiunta di un valore di esempio alla cella "C3" come dati di categoria
worksheet.Cells["C3"].PutValue("Y1");
//Aggiunta di un valore di esempio alla cella "C4" come dati di categoria
worksheet.Cells["C4"].PutValue("Y2");
//Aggiunta di un grafico al foglio di lavoro
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
//Accesso all'istanza del grafico appena aggiunto
Chart chart = worksheet.Charts[chartIndex];
//Aggiunta di NSeries (origine dati grafico) al grafico che va dalla cella "A1" a "B4"
int seriesIndex = chart.NSeries.Add("A1:B4", true);
//Impostazione dell'origine dati per i dati di categoria di NSeries
chart.NSeries.CategoryData = "C1:C4";
Series series = chart.NSeries[seriesIndex];
//Impostazione dei valori della serie.
series.Values = "=B1:B4";
//Cambiare il tipo di grafico della serie.
series.Type = ChartType.Line;
//Impostazione delle proprietà dell'indicatore.
series.Marker.MarkerStyle = ChartMarkerType.Circle;
series.Marker.ForegroundColorSetType = FormattingType.Automatic;
series.Marker.ForegroundColor = System.Drawing.Color.Black;
series.Marker.BackgroundColorSetType = FormattingType.Automatic;

//fai i tuoi affari

//Salvataggio del file Excel
workbook.Save("book1.xls");

[Visual Basic]

'Creazione di un'istanza di un oggetto Workbook
Dim workbook As Workbook = New Workbook()
'Aggiunta di un nuovo foglio di lavoro all'oggetto Excel
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice del foglio
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)
'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)
'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)
'Adding a sample value to "A4" cell
worksheet.Cells("A4").PutValue(200)
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'Adding a sample value to "B4" cell
worksheet.Cells("B4").PutValue(40)
'Adding a sample value to "C1" cell as category data
worksheet.Cells("C1").PutValue("Q1")
'Adding a sample value to "C2" cell as category data
worksheet.Cells("C2").PutValue("Q2")
'Adding a sample value to "C3" cell as category data
worksheet.Cells("C3").PutValue("Y1")
'Adding a sample value to "C4" cell as category data
worksheet.Cells("C4").PutValue("Y2")
'Aggiunta di un grafico al foglio di lavoro
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Accesso all'istanza del grafico appena aggiunto
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
Dim seriesIndex As Int32 = chart.NSeries.Add("A1:B4", True)
'Impostazione dell'origine dati per i dati di categoria di NSeries
chart.NSeries.CategoryData = "C1:C4"
Dim series As Series = chart.NSeries(seriesIndex)
'Impostazione dei valori della serie.
series.Values = "=B1:B4"
'Modifica del tipo di grafico della serie.
series.Type = ChartType.Line
'Impostazione delle proprietà dei marker.
series.Marker.MarkerStyle = ChartMarkerType.Circle
series.Marker.ForegroundColorSetType = FormattingType.Automatic
series.Marker.ForegroundColor = System.Drawing.Color.Black
series.Marker.BackgroundColorSetType = FormattingType.Automatic
'Salvataggio del file Excel
workbook.Save("book1.xls")
```

### Guarda anche

* spazio dei nomi [Aspose.Cells.Charts](../../aspose.cells.charts)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
