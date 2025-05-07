---
title: SparklineGroup.PresetStyle
second_title: Aspose.Cells for .NET API Reference
description: SparklineGroup property. Gets and sets the preset style type of the sparkline group
type: docs
url: /net/aspose.cells.charts/sparklinegroup/presetstyle/
---
## SparklineGroup.PresetStyle property

Gets and sets the preset style type of the sparkline group.

```csharp
public SparklinePresetStyleType PresetStyle { get; set; }
```

### Examples

```csharp
// Called: group.PresetStyle = SparklinePresetStyleType.Style5;
public static void Property_PresetStyle()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for sparklines
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(3);
            worksheet.Cells["D1"].PutValue(4);
            worksheet.Cells["E1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(5);
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["C2"].PutValue(3);
            worksheet.Cells["D2"].PutValue(2);
            worksheet.Cells["E2"].PutValue(1);

            // Define the CellArea for the sparklines
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 1;
            ca.StartColumn = 5;
            ca.EndColumn = 5;

            // Add sparklines to the worksheet
            int idx = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:E2", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[idx];
            group.Sparklines.Add("A1:E1", 0, 5);
            group.Sparklines.Add("A2:E2", 1, 5);

            // Set the preset style type of the sparkline group
            group.PresetStyle = SparklinePresetStyleType.Style5;

            // Save the workbook
            workbook.Save("SparklinePresetStyleTypeExample.xlsx");

            return;
        }
```

### See Also

* enum [SparklinePresetStyleType](../../sparklinepresetstyletype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


