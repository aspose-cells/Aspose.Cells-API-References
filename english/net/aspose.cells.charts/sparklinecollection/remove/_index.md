---
title: SparklineCollection.Remove
second_title: Aspose.Cells for .NET API Reference
description: SparklineCollection method. Removes the sparkline
type: docs
url: /net/aspose.cells.charts/sparklinecollection/remove/
---
## SparklineCollection.Remove method

Removes the sparkline

```csharp
public void Remove(object o)
```

| Parameter | Type | Description |
| --- | --- | --- |
| o | Object |  |

### Examples

```csharp
namespace AsposeCellsExamples.SparklineCollectionMethodRemoveWithObjectDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineCollectionMethodRemoveWithObjectDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Create some sample data for sparklines
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;
            
            // Create sparkline group through the worksheet's SparklineGroups property
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];
            
            // Add sparklines to the collection
            SparklineCollection sparklines = group.SparklineCollection;
            int index1 = sparklines.Add("A1:A3", 0, 0);
            int index2 = sparklines.Add("A1:A3", 0, 1);
            
            try
            {
                // Get the first sparkline to remove
                Sparkline sparklineToRemove = sparklines[0];
                
                // Call the Remove method with the sparkline object
                sparklines.Remove(sparklineToRemove);
                
                Console.WriteLine("Sparkline removed successfully");
                
                // Save the workbook
                workbook.Save("SparklineRemoveDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error removing sparkline: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


