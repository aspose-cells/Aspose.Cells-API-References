---
title: SparklineGroup.LineWeight
second_title: Aspose.Cells for .NET API Reference
description: SparklineGroup property. Gets and sets the line weight in each line sparkline in the sparkline group in the unit of points
type: docs
url: /net/aspose.cells.charts/sparklinegroup/lineweight/
---
## SparklineGroup.LineWeight property

Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points.

```csharp
public double LineWeight { get; set; }
```

### Examples

```csharp
// Called: group.LineWeight = 1.0;
public static void SparklineGroup_Property_LineWeight()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Define the CellArea for the sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Add a sparkline group to the worksheet
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Add sparklines to the group
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Customize the sparkline group
            group.ShowHighPoint = true;
            group.ShowLowPoint = true;
            group.HighPointColor.Color = Color.Green;
            group.LowPointColor.Color = Color.Red;
            group.LineWeight = 1.0;

            // Save the workbook
            workbook.Save("SparklineGroupCollectionExample.xlsx", SaveFormat.Xlsx);
        }
```

### See Also

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


