---
title: "SaveOptions.RefreshChartCache"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SaveOptions-egenskap. Anger om den senaste diagramdata ska cachas"
type: docs
url: /sv/net/aspose.cells/saveoptions/refreshchartcache/
---
## SaveOptions.RefreshChartCache property

Anger om den senaste diagramdata ska cachas.

```csharp
public bool RefreshChartCache { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyRefreshChartCacheDemo
    {
        public static void Run()
        {
            // Skapa ett exempelarbetsbok med ett diagram
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Skapa PDF-sparalternativ med RefreshChartCache aktiverat
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.RefreshChartCache = true;

            // Spara arbetsboken med alternativet för att uppdatera diagramcachen
            workbook.Save("output.pdf", pdfSaveOptions);

            Console.WriteLine("Workbook saved with chart cache refreshed.");
        }
    }
}
```

### Se även

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


