---
title: "Classe Chart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.Chart class. Incapsula l'oggetto che rappresenta un singolo grafico Excel"
type: docs
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
| [ActualChartSize](../../aspose.cells.charts/chart/actualchartsize/) { get; } | (**Obsolete.**) Ottiene le dimensioni effettive del grafico in unità di pixel. |
| [AutoScaling](../../aspose.cells.charts/chart/autoscaling/) { get; set; } | Vero se Microsoft Excel scala un grafico 3-D in modo che sia più vicino in dimensione al grafico 2-D equivalente. La proprietà RightAngleAxes deve essere True. |
| [BackWall](../../aspose.cells.charts/chart/backwall/) { get; } | Restituisce un oggetto [`Walls`](./walls/) che rappresenta la parete posteriore di un grafico 3-D. |
| [CategoryAxis](../../aspose.cells.charts/chart/categoryaxis/) { get; } | Ottiene l'asse X del grafico. |
| [ChartArea](../../aspose.cells.charts/chart/chartarea/) { get; } | Ottiene l'area del grafico nel foglio di lavoro. |
| [ChartDataTable](../../aspose.cells.charts/chart/chartdatatable/) { get; } | Rappresenta la tabella dati del grafico. |
| [ChartObject](../../aspose.cells.charts/chart/chartobject/) { get; } | Rappresenta il chartShape; |
| [DepthPercent](../../aspose.cells.charts/chart/depthpercent/) { get; set; } | Rappresenta la profondità di un grafico 3-D come percentuale della larghezza del grafico (tra il 20 e il 2000 percento). |
| [DisplayNaAsBlank](../../aspose.cells.charts/chart/displaynaasblank/) { get; set; } | Indica se visualizzare #N/A come valore vuoto. |
| [Elevation](../../aspose.cells.charts/chart/elevation/) { get; set; } | Rappresenta l'elevazione della visualizzazione del grafico 3-D, in gradi. |
| [FilteredNSeries](../../aspose.cells.charts/chart/filterednseries/) { get; } | Ottiene una collezione [`SeriesCollection`](../seriescollection/) che rappresenta le serie di dati filtrate nel grafico. |
| [FirstSliceAngle](../../aspose.cells.charts/chart/firstsliceangle/) { get; set; } | Ottiene o imposta l'angolo della prima fetta di grafico a torta o di ciambella, in gradi (in senso orario dal verticale). Si applica solo a grafici a torta, a torta 3-D e a ciambella, da 0 a 360. |
| [Floor](../../aspose.cells.charts/chart/floor/) { get; } | Restituisce un oggetto [`Floor`](./floor/) che rappresenta le pareti di un grafico 3-D. |
| [GapDepth](../../aspose.cells.charts/chart/gapdepth/) { get; set; } | Ottiene o imposta la distanza tra le serie di dati in un grafico 3-D, come percentuale della larghezza del marcatore. Il valore di questa proprietà deve essere compreso tra 0 e 500. |
| [GapWidth](../../aspose.cells.charts/chart/gapwidth/) { get; set; } | Restituisce o imposta lo spazio tra i raggruppamenti di barre o colonne, come percentuale della larghezza della barra o della colonna. Il valore di questa proprietà deve essere compreso tra 0 e 500. |
| [HeightPercent](../../aspose.cells.charts/chart/heightpercent/) { get; set; } | Restituisce o imposta l'altezza di un grafico 3-D come percentuale della larghezza del grafico (tra il 5 e il 500 percento). |
| [HidePivotFieldButtons](../../aspose.cells.charts/chart/hidepivotfieldbuttons/) { get; set; } | Indica se nascondere i pulsanti dei campi del grafico pivot solo quando il grafico è un PivotChart. |
| [Is3D](../../aspose.cells.charts/chart/is3d/) { get; } | Indica se il grafico è un grafico 3D. |
| [IsRectangularCornered](../../aspose.cells.charts/chart/isrectangularcornered/) { get; set; } | Ottiene o imposta un valore che indica se l'area del grafico ha angoli rettangolari. Il valore predefinito è true. |
| [Legend](../../aspose.cells.charts/chart/legend/) { get; } | Ottiene la legenda del grafico. |
| [Line](../../aspose.cells.charts/chart/line/) { get; } | Ottiene la linea. |
| [Name](../../aspose.cells.charts/chart/name/) { get; set; } | Ottiene e imposta il nome del grafico. |
| [NSeries](../../aspose.cells.charts/chart/nseries/) { get; } | Ottiene una collezione [`SeriesCollection`](../seriescollection/) che rappresenta le serie di dati nel grafico. |
| [PageSetup](../../aspose.cells.charts/chart/pagesetup/) { get; } | Rappresenta la descrizione dell'impostazione pagina in questo grafico. |
| [Perspective](../../aspose.cells.charts/chart/perspective/) { get; set; } | Restituisce o imposta la prospettiva per la visualizzazione tridimensionale del grafico. Deve essere compresa tra 0 e 100. Questa proprietà è ignorata se la proprietà RightAngleAxes è True. |
| [PivotOptions](../../aspose.cells.charts/chart/pivotoptions/) { get; } | Specifica i controlli pivot che appaiono sul grafico |
| [PivotSource](../../aspose.cells.charts/chart/pivotsource/) { get; set; } | L'origine è i dati della tabella pivot. Se PivotSource non è vuoto, il grafico è un PivotChart. |
| [Placement](../../aspose.cells.charts/chart/placement/) { get; set; } | Rappresenta il modo in cui il grafico è collegato alle celle sottostanti. |
| [PlotArea](../../aspose.cells.charts/chart/plotarea/) { get; } | Ottiene l'area di tracciamento del grafico che include le etichette di graduazione degli assi. |
| [PlotBy](../../aspose.cells.charts/chart/plotby/) { get; } | Ottiene e imposta se tracciare per riga o per colonna. |
| [PlotEmptyCellsType](../../aspose.cells.charts/chart/plotemptycellstype/) { get; set; } | Ottiene e imposta come tracciare le celle vuote. |
| [PlotVisibleCells](../../aspose.cells.charts/chart/plotvisiblecells/) { get; set; } | (**Obsolete.**) Indica se visualizzare solo le celle del grafico visibili. |
| [PlotVisibleCellsOnly](../../aspose.cells.charts/chart/plotvisiblecellsonly/) { get; set; } | Indica se visualizzare solo le celle del grafico visibili. |
| [PrintSize](../../aspose.cells.charts/chart/printsize/) { get; set; } | Ottiene e imposta la dimensione stampata del grafico. |
| [RightAngleAxes](../../aspose.cells.charts/chart/rightangleaxes/) { get; set; } | Vero se gli assi del grafico sono perpendicolari. Si applica solo ai grafici 3-D (eccetto Column3D e grafici a torta 3-D). |
| [RotationAngle](../../aspose.cells.charts/chart/rotationangle/) { get; set; } | Rappresenta la rotazione della visualizzazione del grafico 3-D (la rotazione dell'area del grafico attorno all'asse z, in gradi). |
| [SecondCategoryAxis](../../aspose.cells.charts/chart/secondcategoryaxis/) { get; } | Ottiene il secondo asse X del grafico. |
| [SecondValueAxis](../../aspose.cells.charts/chart/secondvalueaxis/) { get; } | Ottiene il secondo asse Y del grafico. |
| [SeriesAxis](../../aspose.cells.charts/chart/seriesaxis/) { get; } | Ottiene l'asse delle serie del grafico. |
| [Shapes](../../aspose.cells.charts/chart/shapes/) { get; } | Restituisce tutte le forme di disegno in questo grafico. |
| [ShowDataTable](../../aspose.cells.charts/chart/showdatatable/) { get; set; } | Ottiene o imposta un valore che indica se il grafico visualizza una tabella dati. |
| [ShowLegend](../../aspose.cells.charts/chart/showlegend/) { get; set; } | Ottiene o imposta un valore che indica se la legenda del grafico verrà visualizzata. Il valore predefinito è vero. |
| [SideWall](../../aspose.cells.charts/chart/sidewall/) { get; } | Restituisce un oggetto [`Walls`](./walls/) che rappresenta la parete laterale di un grafico 3-D. |
| [SizeWithWindow](../../aspose.cells.charts/chart/sizewithwindow/) { get; set; } | Vero se Microsoft Excel ridimensiona il grafico per corrispondere alle dimensioni della finestra del foglio del grafico. |
| [Style](../../aspose.cells.charts/chart/style/) { get; set; } | Ottiene e imposta lo stile incorporato. |
| [SubTitle](../../aspose.cells.charts/chart/subtitle/) { get; } | Ottiene il sottotitolo del grafico. Si applica solo ai file ODS. |
| [Title](../../aspose.cells.charts/chart/title/) { get; } | Ottiene il titolo del grafico. |
| [Type](../../aspose.cells.charts/chart/type/) { get; set; } | Ottiene o imposta il tipo di grafico. |
| [ValueAxis](../../aspose.cells.charts/chart/valueaxis/) { get; } | Ottiene l'asse Y del grafico. |
| [Walls](../../aspose.cells.charts/chart/walls/) { get; } | Restituisce un oggetto [`Walls`](./walls/) che rappresenta le pareti di un grafico 3-D. |
| [WallsAndGridlines2D](../../aspose.cells.charts/chart/wallsandgridlines2d/) { get; set; } | Vero se le linee della griglia sono disegnate bidimensionalmente su un grafico 3-D. |
| [Worksheet](../../aspose.cells.charts/chart/worksheet/) { get; } | Ottiene il foglio di lavoro che contiene questo grafico. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Calculate](../../aspose.cells.charts/chart/calculate/#calculate)() | Calcola le posizioni personalizzate dell'area del grafico e degli assi se le loro posizioni sono assegnate automaticamente. |
| [Calculate](../../aspose.cells.charts/chart/calculate/#calculate_1)(ChartCalculateOptions) | Calcola la posizione personalizzata dell'area del grafico e degli assi se le loro posizioni sono assegnate automaticamente, con le Opzioni di Calcolo del Grafico. |
| [ChangeTemplate](../../aspose.cells.charts/chart/changetemplate/)(byte[]) | Cambia il tipo di grafico con un modello predefinito. |
| [GetActualSize](../../aspose.cells.charts/chart/getactualsize/)() | Ottiene la dimensione reale del grafico in unità di pixel. |
| [GetChartDataRange](../../aspose.cells.charts/chart/getchartdatarange/)() | Ottiene l'intervallo della sorgente dati del grafico. |
| [HasAxis](../../aspose.cells.charts/chart/hasaxis/)(AxisType, bool) | Restituisce quali assi esistono nel grafico. |
| [IsCellReferedByChart](../../aspose.cells.charts/chart/iscellreferedbychart/)(int, int, int) | Restituisce se la cella è riferita dal grafico. |
| [IsChartDataChanged](../../aspose.cells.charts/chart/ischartdatachanged/)() | Rileva se la sorgente dati di un grafico è cambiata. |
| [IsReferedByChart](../../aspose.cells.charts/chart/isreferedbychart/)(int, int) | (**Obsolete.**) Restituisce se la cella è riferita dal grafico. |
| [Move](../../aspose.cells.charts/chart/move/)(int, int, int, int) | Sposta il grafico in una posizione specificata. |
| [RefreshPivotData](../../aspose.cells.charts/chart/refreshpivotdata/)() | Aggiorna i dati del grafico dalla tabella pivot. |
| [SetChartDataRange](../../aspose.cells.charts/chart/setchartdatarange/)(string, bool) | Specifica l'intervallo di dati per un grafico. |
| [SwitchRowColumn](../../aspose.cells.charts/chart/switchrowcolumn/)() | Scambia riga/colonna. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage)() | Ottiene un oggetto `Bitmap` a 32 bit del grafico. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_1)(ImageOrPrintOptions) | Ottiene un oggetto `Bitmap` a 32 bit del grafico. Gli attributi `ImageOrPrintOptions.ImageFormat`, ImageOrPrintOptions.TiffCompression e ImageOrPrintOptions.Quality sono ignorati. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_6)(string) | Crea l'immagine del grafico e la salva in un file. L'estensione del nome file determina il formato dell'immagine. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_5)(Stream, ImageFormat) | (**Obsolete.**) Crea l'immagine del grafico e la salva in uno stream nel formato specificato. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_3)(Stream, ImageOrPrintOptions) | Crea l'immagine del grafico e la salva in uno stream nel formato specificato. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_2)(Stream, ImageType) | Crea l'immagine del grafico e la salva in uno stream nel formato specificato. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_4)(Stream, long) | Crea l'immagine del grafico e la salva in uno stream nel formato Jpeg. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_10)(string, ImageFormat) | (**Obsolete.**) Crea l'immagine del grafico e la salva in un file nel formato specificato. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_8)(string, ImageOrPrintOptions) | Crea l'immagine del grafico e la salva in un file. L'estensione del nome file determina il formato dell'immagine. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_7)(string, ImageType) | Crea l'immagine del grafico e la salva in un file nel tipo di immagine specificato. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_9)(string, long) | (**Obsolete.**) Crea l'immagine del grafico e la salva in un file nel formato Jpeg. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf)(Stream) | Crea il PDF del grafico e lo salva in uno stream. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_2)(string) | Salva il grafico in un file PDF. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_1)(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Crea il PDF del grafico e lo salva in uno stream. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_3)(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Salva il grafico in un file PDF. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartDemo
    {
        public static void ChartExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells[0, 1].PutValue("Income");
            worksheet.Cells[1, 0].PutValue("Company A");
            worksheet.Cells[2, 0].PutValue("Company B");
            worksheet.Cells[3, 0].PutValue("Company C");
            worksheet.Cells[1, 1].PutValue(10000);
            worksheet.Cells[2, 1].PutValue(20000);
            worksheet.Cells[3, 1].PutValue(30000);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo di dati per il grafico
            chart.SetChartDataRange("A1:B4", true);

            // Imposta le proprietà del grafico
            chart.ShowLegend = true;
            chart.Title.Text = "Income Analysis";
            chart.Style = 2; // Built-in style

            // Personalizza l'aspetto del grafico
            chart.ChartObject.Name = "IncomeChart";
            chart.PlotEmptyCellsType = PlotEmptyCellsType.NotPlotted;
            chart.PlotVisibleCells = true;
            chart.DisplayNaAsBlank = true;
            chart.SizeWithWindow = true;

            // Personalizza gli assi del grafico
            chart.CategoryAxis.Title.Text = "Companies";
            chart.ValueAxis.Title.Text = "Income";
            chart.CategoryAxis.MajorTickMark = TickMarkType.Outside;
            chart.ValueAxis.MajorTickMark = TickMarkType.Outside;

            // Personalizza la legenda del grafico
            chart.Legend.Position = LegendPositionType.Bottom;
            chart.Legend.IsOverLay = false;

            // Personalizza l'area del tracciato del grafico
            chart.PlotArea.Area.ForegroundColor = Color.LightYellow;
            chart.PlotArea.Border.IsVisible = false;

            // Personalizza l'area del grafico
            chart.ChartArea.Area.ForegroundColor = Color.LightBlue;
            chart.ChartArea.Border.IsVisible = false;

            // Salva la cartella di lavoro
            workbook.Save("ChartExample.xlsx");
            workbook.Save("ChartExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


