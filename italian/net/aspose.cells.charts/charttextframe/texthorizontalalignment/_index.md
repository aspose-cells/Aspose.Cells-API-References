---
title: "ChartTextFrame.TextHorizontalAlignment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartTextFrame. Ottiene e imposta l'allineamento orizzontale del testo"
type: docs
url: /it/net/aspose.cells.charts/charttextframe/texthorizontalalignment/
---
## ChartTextFrame.TextHorizontalAlignment property

Ottiene e imposta l'allineamento orizzontale del testo.

```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico e imposta il suo intervallo di dati
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni il titolo del grafico e imposta le proprietà
            Title title = chart.Title;
            title.Text = "Sample Chart Title";
            
            // Dimostra la proprietà TextHorizontalAlignment
            title.TextHorizontalAlignment = TextAlignmentType.Center;
            Console.WriteLine("Title horizontal alignment set to: " + title.TextHorizontalAlignment);

            // Salva la cartella di lavoro
            workbook.Save("ChartTextHorizontalAlignmentDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


