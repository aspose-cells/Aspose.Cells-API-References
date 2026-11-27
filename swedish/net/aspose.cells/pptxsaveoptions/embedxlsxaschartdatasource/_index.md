---
title: "PptxSaveOptions.EmbedXlsxAsChartDataSource"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PptxSaveOptions-egenskap. Anger om en xlsx-fil ska bäddas in som datakälla för diagrammet"
type: docs
url: /sv/net/aspose.cells/pptxsaveoptions/embedxlsxaschartdatasource/
---
## PptxSaveOptions.EmbedXlsxAsChartDataSource property

Anger om en xlsx‑fil ska bäddas in som datakälla för diagrammet.

```csharp
public bool EmbedXlsxAsChartDataSource { get; set; }
```

### Anmärkningar

Standardvärdet är sant.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PptxSaveOptionsPropertyEmbedXlsxAsChartDataSourceDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa ett exempelark med diagramdata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Lägg till ett diagram för att demonstrera egenskapens effekt
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Skapa en PptxSaveOptions‑instans
                PptxSaveOptions saveOptions = new PptxSaveOptions();

                // Visa standardvärdet för EmbedXlsxAsChartDataSource
                Console.WriteLine("Default EmbedXlsxAsChartDataSource value: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Ställ in egenskapen till true för att demonstrera dess användning
                saveOptions.EmbedXlsxAsChartDataSource = true;
                Console.WriteLine("EmbedXlsxAsChartDataSource set to: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Spara arbetsboken som PPTX med alternativet aktiverat
                workbook.Save("EmbedXlsxAsChartDataSourceDemo.pptx", saveOptions);

                Console.WriteLine("PPTX saved with EmbedXlsxAsChartDataSource enabled");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


