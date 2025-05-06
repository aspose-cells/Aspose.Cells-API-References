---
title: SparklineGroup.ShowLowPoint
second_title: Aspose.Cells for .NET API Reference
description: SparklineGroup property. Indicates whether to highlight the lowest points of data in the sparkline group
type: docs
url: /net/aspose.cells.charts/sparklinegroup/showlowpoint/
---
## SparklineGroup.ShowLowPoint property

Indicates whether to highlight the lowest points of data in the sparkline group.

```csharp
public bool ShowLowPoint { get; set; }
```

### Examples

```csharp
// Called: group.ShowLowPoint = true;
public static void Property_ShowLowPoint()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            sheet.Cells[&quot;A1&quot;].PutValue(5);
            sheet.Cells[&quot;B1&quot;].PutValue(2);
            sheet.Cells[&quot;C1&quot;].PutValue(1);
            sheet.Cells[&quot;D1&quot;].PutValue(3);

            // Define the CellArea for the sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Add a sparkline group to the worksheet
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, &quot;A1:D1&quot;, false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Add sparklines to the group
            group.Sparklines.Add(sheet.Name + &quot;!A1:D1&quot;, 0, 4);

            // Customize the sparkline group
            group.ShowHighPoint = true;
            group.ShowLowPoint = true;
            group.HighPointColor.Color = Color.Green;
            group.LowPointColor.Color = Color.Red;
            group.LineWeight = 1.0;

            // Save the workbook
            workbook.Save(&quot;SparklineGroupCollectionExample.xlsx&quot;, SaveFormat.Xlsx);
        }
```

### See Also

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


