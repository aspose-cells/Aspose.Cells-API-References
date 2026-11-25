---
title: "Classe DisplayUnitLabel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Charts.DisplayUnitLabel. Rappresenta l'etichetta dell'unità di visualizzazione"
type: docs
url: /it/net/aspose.cells.charts/displayunitlabel/
---
## DisplayUnitLabel class

Rappresenta l'etichetta dell'unità di visualizzazione.

```csharp
public class DisplayUnitLabel : ChartTextFrame
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area/) { get; } | Ottiene il [`area`](../chartframe/area/).(Ereditato da [`ChartFrame`](../chartframe/).) |
| override [AutoScaleFont](../../aspose.cells.charts/displayunitlabel/autoscalefont/) { get; set; } | True se il testo nell'oggetto cambia dimensione del carattere quando le dimensioni dell'oggetto cambiano. Il valore predefinito è True. |
| [Background](../../aspose.cells.charts/chartframe/background/) { get; set; } | (**Obsolete.**) Ottiene e imposta la modalità di visualizzazione dello sfondo. Questa proprietà è valida solo in Excel 2003 o versioni precedenti.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode/) { get; set; } | (**Obsolete.**) Ottiene e imposta la modalità di visualizzazione dello sfondo. Questa proprietà è valida solo in Excel 2003 o versioni precedenti.(Ereditato da [`ChartFrame`](../chartframe/).) |
| virtual [Border](../../aspose.cells.charts/chartframe/border/) { get; } | Ottiene il [`border`](../../aspose.cells.drawing/line/).(Ereditato da [`ChartFrame`](../chartframe/).) |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight/) { get; } | (**Obsolete.**) Rappresenta l'altezza della posizione predefinita in unità di 1/4000 dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [DefaultHeightRatioToChart](../../aspose.cells.charts/chartframe/defaultheightratiotochart/) { get; } | Rappresenta l'altezza della posizione predefinita in unità della frazione dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth/) { get; } | (**Obsolete.**) Rappresenta la larghezza della posizione predefinita in unità di 1/4000 dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [DefaultWidthRatioToChart](../../aspose.cells.charts/chartframe/defaultwidthratiotochart/) { get; } | Rappresenta la larghezza della posizione predefinita in unità della frazione dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx/) { get; } | (**Obsolete.**) Rappresenta x della posizione predefinita in unità di 1/4000 dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [DefaultXRatioToChart](../../aspose.cells.charts/chartframe/defaultxratiotochart/) { get; } | Rappresenta x della posizione predefinita in unità della frazione dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty/) { get; } | (**Obsolete.**) Rappresenta y della posizione predefinita in unità di 1/4000 dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [DefaultYRatioToChart](../../aspose.cells.charts/chartframe/defaultyratiotochart/) { get; } | Rappresenta y della posizione predefinita in unità della frazione dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype/) { get; set; } | Ottiene e imposta la direzione del testo.(Ereditato da [`ChartTextFrame`](../charttextframe/).) |
| override [Font](../../aspose.cells.charts/displayunitlabel/font/) { get; } | Ottiene un oggetto [`Font`](./font/) del specificato oggetto ChartFrame. |
| virtual [Height](../../aspose.cells.charts/chartframe/height/) { get; set; } | (**Obsolete.**) Ottiene o imposta l'altezza del frame in unità di 1/4000 dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| virtual [HeightPixel](../../aspose.cells.charts/chartframe/heightpixel/) { get; set; } | Ottiene o imposta l'altezza del frame in unità di pixel.(Ereditato da [`ChartFrame`](../chartframe/).) |
| virtual [HeightRatioToChart](../../aspose.cells.charts/chartframe/heightratiotochart/) { get; set; } | Ottiene o imposta l'altezza del frame in unità del rapporto dell'area del grafico.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [IsAutomaticRotation](../../aspose.cells.charts/charttextframe/isautomaticrotation/) { get; } | Indica se il testo del grafico è ruotato automaticamente.(Ereditato da [`ChartTextFrame`](../charttextframe/).) |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize/) { get; set; } | Indica se il frame del grafico è dimensionato automaticamente.(Ereditato da [`ChartFrame`](../chartframe/).) |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext/) { get; set; } | Indica che il testo è generato automaticamente.(Ereditato da [`ChartTextFrame`](../charttextframe/).) |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset/) { get; } | Indica se la posizione predefinita (DefaultX, DefaultY, DefaultWidth e DefaultHeight) è impostata.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted/) { get; set; } | Indica se questa etichetta dati è eliminata.(Ereditato da [`ChartTextFrame`](../charttextframe/).) |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode/) { get; set; } | Indica se la dimensione dell'area del grafico include le tacche e le etichette degli assi. False specifica che la dimensione deve determinare la dimensione dell'area del grafico, le tacche e le etichette degli assi.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext/) { get; set; } | Ottiene o imposta se una forma deve adattarsi automaticamente per contenere completamente il testo al suo interno. L'adattamento automatico avviene quando il testo all'interno di una forma viene scalato per contenere tutto il testo.(Ereditato da [`ChartTextFrame`](../charttextframe/).) |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped/) { get; set; } | Ottiene o imposta un valore che indica se il testo è a capo.(Ereditato da [`ChartTextFrame`](../charttextframe/).) |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource/) { get; set; } | Ottiene e imposta un riferimento al foglio di lavoro.(Ereditato da [`ChartTextFrame`](../charttextframe/).) |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder/) { get; set; } | Rappresenta l'ordine di lettura del testo.(Ereditato da [`ChartTextFrame`](../charttextframe/).) |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle/) { get; set; } | Rappresenta l'angolo di rotazione del testo.(Ereditato da [`ChartTextFrame`](../charttextframe/).) |
| [Shadow](../../aspose.cells.charts/chartframe/shadow/) { get; set; } | True se il frame ha un'ombra.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties/) { get; } | Ottiene l'oggetto [`ShapeProperties`](../chartframe/shapeproperties/).(Ereditato da [`ChartFrame`](../chartframe/).) |
| override [Text](../../aspose.cells.charts/displayunitlabel/text/) { get; set; } | Ottiene o imposta il testo dell'etichetta dell'unità di visualizzazione. |
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
| [Characters](../../aspose.cells.charts/charttextframe/characters/)(int, int) | Restituisce un oggetto Characters che rappresenta un intervallo di caratteri all'interno del testo.(Ereditato da [`ChartTextFrame`](../charttextframe/).) |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto/)() | Imposta la posizione del frame su automatico(Ereditato da [`ChartFrame`](../chartframe/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class DisplayUnitLabelDemo
    {
        public static void DisplayUnitLabelExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            // Aggiungere un nuovo foglio di lavoro all'oggetto Workbook
            int sheetIndex = workbook.Worksheets.Add();
            // Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice di foglio
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Aggiunta di valori di esempio alle celle
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Aggiunta di un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            // Accesso all'istanza del grafico appena aggiunto
            Chart chart = worksheet.Charts[chartIndex];
            // Aggiunta di NSeries (origine dati del grafico) al grafico che va dalla cella "A1" alla "B4"
            chart.NSeries.Add("A1:B4", true);
            // Impostazione dell'origine dati per i dati di categoria di NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Impostazione dell'unità di visualizzazione dell'asse dei valori (Y)
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
            DisplayUnitLabel displayUnitLabel = chart.ValueAxis.DisplayUnitLabel;

            // Impostazione delle proprietà di DisplayUnitLabel
            displayUnitLabel.Text = "100";
            displayUnitLabel.AutoScaleFont = true;
            displayUnitLabel.IsAutoText = false;
            displayUnitLabel.IsDeleted = false;
            displayUnitLabel.TextHorizontalAlignment = TextAlignmentType.Center;
            displayUnitLabel.TextVerticalAlignment = TextAlignmentType.Center;
            displayUnitLabel.RotationAngle = 0;
            displayUnitLabel.LinkedSource = "";
            displayUnitLabel.TextDirection = TextDirectionType.LeftToRight;
            displayUnitLabel.ReadingOrder = TextDirectionType.LeftToRight;
            displayUnitLabel.DirectionType = ChartTextDirectionType.Horizontal;
            displayUnitLabel.IsTextWrapped = false;
            displayUnitLabel.IsResizeShapeToFitText = false;
            displayUnitLabel.IsInnerMode = false;
            displayUnitLabel.BackgroundMode = BackgroundMode.Transparent;
            displayUnitLabel.IsAutomaticSize = true;
            displayUnitLabel.X = 0;
            displayUnitLabel.Y = 0;
            displayUnitLabel.Height = 100;
            displayUnitLabel.Width = 100;
            displayUnitLabel.Shadow = false;

            // Salvataggio del file Excel
            workbook.Save("DisplayUnitLabelExample.xlsx");
            workbook.Save("DisplayUnitLabelExample.pdf");
        }
    }
}
```

### Vedi anche

* class [ChartTextFrame](../charttextframe/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


