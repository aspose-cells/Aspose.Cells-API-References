---
title: "Classe TickLabels"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Charts.TickLabels. Rappresenta le etichette dei segni di graduazione associate ai segni di graduazione su un asse del grafico"
type: docs
url: /it/net/aspose.cells.charts/ticklabels/
---
## TickLabels class

Rappresenta le etichette dei segni di graduazione associate ai segni di graduazione su un asse del grafico.

```csharp
public class TickLabels
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AlignmentType](../../aspose.cells.charts/ticklabels/alignmenttype/) { get; set; } | Ottiene e imposta l'allineamento del testo per le etichette dei segni sull'asse. |
| [AutoScaleFont](../../aspose.cells.charts/ticklabels/autoscalefont/) { get; set; } | True se il testo nell'oggetto cambia dimensione del carattere quando le dimensioni dell'oggetto cambiano. Il valore predefinito è True. |
| [BackgroundMode](../../aspose.cells.charts/ticklabels/backgroundmode/) { get; set; } | Ottiene e imposta la modalità di visualizzazione dello sfondo |
| [DirectionType](../../aspose.cells.charts/ticklabels/directiontype/) { get; set; } | Ottiene e imposta la direzione del testo. |
| [DisplayNumberFormat](../../aspose.cells.charts/ticklabels/displaynumberformat/) { get; } | Ottiene e imposta il formato numerico di visualizzazione delle etichette dei segni. |
| [Font](../../aspose.cells.charts/ticklabels/font/) { get; } | Restituisce un oggetto [`Font`](./font/) che rappresenta il carattere dell'oggetto TickLabels specificato. |
| [IsAutomaticRotation](../../aspose.cells.charts/ticklabels/isautomaticrotation/) { get; set; } | Indica se l'angolo di rotazione è automatico |
| [Number](../../aspose.cells.charts/ticklabels/number/) { get; set; } | Rappresenta il numero di formato per l'oggetto TickLabels. |
| [NumberFormat](../../aspose.cells.charts/ticklabels/numberformat/) { get; set; } | Rappresenta la stringa di formato per l'oggetto TickLabels. |
| [NumberFormatLinked](../../aspose.cells.charts/ticklabels/numberformatlinked/) { get; set; } | True se il formato numerico è collegato alle celle (in modo che il formato numerico cambi nelle etichette quando cambia nelle celle). |
| [Offset](../../aspose.cells.charts/ticklabels/offset/) { get; set; } | Ottiene e imposta la distanza delle etichette dall'asse delle categorie. Questo si applica solo all'asse delle categorie (x). |
| [ReadingOrder](../../aspose.cells.charts/ticklabels/readingorder/) { get; set; } | Rappresenta l'ordine di lettura del testo. |
| [RotationAngle](../../aspose.cells.charts/ticklabels/rotationangle/) { get; set; } | Rappresenta l'angolo di rotazione del testo in senso orario. |
| [TextDirection](../../aspose.cells.charts/ticklabels/textdirection/) { get; set; } | (**Obsolete.**) Rappresenta l'ordine di lettura del testo. |
| [TickLabelItems](../../aspose.cells.charts/ticklabels/ticklabelitems/) { get; } | Ottiene le etichette dei segni di visualizzazione dell'asse. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelsDemo
    {
        public static void TickLabelsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi NSeries (origine dati del grafico) al grafico che va dalla cella "A1" alla "B3"
            chart.NSeries.Add("A1:B3", true);

            // Accedi all'asse dei valori
            Axis valueAxis = chart.ValueAxis;

            // Accedi alle etichette dei segni dell'asse dei valori
            TickLabels tickLabels = valueAxis.TickLabels;

            // Imposta le proprietà delle etichette dei segni
            tickLabels.AutoScaleFont = true;
            tickLabels.BackgroundMode = BackgroundMode.Transparent;
            tickLabels.RotationAngle = 45;
            tickLabels.IsAutomaticRotation = false;
            tickLabels.NumberFormat = "0.00";
            tickLabels.Number = 2;
            tickLabels.NumberFormatLinked = true;
            tickLabels.Offset = 100;
            tickLabels.TextDirection = TextDirectionType.LeftToRight;
            tickLabels.ReadingOrder = TextDirectionType.LeftToRight;
            tickLabels.DirectionType = ChartTextDirectionType.Horizontal;
            tickLabels.AlignmentType = TickLabelAlignmentType.Center;

            // Salva la cartella di lavoro
            workbook.Save("TickLabelsExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


