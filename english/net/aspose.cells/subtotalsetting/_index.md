---
title: Class SubtotalSetting
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.SubtotalSetting class. Represents the setting of the subtotal 
type: docs
url: /net/aspose.cells/subtotalsetting/
---
## SubtotalSetting class

Represents the setting of the subtotal .

```csharp
public class SubtotalSetting
```

## Properties

| Name | Description |
| --- | --- |
| [GroupBy](../../aspose.cells/subtotalsetting/groupby/) { get; } | The field to group by, as a zero-based integer offset |
| [SubtotalFunction](../../aspose.cells/subtotalsetting/subtotalfunction/) { get; } | The subtotal function. |
| [SummaryBelowData](../../aspose.cells/subtotalsetting/summarybelowdata/) { get; } | Indicates whether add summary below data. |
| [TotalList](../../aspose.cells/subtotalsetting/totallist/) { get; } | An array of zero-based field offsets, indicating the fields to which the subtotals are added. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassSubtotalSettingDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add sample data to the worksheet
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["A2"].PutValue("Group A");
                worksheet.Cells["A3"].PutValue("Group B");
                worksheet.Cells["A4"].PutValue("Group A");
                worksheet.Cells["A5"].PutValue("Group B");
                worksheet.Cells["B2"].PutValue(100);
                worksheet.Cells["B3"].PutValue(200);
                worksheet.Cells["B4"].PutValue(300);
                worksheet.Cells["B5"].PutValue(400);

                // Define the cell area for subtotals
                CellArea area = CellArea.CreateCellArea("A1", "B5");

                // Apply subtotals to the data
                worksheet.Cells.Subtotal(
                    area,
                    0, // Group by first column (Category)
                    ConsolidationFunction.Sum,
                    new int[] { 1 }, // Subtotal on second column (Value)
                    true,
                    true,
                    true);

                // Retrieve the SubtotalSetting from the worksheet
                SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);

                // Display the properties of the SubtotalSetting
                Console.WriteLine("Subtotal Setting Properties:");
                Console.WriteLine($"GroupBy field index: {subtotalSetting.GroupBy}");
                Console.WriteLine($"Subtotal Function: {subtotalSetting.SubtotalFunction}");
                Console.WriteLine($"TotalList contains column index: {subtotalSetting.TotalList[0]}");
                Console.WriteLine($"Summary Below Data: {subtotalSetting.SummaryBelowData}");

                // Save the workbook
                workbook.Save("SubtotalSettingDemo.xlsx");
                Console.WriteLine("SubtotalSetting demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SubtotalSetting: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


