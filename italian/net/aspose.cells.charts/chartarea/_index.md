---
title: "Classe ChartArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.ChartArea classe. Incapsula l'oggetto che rappresenta l'area del grafico nel foglio di lavoro."
type: docs
url: /it/net/aspose.cells.charts/chartarea/
---
## ChartArea class

Incapsula l'oggetto che rappresenta l'area del grafico nel foglio di lavoro.

```csharp
public class ChartArea : ChartFrame
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area/) { get; } | Ottiene il [`area`](../chartframe/area/).(Ereditato da [`ChartFrame`](../chartframe/).) |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont/) { get; set; } | True se il testo nell'oggetto cambia la dimensione del carattere quando la dimensione dell'oggetto cambia. Il valore predefinito è True.(Ereditato da [`ChartFrame`](../chartframe/).) |
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
| override [Font](../../aspose.cells.charts/chartarea/font/) { get; } | Restituisce un oggetto [`Font`](./font/) dell'oggetto ChartArea specificato. |
| override [Height](../../aspose.cells.charts/chartarea/height/) { get; set; } | (**Obsolete.**) Restituisce o imposta lo spostamento verticale dalla riga dell'angolo inferiore‑destro, in unità di 1/4000 dell'area del grafico. |
| virtual [HeightPixel](../../aspose.cells.charts/chartframe/heightpixel/) { get; set; } | Ottiene o imposta l'altezza del frame in unità di pixel.(Ereditato da [`ChartFrame`](../chartframe/).) |
| override [HeightRatioToChart](../../aspose.cells.charts/chartarea/heightratiotochart/) { get; set; } | Restituisce o imposta lo spostamento verticale dalla riga dell'angolo inferiore destro, in unità di rapporto dell'area del grafico. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize/) { get; set; } | Indica se il frame del grafico è dimensionato automaticamente.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset/) { get; } | Indica se la posizione predefinita (DefaultX, DefaultY, DefaultWidth e DefaultHeight) è impostata.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode/) { get; set; } | Indica se la dimensione dell'area del grafico include le tacche e le etichette degli assi. False specifica che la dimensione deve determinare la dimensione dell'area del grafico, le tacche e le etichette degli assi.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [Shadow](../../aspose.cells.charts/chartframe/shadow/) { get; set; } | True se il frame ha un'ombra.(Ereditato da [`ChartFrame`](../chartframe/).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties/) { get; } | Ottiene l'oggetto [`ShapeProperties`](../chartframe/shapeproperties/).(Ereditato da [`ChartFrame`](../chartframe/).) |
| virtual [TextFont](../../aspose.cells.charts/chartframe/textfont/) { get; } | (**Obsolete.**) Ottiene un oggetto [`Font`](../chartframe/font/) del ChartFrame specificato.(Ereditato da [`ChartFrame`](../chartframe/).) |
| virtual [TextOptions](../../aspose.cells.charts/chartframe/textoptions/) { get; } | Ottiene e imposta le opzioni del testo.(Ereditato da [`ChartFrame`](../chartframe/).) |
| override [Width](../../aspose.cells.charts/chartarea/width/) { get; set; } | (**Obsolete.**) Restituisce o imposta lo spostamento orizzontale dalla colonna dell'angolo inferiore destro, in unità di 1/4000 dell'area del grafico. |
| virtual [WidthPixel](../../aspose.cells.charts/chartframe/widthpixel/) { get; set; } | Ottiene o imposta la larghezza del frame in unità di Pixel.(Ereditato da [`ChartFrame`](../chartframe/).) |
| override [WidthRatioToChart](../../aspose.cells.charts/chartarea/widthratiotochart/) { get; set; } | Restituisce o imposta lo spostamento orizzontale dalla colonna dell'angolo inferiore destro, in unità di rapporto dell'area del grafico. |
| override [X](../../aspose.cells.charts/chartarea/x/) { get; set; } | (**Obsolete.**) Restituisce o imposta lo spostamento orizzontale dalla colonna dell'angolo superiore‑sinistro, in unità di 1/4000 dell'area del grafico. |
| virtual [XPixel](../../aspose.cells.charts/chartframe/xpixel/) { get; set; } | Ottiene o imposta la coordinata x dell'angolo in alto a sinistra in unità di Pixel.(Ereditato da [`ChartFrame`](../chartframe/).) |
| override [XRatioToChart](../../aspose.cells.charts/chartarea/xratiotochart/) { get; set; } | Restituisce o imposta lo spostamento orizzontale dalla colonna dell'angolo superiore‑sinistro, come rapporto dell'area del grafico. |
| override [Y](../../aspose.cells.charts/chartarea/y/) { get; set; } | (**Obsolete.**) Restituisce o ottiene lo spostamento verticale dalla riga dell'angolo superiore sinistro, in unità di 1/4000 dell'area del grafico. |
| virtual [YPixel](../../aspose.cells.charts/chartframe/ypixel/) { get; set; } | Ottiene o imposta la coordinata y dell'angolo in alto a sinistra in unità di pixel.(Ereditato da [`ChartFrame`](../chartframe/).) |
| override [YRatioToChart](../../aspose.cells.charts/chartarea/yratiotochart/) { get; set; } | Restituisce o ottiene lo spostamento verticale dalla riga dell'angolo superiore sinistro, in unità di rapporto dell'area del grafico. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto/)() | Imposta la posizione del frame su automatico(Ereditato da [`ChartFrame`](../chartframe/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartAreaDemo
    {
        public static void ChartAreaExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();

            // Ottenere il riferimento del primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiunta di un valore di esempio alla cella "A1"
            worksheet.Cells["A1"].PutValue(50);

            // Aggiunta di un valore di esempio alla cella "A2"
            worksheet.Cells["A2"].PutValue(100);

            // Aggiunta di un valore di esempio alla cella "A3"
            worksheet.Cells["A3"].PutValue(150);

            // Aggiunta di un valore di esempio alla cella "B1"
            worksheet.Cells["B1"].PutValue(60);

            // Aggiunta di un valore di esempio alla cella "B2"
            worksheet.Cells["B2"].PutValue(32);

            // Aggiunta di un valore di esempio alla cella "B3"
            worksheet.Cells["B3"].PutValue(50);

            // Aggiunta di un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);

            // Accesso all'istanza del grafico appena aggiunto
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiunta di NSeries (origine dati del grafico) al grafico dall'intervallo di celle "A1" a "B3"
            chart.NSeries.Add("A1:B3", true);

            // Ottenere l'area del grafico
            ChartArea chartArea = chart.ChartArea;

            // Impostazione delle proprietà dell'area del grafico
            chartArea.X = 10;
            chartArea.Y = 10;
            chartArea.Width = 400;
            chartArea.Height = 300;
            chartArea.IsInnerMode = false;
            chartArea.AutoScaleFont = true;
            chartArea.BackgroundMode = BackgroundMode.Transparent;
            chartArea.IsAutomaticSize = true;
            chartArea.Shadow = true;

            // Impostazione del colore di primo piano dell'area del diagramma
            chartArea.Area.ForegroundColor = Color.Yellow;

            // Salvataggio del file Excel
            workbook.Save("ChartAreaExample.xlsx");
            workbook.Save("ChartAreaExample.pdf");
        }
    }
}
```

### Vedi anche

* class [ChartFrame](../chartframe/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


