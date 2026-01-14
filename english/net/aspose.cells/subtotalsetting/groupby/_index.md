---
title: SubtotalSetting.GroupBy
second_title: Aspose.Cells for .NET API Reference
description: SubtotalSetting property. The field to group by as a zerobased integer offset
type: docs
url: /net/aspose.cells/subtotalsetting/groupby/
---
## SubtotalSetting.GroupBy property

The field to group by, as a zero-based integer offset

```csharp
public int GroupBy { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SubtotalSettingPropertyGroupByDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
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

            try
            {
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

                // Retrieve the subtotal setting to access the GroupBy property
                SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);

                // Display the GroupBy property value
                Console.WriteLine("GroupBy field index: " + subtotalSetting.GroupBy);

                // Save the workbook
                workbook.Save("GroupByDemo.xlsx");
                Console.WriteLine("Subtotal with GroupBy demonstrated successfully.");
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

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


