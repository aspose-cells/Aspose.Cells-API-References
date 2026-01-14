---
title: DocxSaveOptions.EmbedXlsxAsChartDataSource
second_title: Aspose.Cells for .NET API Reference
description: DocxSaveOptions property. Indicates whether embedding an xlsx file as data source of the chart
type: docs
url: /net/aspose.cells/docxsaveoptions/embedxlsxaschartdatasource/
---
## DocxSaveOptions.EmbedXlsxAsChartDataSource property

Indicates whether embedding an xlsx file as data source of the chart.

```csharp
public bool EmbedXlsxAsChartDataSource { get; set; }
```

### Remarks

The default value is true.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyEmbedXlsxAsChartDataSourceDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet and add sample data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Chart Data";

            try
            {
                // Initialize DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Display the default value of EmbedXlsxAsChartDataSource property
                Console.WriteLine("Default EmbedXlsxAsChartDataSource value: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Set EmbedXlsxAsChartDataSource to true to demonstrate its usage
                saveOptions.EmbedXlsxAsChartDataSource = true;
                Console.WriteLine("EmbedXlsxAsChartDataSource set to: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Save the workbook as DOCX with the configured options
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

### See Also

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


