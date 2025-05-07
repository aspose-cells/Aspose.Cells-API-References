---
title: SparklineGroup.ShowHighPoint
second_title: Aspose.Cells for .NET API Reference
description: SparklineGroup property. Indicates whether to highlight the highest points of data in the sparkline group
type: docs
url: /net/aspose.cells.charts/sparklinegroup/showhighpoint/
---
## SparklineGroup.ShowHighPoint property

Indicates whether to highlight the highest points of data in the sparkline group.

```csharp
public bool ShowHighPoint { get; set; }
```

### Examples

```csharp
// Called: group.ShowHighPoint = true;
public static void Property_ShowHighPoint()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Define the CellArea for the sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Add a sparkline group to the worksheet
            int idx = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[idx];

            // Add sparklines to the group
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Customize the sparkline group
            CellsColor clr = workbook.CreateCellsColor();
            clr.Color = Color.Orange;
            group.SeriesColor = clr;

            // Set the high points to be colored green and the low points to be colored red
            group.ShowHighPoint = true;
            group.ShowLowPoint = true;
            group.HighPointColor.Color = Color.Green;
            group.LowPointColor.Color = Color.Red;

            // Set line weight
            group.LineWeight = 1.0;

            // Save the workbook
            workbook.Save("SparklineTypeExample.xlsx", SaveFormat.Xlsx);
        }
```

### See Also

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


