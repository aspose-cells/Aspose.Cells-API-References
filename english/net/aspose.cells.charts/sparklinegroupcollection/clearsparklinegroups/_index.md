---
title: SparklineGroupCollection.ClearSparklineGroups
second_title: Aspose.Cells for .NET API Reference
description: SparklineGroupCollection method. Clears the sparkline groups that overlaps an area of cells
type: docs
url: /net/aspose.cells.charts/sparklinegroupcollection/clearsparklinegroups/
---
## SparklineGroupCollection.ClearSparklineGroups method

Clears the sparkline groups that overlaps an area of cells.

```csharp
public void ClearSparklineGroups(CellArea cellArea)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | Specifies the area of cells |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupCollectionMethodClearSparklineGroupsWithCellAreaDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sparklines to the worksheet
            SparklineGroupCollection sparklineGroups = worksheet.SparklineGroups;
            int groupIndex = sparklineGroups.Add(SparklineType.Line, "A1:A5", false, CellArea.CreateCellArea(0, 0, 4, 0));
            
            // Create cell area to clear sparkline groups
            CellArea cellArea = CellArea.CreateCellArea(0, 0, 4, 0);

            try
            {
                // Call the ClearSparklineGroups method with CellArea parameter
                sparklineGroups.ClearSparklineGroups(cellArea);
                
                Console.WriteLine("Sparkline groups cleared successfully for the specified cell area.");
                
                // Verify the sparkline groups count after clearing
                Console.WriteLine($"Remaining sparkline groups count: {sparklineGroups.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearSparklineGroups method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("ClearSparklineGroupsWithCellAreaDemo.xlsx");
        }
    }
}
```

### See Also

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


