---
title: "Series.HasDropLines"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. True se il grafico ha linee di discesa. Si applica solo a grafici a linee o a grafici ad area"
type: docs
url: /it/net/aspose.cells.charts/series/hasdroplines/
---
## Series.HasDropLines property

Vero se il grafico ha linee di discesa. Si applica solo ai grafici a linee o a aree.

```csharp
public bool HasDropLines { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasDropLinesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
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

            // Aggiungi un grafico a linee
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi dati della serie
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni la prima serie
            Series series = chart.NSeries[0];

            // Dimostrare la proprietà HasDropLines
            series.HasDropLines = true; // Enable drop lines
            series.Type = ChartType.Line; // Ensure it's a line chart for drop lines to be visible

            // Salva la cartella di lavoro
            workbook.Save("SeriesHasDropLinesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


