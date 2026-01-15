---
title: Enum SaveElementType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Saving.SaveElementType enum. Represents what kind of elements should be saved
type: docs
url: /net/aspose.cells.saving/saveelementtype/
---
## SaveElementType enumeration

Represents what kind of elements should be saved.

```csharp
public enum SaveElementType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| All | `251658239` | All data. |
| Chart | `256` | Only charts. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Saving;
    using System;

    public class SavingClassSaveElementTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add some sample data to demonstrate saving
                worksheet.Cells["A1"].PutValue("Sample Data");
                worksheet.Cells["B1"].PutValue(12345);

                // Create a chart to demonstrate Chart save element type
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B1", true);

                // Demonstrate using SaveElementType enum values
                SaveElementType chartType = SaveElementType.Chart;
                SaveElementType allType = SaveElementType.All;

                Console.WriteLine($"Chart SaveElementType value: {chartType}");
                Console.WriteLine($"All SaveElementType value: {allType}");

                // Save the workbook with all elements
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
                workbook.Save("SaveElementTypeDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved successfully with all elements");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SaveElementType: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


