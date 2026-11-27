---
title: "DocxSaveOptions.EmbedXlsxAsChartDataSource"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DocxSaveOptions-egenskap. Anger om en xlsx-fil ska bäddas in som datakälla för diagrammet"
type: docs
url: /sv/net/aspose.cells/docxsaveoptions/embedxlsxaschartdatasource/
---
## DocxSaveOptions.EmbedXlsxAsChartDataSource property

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
    using System;

    public class DocxSaveOptionsPropertyEmbedXlsxAsChartDataSourceDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet och lägg till exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Chart Data";

            try
            {
                // Initiera DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Visa standardvärdet för EmbedXlsxAsChartDataSource-egenskapen
                Console.WriteLine("Default EmbedXlsxAsChartDataSource value: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Sätt EmbedXlsxAsChartDataSource till true för att demonstrera dess användning
                saveOptions.EmbedXlsxAsChartDataSource = true;
                Console.WriteLine("EmbedXlsxAsChartDataSource set to: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Spara arbetsboken som DOCX med de konfigurerade alternativen
                workbook.Save("EmbedXlsxAsChartDataSourceDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with EmbedXlsxAsChartDataSource option.");
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

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


