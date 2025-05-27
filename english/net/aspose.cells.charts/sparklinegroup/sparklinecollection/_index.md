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
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertySparklineCollectionDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[5, i + 4].PutValue(i + 1);
            }

            // Create a sparkline group
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "E6:N6", false, CellArea.CreateCellArea(5, 4, 5, 13));

            // Get the sparkline group
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];

            // Add a sparkline to the collection
            group.Sparklines.Add("E6:N6", 5, 16);

            // Save the workbook
            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [SparklineCollection](../../sparklinecollection/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


