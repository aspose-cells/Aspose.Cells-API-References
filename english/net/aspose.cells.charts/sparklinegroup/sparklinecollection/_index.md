---
title: SparklineGroup.SparklineCollection
second_title: Aspose.Cells for .NET API Reference
description: SparklineGroup property. Gets the collection of Sparkline object
type: docs
url: /net/aspose.cells.charts/sparklinegroup/sparklinecollection/
---
## SparklineGroup.SparklineCollection property

Gets the collection of [`Sparkline`](../../sparkline/) object.

```csharp
[Obsolete("Use SparklineGroup.Sparklines property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SparklineCollection SparklineCollection { get; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use SparklineGroup.Sparklines property. This property will be removed 12 months later since November 2022. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupPropertySparklineCollectionDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for sparklines
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);
            worksheet.Cells["C1"].PutValue(15);
            worksheet.Cells["D1"].PutValue(30);

            try
            {
                // Define location for sparklines
                CellArea location = new CellArea
                {
                    StartRow = 0,
                    EndRow = 0,
                    StartColumn = 4,
                    EndColumn = 4
                };

                // Add a sparkline group to the worksheet
                int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, location);
                SparklineGroup sparklineGroup = worksheet.SparklineGroups[groupIndex];

                // Add a sparkline to the group
                sparklineGroup.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

                // Access the SparklineCollection property (read-only)
                SparklineCollection sparklineCollection = sparklineGroup.SparklineCollection;

                // Display information about the sparkline collection
                Console.WriteLine($"SparklineCollection contains {sparklineCollection.Count} sparklines");

                // Iterate through the sparklines in the collection
                for (int i = 0; i < sparklineCollection.Count; i++)
                {
                    Sparkline sparkline = sparklineCollection[i];
                    Console.WriteLine($"Sparkline {i + 1} location: Row {sparkline.Row}, Column {sparkline.Column}");
                }

                // Save the workbook
                workbook.Save("SparklineCollectionDemo.xlsx");
                Console.WriteLine("SparklineCollection demonstration completed successfully.");
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

* class [SparklineCollection](../../sparklinecollection/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


