---
title: "Classe LegendEntry"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Charts.LegendEntry. Rappresenta una voce di legenda in una legenda del grafico"
type: docs
url: /it/net/aspose.cells.charts/legendentry/
---
## LegendEntry class

Rappresenta una voce della legenda in una legenda del grafico.

```csharp
public class LegendEntry
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutoScaleFont](../../aspose.cells.charts/legendentry/autoscalefont/) { get; set; } | True se il testo nell'oggetto cambia dimensione del carattere quando le dimensioni dell'oggetto cambiano. Il valore predefinito è True. |
| [Background](../../aspose.cells.charts/legendentry/background/) { get; set; } | (**Obsolete.**) Ottiene e imposta la modalità di visualizzazione dello sfondo |
| [BackgroundMode](../../aspose.cells.charts/legendentry/backgroundmode/) { get; set; } | Ottiene e imposta la modalità di visualizzazione dello sfondo |
| [Font](../../aspose.cells.charts/legendentry/font/) { get; } | Ottiene un oggetto [`Font`](./font/) del specificato oggetto ChartFrame. |
| [IsDeleted](../../aspose.cells.charts/legendentry/isdeleted/) { get; set; } | Ottiene e imposta se la voce di legenda è eliminata. |
| [IsTextNoFill](../../aspose.cells.charts/legendentry/istextnofill/) { get; set; } | Ottiene o imposta nessun riempimento del testo. |
| virtual [TextFont](../../aspose.cells.charts/legendentry/textfont/) { get; } | (**Obsolete.**) Ottiene un oggetto [`Font`](./font/) dell'oggetto LegendEntry specificato. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendEntryDemo
    {
        public static void LegendEntryExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio al foglio di lavoro
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

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi NSeries (origine dati del grafico) al grafico che va dalla cella "A1" alla "B4"
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Accedi alla voce della legenda della prima serie
            LegendEntry legendEntry = chart.NSeries[0].LegendEntry;

            // Imposta le proprietà della voce della legenda
            legendEntry.IsDeleted = false;
            legendEntry.IsTextNoFill = false;
            legendEntry.AutoScaleFont = true;
            legendEntry.Background = BackgroundMode.Transparent;
            legendEntry.BackgroundMode = BackgroundMode.Opaque;

            // Accedi e modifica il font della voce della legenda
            Font font = legendEntry.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            font.Color = System.Drawing.Color.Blue;

            // Salva la cartella di lavoro
            workbook.Save("LegendEntryExample.xlsx");
            workbook.Save("LegendEntryExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


