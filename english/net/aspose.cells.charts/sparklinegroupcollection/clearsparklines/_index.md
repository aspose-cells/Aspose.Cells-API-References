---
title: SparklineGroupCollection.ClearSparklines
second_title: Aspose.Cells for .NET API Reference
description: SparklineGroupCollection method. Clears the sparklines that is inside an area of cells
type: docs
url: /net/aspose.cells.charts/sparklinegroupcollection/clearsparklines/
---
## SparklineGroupCollection.ClearSparklines method

Clears the sparklines that is inside an area of cells.

```csharp
public void ClearSparklines(CellArea cellArea)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | Specifies the area of cells |

### Examples

```csharp
namespace AsposeCellsExamples.SparklineGroupCollectionMethodClearSparklinesWithCellAreaDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupCollectionMethodClearSparklinesWithCellAreaDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for sparklines
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(3);
            worksheet.Cells["A3"].PutValue(6);
            worksheet.Cells["A4"].PutValue(4);
            worksheet.Cells["A5"].PutValue(7);

            // Create a sparkline group
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:A5", false, CellArea.CreateCellArea(0, 1, 4, 1));

            // Create CellArea parameter for ClearSparklines method
            CellArea cellArea = CellArea.CreateCellArea(0, 1, 4, 1);

            try
            {
                // Call ClearSparklines method with CellArea parameter
                worksheet.SparklineGroups.ClearSparklines(cellArea);
                
                Console.WriteLine("Sparklines cleared successfully from the specified area.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearSparklines method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("SparklineGroupCollectionMethodClearSparklinesWithCellAreaDemo.xlsx");
        }
    }
}
```

### See Also

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


