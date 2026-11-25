---
title: "Classe DataLabels"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Charts.DataLabels. Incapsula una collezione di tutti gli oggetti DataLabel per la Serie specificata"
type: docs
url: /it/net/aspose.cells.charts/datalabels/
---
## DataLabels class

Incapsula una raccolta di tutti gli oggetti DataLabel per la Serie specificata.

```csharp
public class DataLabels : ChartTextFrame
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| override [Area](../../aspose.cells.charts/datalabels/area/) { get; } | Ottiene il [`area`](./area/). |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont/) { get; set; } | True se il testo nell'oggetto cambia la dimensione del carattere quando la dimensione dell'oggetto cambia. Il valore predefinito è True.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [Background](../../aspose.cells.charts/chartframe/background/) { get; set; } | (**Obsolete.**) Ottiene e imposta la modalità di visualizzazione dello sfondo. Questa proprietà è valida solo in Excel 2003 o versioni precedenti.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [BackgroundMode](../../aspose.cells.charts/datalabels/backgroundmode/) { get; set; } | Ottiene e imposta la modalità di visualizzazione dello sfondo |
| override [Border](../../aspose.cells.charts/datalabels/border/) { get; } | Ottiene il [`border`](../../aspose.cells.drawing/line/). |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight/) { get; } | (**Obsolete.**) Rappresenta l'altezza della posizione predefinita in unità di 1/4000 dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [DefaultHeightRatioToChart](../../aspose.cells.charts/chartframe/defaultheightratiotochart/) { get; } | Rappresenta l'altezza della posizione predefinita in unità della frazione dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth/) { get; } | (**Obsolete.**) Rappresenta la larghezza della posizione predefinita in unità di 1/4000 dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [DefaultWidthRatioToChart](../../aspose.cells.charts/chartframe/defaultwidthratiotochart/) { get; } | Rappresenta la larghezza della posizione predefinita in unità della frazione dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx/) { get; } | (**Obsolete.**) Rappresenta x della posizione predefinita in unità di 1/4000 dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [DefaultXRatioToChart](../../aspose.cells.charts/chartframe/defaultxratiotochart/) { get; } | Rappresenta x della posizione predefinita in unità della frazione dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty/) { get; } | (**Obsolete.**) Rappresenta y della posizione predefinita in unità di 1/4000 dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [DefaultYRatioToChart](../../aspose.cells.charts/chartframe/defaultyratiotochart/) { get; } | Rappresenta y della posizione predefinita in unità della frazione dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| override [DirectionType](../../aspose.cells.charts/datalabels/directiontype/) { get; set; } | Ottiene e imposta la direzione del testo. |
| override [Font](../../aspose.cells.charts/datalabels/font/) { get; } | Ottiene il carattere dei DataLabels; |
| virtual [Height](../../aspose.cells.charts/chartframe/height/) { get; set; } | (**Obsolete.**) Ottiene o imposta l'altezza del frame in unità di 1/4000 dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| virtual [HeightPixel](../../aspose.cells.charts/chartframe/heightpixel/) { get; set; } | Ottiene o imposta l'altezza del frame in unità di pixel.(Ereditato da [`ChartFrame`](../chartframe/).) |
| virtual [HeightRatioToChart](../../aspose.cells.charts/chartframe/heightratiotochart/) { get; set; } | Ottiene o imposta l'altezza del frame in unità del rapporto dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [IsAutomaticRotation](../../aspose.cells.charts/charttextframe/isautomaticrotation/) { get; } | Indica se il testo del grafico è ruotato automaticamente.(Ereditato da [`ChartTextFrame`](../charttextframe/).) |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize/) { get; set; } | Indica se il frame del grafico è dimensionato automaticamente.(Ereditato da [`ChartFrame`](../chartframe/).) |
| override [IsAutoText](../../aspose.cells.charts/datalabels/isautotext/) { get; set; } | Indica che il testo è generato automaticamente. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset/) { get; } | Indica se la posizione predefinita (DefaultX, DefaultY, DefaultWidth e DefaultHeight) è impostata.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted/) { get; set; } | Indica se questa etichetta dati è eliminata.(Ereditato da [`ChartTextFrame`](../charttextframe/).) |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode/) { get; set; } | Indica se la dimensione dell'area del grafico include le tacche e le etichette degli assi. False specifica che la dimensione deve determinare la dimensione dell'area del grafico, le tacche e le etichette degli assi.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [IsNeverOverlap](../../aspose.cells.charts/datalabels/isneveroverlap/) { get; set; } | Indica se le etichette dati non si sovrappongono mai durante la creazione di un'immagine di grafico a torta. Nota: questa proprietà è significativa solo quando si crea un'immagine di grafico a torta. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext/) { get; set; } | Ottiene o imposta se una forma deve adattarsi automaticamente per contenere completamente il testo al suo interno. L'adattamento automatico avviene quando il testo all'interno di una forma viene scalato per contenere tutto il testo.(Ereditato da [`ChartTextFrame`](../charttextframe/).) |
| override [IsTextWrapped](../../aspose.cells.charts/datalabels/istextwrapped/) { get; set; } | Ottiene o imposta un valore che indica se il testo è a capo. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource/) { get; set; } | Ottiene e imposta un riferimento al foglio di lavoro.(Ereditato da [`ChartTextFrame`](../charttextframe/).) |
| [Number](../../aspose.cells.charts/datalabels/number/) { get; set; } | Ottiene e imposta il formato numerico incorporato. |
| [NumberFormat](../../aspose.cells.charts/datalabels/numberformat/) { get; set; } | Rappresenta la stringa di formato per l'oggetto DataLabels. |
| [NumberFormatLinked](../../aspose.cells.charts/datalabels/numberformatlinked/) { get; set; } | True se il formato numerico è collegato alle celle (in modo che il formato numerico cambi nelle etichette quando cambia nelle celle). |
| [Position](../../aspose.cells.charts/datalabels/position/) { get; set; } | Rappresenta la posizione dell'etichetta dati. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder/) { get; set; } | Rappresenta l'ordine di lettura del testo.(Ereditato da [`ChartTextFrame`](../charttextframe/).) |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle/) { get; set; } | Rappresenta l'angolo di rotazione del testo.(Ereditato da [`ChartTextFrame`](../charttextframe/).) |
| [SeparatorType](../../aspose.cells.charts/datalabels/separatortype/) { get; set; } | Ottiene o imposta il tipo di separatore utilizzato per le etichette dati in un grafico. |
| [SeparatorValue](../../aspose.cells.charts/datalabels/separatorvalue/) { get; set; } | Ottiene o imposta il valore del separatore utilizzato per le etichette dati in un grafico. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow/) { get; set; } | True se il frame ha un'ombra.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties/) { get; } | Ottiene l'oggetto [`ShapeProperties`](../chartframe/shapeproperties/).(Ereditato da [`ChartFrame`](../chartframe/).) |
| [ShapeType](../../aspose.cells.charts/datalabels/shapetype/) { get; set; } | Ottiene o imposta il tipo di forma dell'etichetta dati. |
| [ShowBubbleSize](../../aspose.cells.charts/datalabels/showbubblesize/) { get; set; } | Rappresenta il comportamento di visualizzazione del valore percentuale dell'etichetta dati di un grafico specificato. True visualizza il valore percentuale. False lo nasconde. |
| [ShowCategoryName](../../aspose.cells.charts/datalabels/showcategoryname/) { get; set; } | Rappresenta il comportamento di visualizzazione del nome della categoria dell'etichetta dati di un grafico specificato. True per visualizzare il nome della categoria per le etichette dati in un grafico. False per nasconderlo. |
| [ShowCellRange](../../aspose.cells.charts/datalabels/showcellrange/) { get; set; } | Indica se mostrare l'intervallo di celle come etichette dati. |
| [ShowLegendKey](../../aspose.cells.charts/datalabels/showlegendkey/) { get; set; } | Rappresenta il comportamento di visualizzazione della chiave legenda dell'etichetta dati di un grafico specificato. True se la chiave legenda dell'etichetta dati è visibile. |
| [ShowPercentage](../../aspose.cells.charts/datalabels/showpercentage/) { get; set; } | Rappresenta il comportamento di visualizzazione del valore percentuale dell'etichetta dati di un grafico specificato. True visualizza il valore percentuale. False lo nasconde. |
| [ShowSeriesName](../../aspose.cells.charts/datalabels/showseriesname/) { get; set; } | Indica se il nome della serie viene visualizzato sulle etichette dati in un grafico. True per mostrare il nome della serie. False per nasconderlo. |
| [ShowValue](../../aspose.cells.charts/datalabels/showvalue/) { get; set; } | Rappresenta il comportamento di visualizzazione dei valori dell'etichetta dati di un grafico specificato. True visualizza i valori. False li nasconde. |
| override [Text](../../aspose.cells.charts/datalabels/text/) { get; set; } | Ottiene o imposta il testo dell'etichetta dati. |
| [TextDirection](../../aspose.cells.charts/charttextframe/textdirection/) { get; set; } | (**Obsolete.**) Rappresenta l'ordine di lettura del testo.(Ereditato da [`ChartTextFrame`](../charttextframe/).) |
| virtual [TextFont](../../aspose.cells.charts/chartframe/textfont/) { get; } | (**Obsolete.**) Ottiene un oggetto [`Font`](../chartframe/font/) del ChartFrame specificato.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment/) { get; set; } | Ottiene e imposta l'allineamento orizzontale del testo.(Ereditato da [`ChartTextFrame`](../charttextframe/).) |
| virtual [TextOptions](../../aspose.cells.charts/chartframe/textoptions/) { get; } | Ottiene e imposta le opzioni del testo.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment/) { get; set; } | Ottiene o imposta l'allineamento verticale del testo.(Ereditato da [`ChartTextFrame`](../charttextframe/).) |
| virtual [Width](../../aspose.cells.charts/chartframe/width/) { get; set; } | (**Obsolete.**) Ottiene o imposta la larghezza del frame in unità di 1/4000 dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| virtual [WidthPixel](../../aspose.cells.charts/chartframe/widthpixel/) { get; set; } | Ottiene o imposta la larghezza del frame in unità di Pixel.(Ereditato da [`ChartFrame`](../chartframe/).) |
| virtual [WidthRatioToChart](../../aspose.cells.charts/chartframe/widthratiotochart/) { get; set; } | Ottiene o imposta la larghezza del frame in unità di rapporto dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| virtual [X](../../aspose.cells.charts/chartframe/x/) { get; set; } | (**Obsolete.**) Ottiene o imposta la coordinata x dell'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico. (Ereditato da [`ChartFrame`](../chartframe/).) |
| virtual [XPixel](../../aspose.cells.charts/chartframe/xpixel/) { get; set; } | Ottiene o imposta la coordinata x dell'angolo in alto a sinistra in unità di Pixel.(Ereditato da [`ChartFrame`](../chartframe/).) |
| virtual [XRatioToChart](../../aspose.cells.charts/chartframe/xratiotochart/) { get; set; } | Ottiene o imposta la coordinata x dell'angolo in alto a sinistra in unità di rapporto dell'area del grafico. (Ereditato da [`ChartFrame`](../chartframe/).) |
| virtual [Y](../../aspose.cells.charts/chartframe/y/) { get; set; } | (**Obsolete.**) Ottiene o imposta la coordinata y dell'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico. (Ereditato da [`ChartFrame`](../chartframe/).) |
| virtual [YPixel](../../aspose.cells.charts/chartframe/ypixel/) { get; set; } | Ottiene o imposta la coordinata y dell'angolo in alto a sinistra in unità di pixel.(Ereditato da [`ChartFrame`](../chartframe/).) |
| virtual [YRatioToChart](../../aspose.cells.charts/chartframe/yratiotochart/) { get; set; } | Ottiene o imposta la coordinata y dell'angolo in alto a sinistra in unità di rapporto dell'area del grafico. (Ereditato da [`ChartFrame`](../chartframe/).) |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ApplyFont](../../aspose.cells.charts/datalabels/applyfont/)() | Applica il carattere delle etichette dati a tutti i nodi figlio. |
| [Characters](../../aspose.cells.charts/charttextframe/characters/)(int, int) | Restituisce un oggetto Characters che rappresenta un intervallo di caratteri all'interno del testo.(Ereditato da [`ChartTextFrame`](../charttextframe/).) |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto/)() | Imposta la posizione del frame su automatico(Ereditato da [`ChartFrame`](../chartframe/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class DataLabelsDemo
    {
        public static void DataLabelsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi serie al grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi alle DataLabels della prima serie
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // Imposta le proprietà delle DataLabels
            dataLabels.Position = LabelPositionType.InsideBase;
            dataLabels.ShowCategoryName = true;
            dataLabels.ShowValue = true;
            dataLabels.ShowPercentage = false;
            dataLabels.ShowLegendKey = false;
            dataLabels.IsAutoText = true;
            dataLabels.DirectionType = ChartTextDirectionType.Horizontal;
            dataLabels.Text = "Custom Text";
            dataLabels.IsTextWrapped = true;
            dataLabels.BackgroundMode = BackgroundMode.Transparent;
            dataLabels.ShowCellRange = false;
            dataLabels.ShowBubbleSize = false;
            dataLabels.ShowSeriesName = false;
            dataLabels.NumberFormat = "0.00";
            dataLabels.Number = 0;
            dataLabels.NumberFormatLinked = false;
            dataLabels.SeparatorType = DataLabelsSeparatorType.Comma;
            dataLabels.SeparatorValue = ", ";
            dataLabels.IsNeverOverlap = true;
            dataLabels.IsDeleted = false;
            dataLabels.TextHorizontalAlignment = TextAlignmentType.Center;
            dataLabels.TextVerticalAlignment = TextAlignmentType.Center;
            dataLabels.RotationAngle = 0;
            dataLabels.LinkedSource = "";
            dataLabels.TextDirection = TextDirectionType.LeftToRight;
            dataLabels.ReadingOrder = TextDirectionType.LeftToRight;
            dataLabels.IsResizeShapeToFitText = true;
            dataLabels.IsInnerMode = false;
            dataLabels.AutoScaleFont = true;
            dataLabels.Background = BackgroundMode.Transparent;
            dataLabels.IsAutomaticSize = true;
            dataLabels.X = 0;
            dataLabels.Y = 0;
            dataLabels.Height = 100;
            dataLabels.Width = 100;
            dataLabels.Shadow = false;

            // Salva la cartella di lavoro
            workbook.Save("DataLabelsExample.xlsx");
            workbook.Save("DataLabelsExample.pdf");
        }
    }
}
```

### Vedi anche

* class [ChartTextFrame](../charttextframe/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


