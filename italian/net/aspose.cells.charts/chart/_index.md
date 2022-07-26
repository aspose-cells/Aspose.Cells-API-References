---
title: Chart
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Incapsula loggetto che rappresenta un singolo grafico Excel.
type: docs
weight: 430
url: /it/net/aspose.cells.charts/chart/
---
## Chart class

Incapsula l'oggetto che rappresenta un singolo grafico Excel.

```csharp
public class Chart
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutoScaling](../../aspose.cells.charts/chart/autoscaling) { get; set; } | True se Microsoft Excel ridimensiona un grafico 3D in modo che sia di dimensioni più vicine al grafico 2D equivalente. La proprietà RightAngleAxes deve essere True. |
| [BackWall](../../aspose.cells.charts/chart/backwall) { get; } | Restituisce a[`Walls`](./walls) oggetto che rappresenta la parete di fondo di un grafico 3D. |
| [CategoryAxis](../../aspose.cells.charts/chart/categoryaxis) { get; } | Ottiene l'asse X del grafico. |
| [ChartArea](../../aspose.cells.charts/chart/chartarea) { get; } | Ottiene l'area del grafico nel foglio di lavoro. |
| [ChartDataTable](../../aspose.cells.charts/chart/chartdatatable) { get; } | Rappresenta la tabella dei dati del grafico. |
| [ChartObject](../../aspose.cells.charts/chart/chartobject) { get; } | Rappresenta la forma del grafico; |
| [DepthPercent](../../aspose.cells.charts/chart/depthpercent) { get; set; } | Rappresenta la profondità di un grafico 3D come percentuale della larghezza del grafico (tra il 20 e il 2000 percento). |
| [DisplayNaAsBlank](../../aspose.cells.charts/chart/displaynaasblank) { get; set; } | Indica se visualizzare #N/D come valore vuoto. |
| [Elevation](../../aspose.cells.charts/chart/elevation) { get; set; } | Rappresenta l'elevazione della vista mappa 3D, in gradi. |
| [FirstSliceAngle](../../aspose.cells.charts/chart/firstsliceangle) { get; set; } | Ottiene o imposta l'angolo della prima fetta del grafico a torta oa ciambella, in gradi (in senso orario dalla verticale). Si applica solo a grafici a torta, a torta 3D e ad anello, da 0 a 360. |
| [Floor](../../aspose.cells.charts/chart/floor) { get; } | Restituisce a[`Floor`](./floor) oggetto che rappresenta le pareti di un grafico 3D. |
| [GapDepth](../../aspose.cells.charts/chart/gapdepth) { get; set; } | Ottiene o imposta la distanza tra le serie di dati in un grafico 3D, come percentuale della larghezza dell'indicatore. Il valore di questa proprietà deve essere compreso tra 0 e 500. |
| [GapWidth](../../aspose.cells.charts/chart/gapwidth) { get; set; } | Restituisce o imposta lo spazio tra i cluster di barre o colonne, come percentuale della larghezza della barra o della colonna. Il valore di questa proprietà deve essere compreso tra 0 e 500. |
| [HeightPercent](../../aspose.cells.charts/chart/heightpercent) { get; set; } | Restituisce o imposta l'altezza di un grafico 3D come percentuale della larghezza del grafico (tra il 5 e il 500 percento). |
| [HidePivotFieldButtons](../../aspose.cells.charts/chart/hidepivotfieldbuttons) { get; set; } | Indica se nascondere i pulsanti del campo del grafico pivot solo quando il grafico è Grafico pivot. |
| [Is3D](../../aspose.cells.charts/chart/is3d) { get; } | Indica se il grafico è un grafico 3d. |
| [IsRectangularCornered](../../aspose.cells.charts/chart/isrectangularcornered) { get; set; } | Ottiene o imposta un valore che indica se l'area del grafico è rettangolare. L'impostazione predefinita è true. |
| [Legend](../../aspose.cells.charts/chart/legend) { get; } | Ottiene la legenda del grafico. |
| [Line](../../aspose.cells.charts/chart/line) { get; } | Ottiene la linea. |
| [Name](../../aspose.cells.charts/chart/name) { get; set; } | Ottiene e imposta il nome del grafico. |
| [NSeries](../../aspose.cells.charts/chart/nseries) { get; } | Ottiene a[`SeriesCollection`](../seriescollection) raccolta che rappresenta la serie di dati nel grafico. |
| [PageSetup](../../aspose.cells.charts/chart/pagesetup) { get; } | Rappresenta la descrizione dell'impostazione della pagina in questo grafico. |
| [Perspective](../../aspose.cells.charts/chart/perspective) { get; set; } | Restituisce o imposta la prospettiva per la visualizzazione del grafico 3D. Deve essere compreso tra 0 e 100. Questa proprietà viene ignorata se la proprietà RightAngleAxes è True. |
| [PivotOptions](../../aspose.cells.charts/chart/pivotoptions) { get; } | Specifica i controlli pivot visualizzati nel grafico |
| [PivotSource](../../aspose.cells.charts/chart/pivotsource) { get; set; } | L'origine sono i dati della tabella pivot. Se PivotSource non è vuota, il grafico è Grafico pivot. |
| [Placement](../../aspose.cells.charts/chart/placement) { get; set; } | Rappresenta il modo in cui il grafico è collegato alle celle sottostanti. |
| [PlotArea](../../aspose.cells.charts/chart/plotarea) { get; } | Ottiene l'area del grafico del grafico che include le etichette dei tick degli assi. |
| [PlotBy](../../aspose.cells.charts/chart/plotby) { get; } | Ottiene e imposta se tracciare per riga o colonna. |
| [PlotEmptyCellsType](../../aspose.cells.charts/chart/plotemptycellstype) { get; set; } | Ottiene e imposta come tracciare le celle vuote. |
| [PlotVisibleCells](../../aspose.cells.charts/chart/plotvisiblecells) { get; set; } | Indica se tracciare solo le celle visibili. |
| [PrintSize](../../aspose.cells.charts/chart/printsize) { get; set; } | Ottiene e imposta la dimensione del grafico stampato. |
| [RightAngleAxes](../../aspose.cells.charts/chart/rightangleaxes) { get; set; } | Vero se gli assi del grafico sono ad angolo retto. Si applica solo ai grafici 3D (tranne Column3D e grafici a torta 3D). |
| [RotationAngle](../../aspose.cells.charts/chart/rotationangle) { get; set; } | Rappresenta la rotazione della vista del grafico 3D (la rotazione dell'area del tracciato attorno all'asse z, in gradi). |
| [SecondCategoryAxis](../../aspose.cells.charts/chart/secondcategoryaxis) { get; } | Ottiene il secondo asse X del grafico. |
| [SecondValueAxis](../../aspose.cells.charts/chart/secondvalueaxis) { get; } | Ottiene il secondo asse Y del grafico. |
| [SeriesAxis](../../aspose.cells.charts/chart/seriesaxis) { get; } | Ottiene l'asse della serie del grafico. |
| [Shapes](../../aspose.cells.charts/chart/shapes) { get; } | Restituisce tutte le forme del disegno in questo grafico. |
| [ShowDataTable](../../aspose.cells.charts/chart/showdatatable) { get; set; } | Ottiene o imposta un valore che indica se il grafico visualizza una tabella di dati. |
| [ShowLegend](../../aspose.cells.charts/chart/showlegend) { get; set; } | Ottiene o imposta un valore che indica se verrà visualizzata la legenda del grafico. L'impostazione predefinita è true. |
| [SideWall](../../aspose.cells.charts/chart/sidewall) { get; } | Restituisce a[`Walls`](./walls)oggetto che rappresenta la parete laterale di un grafico 3D. |
| [SizeWithWindow](../../aspose.cells.charts/chart/sizewithwindow) { get; set; } | Vero se Microsoft Excel ridimensiona il grafico in modo che corrisponda alle dimensioni della finestra del foglio grafico. |
| [Style](../../aspose.cells.charts/chart/style) { get; set; } | Ottiene e imposta lo stile incorporato. |
| [SubTitle](../../aspose.cells.charts/chart/subtitle) { get; } | Ottiene il sottotitolo del grafico. Solo per file in formato ODS. |
| [Title](../../aspose.cells.charts/chart/title) { get; } | Ottiene il titolo del grafico. |
| [Type](../../aspose.cells.charts/chart/type) { get; set; } | Ottiene o imposta il tipo di un grafico. |
| [ValueAxis](../../aspose.cells.charts/chart/valueaxis) { get; } | Ottiene l'asse Y del grafico. |
| [Walls](../../aspose.cells.charts/chart/walls) { get; } | Restituisce a[`Walls`](./walls) oggetto che rappresenta le pareti di un grafico 3D. |
| [WallsAndGridlines2D](../../aspose.cells.charts/chart/wallsandgridlines2d) { get; set; } | Vero se le linee della griglia sono disegnate bidimensionalmente su un grafico 3D. |
| [Worksheet](../../aspose.cells.charts/chart/worksheet) { get; } | Ottiene il foglio di lavoro che contiene questo grafico. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Calculate](../../aspose.cells.charts/chart/calculate)() | Calcola la posizione personalizzata dell'area del tracciato, gli assi se la loro posizione è assegnata automaticamente. |
| [GetActualSize](../../aspose.cells.charts/chart/getactualsize)() | Ottiene la dimensione effettiva del grafico in unità di pixel. |
| [GetChartDataRange](../../aspose.cells.charts/chart/getchartdatarange)() | Ottiene l'intervallo dell'origine dati del grafico. |
| [HasAxis](../../aspose.cells.charts/chart/hasaxis)(AxisType, bool) | Restituisce quali assi esistono nel grafico. |
| [IsChartDataChanged](../../aspose.cells.charts/chart/ischartdatachanged)() | Rileva se l'origine dati di un grafico è cambiata. |
| [Move](../../aspose.cells.charts/chart/move)(int, int, int, int) | Sposta il grafico in una posizione specificata. |
| [RefreshPivotData](../../aspose.cells.charts/chart/refreshpivotdata)() | Aggiorna i dati del grafico pivot dall'origine dati pivot. |
| [SetChartDataRange](../../aspose.cells.charts/chart/setchartdatarange)(string, bool) | Specifica l'intervallo di dati per un grafico. |
| [SwitchRowColumn](../../aspose.cells.charts/chart/switchrowcolumn)() | Cambia riga/colonna. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage)() | Ottiene un 32 bit`Bitmap` oggetto del grafico. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_1)(ImageOrPrintOptions) | Ottiene un 32 bit`Bitmap` oggetto del grafico. `ImageOrPrintOptions.ImageFormat` , gli attributi ImageOrPrintOptions.TiffCompression e ImageOrPrintOptions.Quality vengono ignorati. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_6)(string) | Crea l'immagine del grafico e la salva in un file. L'estensione del nome del file determina il formato dell'immagine. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_3)(Stream, ImageOrPrintOptions) | Crea l'immagine del grafico e la salva in un flusso nel formato specificato. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_2)(Stream, ImageType) | Crea l'immagine del grafico e la salva in un flusso nel formato specificato. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_4)(Stream, long) | Crea l'immagine del grafico e la salva in uno stream nel formato Jpeg. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_8)(string, ImageOrPrintOptions) | Crea l'immagine del grafico e la salva in un file. L'estensione del nome del file determina il formato dell'immagine. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_7)(string, ImageType) | Crea l'immagine del grafico e la salva in un file del tipo di immagine specificato. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_9)(string, long) | Crea l'immagine del grafico e la salva in un file in formato Jpeg. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf)(Stream) | Crea il pdf del grafico e lo salva in uno stream. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_2)(string) | Salva il grafico in un file pdf. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_1)(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Crea il pdf del grafico e lo salva in uno stream. |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_3)(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Salva il grafico in un file pdf. |

### Esempi

```csharp
[C#]

Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];

Cells cells = sheet.Cells;
cells[0,1].PutValue("Income");
cells[1,0].PutValue("Company A");
cells[2,0].PutValue("Company B");
cells[3,0].PutValue("Company C");
cells[1,1].PutValue(10000);
cells[2,1].PutValue(20000);
cells[3,1].PutValue(30000);
		
int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);

Chart chart = sheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
chart.ShowLegend = true;
chart.Title.Text = "Income Analysis";

[Visual Basic]

Dim workbook as Workbook = new Workbook()
Dim sheet as Worksheet = workbook.Worksheets(0)

Dim cells as Cells = sheet.Cells
cells(0,1).PutValue("Income")
cells(1,0).PutValue("Company A")
cells(2,0).PutValue("Company B")
cells(3,0).PutValue("Company C")
cells(1,1).PutValue(10000)
cells(2,1).PutValue(20000)
cells(3,1).PutValue(30000)
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)

Dim chart as Chart = sheet.Charts(chartIndex) 
chart.SetChartDataRange("A1:B4", True);
chart.ShowLegend = True
chart.Title.Text = "Income Analysis"
```

### Guarda anche

* spazio dei nomi [Aspose.Cells.Charts](../../aspose.cells.charts)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
