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
[Obsolete("Use SparklineCollection.RemoveSparkline(Sparkline) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Remove(object o)
```

| Parameter | Type | Description |
| --- | --- | --- |
| o | Object |  |

### Remarks

NOTE: This member is now obsolete. Instead, please use RemoveSparkline() method. This method will be removed 6 months later since December 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineCollectionMethodRemoveWithObjectDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Insert sample data into the worksheet
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);


            // Define the CellArea where the sparklines will be added
            CellArea cellArea = new CellArea { StartColumn = 4, EndColumn = 4, StartRow = 0, EndRow = 0 };

            // Add a new SparklineGroup to the worksheet
            int sparklineGroupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup sparklineGroup = worksheet.SparklineGroups[sparklineGroupIndex];

            SparklineCollection sparklineCollection = sparklineGroup.Sparklines;

            // Add sparklines to the SparklineGroup
            sparklineCollection.Add("A1:D1", 0, 5);

            Console.WriteLine("Sparkline count: " + sparklineCollection.Count);

            // Set various properties for the SparklineGroup
            sparklineGroup.ShowHighPoint = true;
            sparklineGroup.ShowLowPoint = true;

            // Set colors for high and low points
            CellsColor highPointColor = workbook.CreateCellsColor();
            highPointColor.Color = System.Drawing.Color.Green;
            sparklineGroup.HighPointColor = highPointColor;

            CellsColor lowPointColor = workbook.CreateCellsColor();
            lowPointColor.Color = System.Drawing.Color.Red;
            sparklineGroup.LowPointColor = lowPointColor;

            // Set the series color and line weight
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = System.Drawing.Color.Orange;
            sparklineGroup.SeriesColor = seriesColor;
            sparklineGroup.LineWeight = 1.0;


            // Get the first sparkline to remove
            Sparkline sparklineToRemove = sparklineCollection[0];

            // Call the Remove method with the sparkline object
            sparklineCollection.Remove(sparklineToRemove);

            Console.WriteLine("Sparkline removed successfully");


            Console.WriteLine("after deleted---Sparkline count: " + sparklineCollection.Count);
            // Save the workbook
            workbook.Save("SparklineRemoveDemo.xlsx");
        }
    }
}
```

### See Also

* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


