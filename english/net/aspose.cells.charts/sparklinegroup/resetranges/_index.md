---
title: SparklineGroup.ResetRanges
second_title: Aspose.Cells for .NET API Reference
description: SparklineGroup method. Resets the data range and location range of the sparkline group. This method will clear original sparkline items in the group and creates new sparkline items for the new ranges
type: docs
url: /net/aspose.cells.charts/sparklinegroup/resetranges/
---
## SparklineGroup.ResetRanges method

Resets the data range and location range of the sparkline group. This method will clear original sparkline items in the group and creates new sparkline items for the new ranges.

```csharp
public void ResetRanges(string dataRange, bool isVertical, CellArea locationRange)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataRange | String | Specifies the new data range of the sparkline group. |
| isVertical | Boolean | Specifies whether to plot the sparklines from the new data range by row or by column. |
| locationRange | CellArea | Specifies where the sparklines to be placed. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupMethodResetRangesWithStringBooleanCellAreaDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for sparklines
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(3);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["A4"].PutValue(2);
            worksheet.Cells["A5"].PutValue(9);

            // Create a sparkline group
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];

            // Prepare parameters for ResetRanges
            string dataRange = "A1:A5";
            bool isVertical = true;
            CellArea locationRange = CellArea.CreateCellArea(0, 1, 4, 1); // B1:B5

            try
            {
                // Call ResetRanges with parameters (String, Boolean, CellArea)
                group.ResetRanges(dataRange, isVertical, locationRange);

                Console.WriteLine("ResetRanges method executed successfully with parameters (String, Boolean, CellArea)");
                
                // Add sparklines to visualize the effect
                for (int i = 0; i < 5; i++)
                {
                    worksheet.Cells[0 + i, 1].PutValue("Sparkline");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ResetRanges method: {ex.Message}");
            }

            // Save the result
            workbook.Save("SparklineGroupResetRangesDemo.xlsx");
        }
    }
}
```

### See Also

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


