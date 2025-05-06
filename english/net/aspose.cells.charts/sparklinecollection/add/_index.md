---
title: SparklineCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: SparklineCollection method. Add a sparkline
type: docs
url: /net/aspose.cells.charts/sparklinecollection/add/
---
## SparklineCollection.Add method

Add a sparkline.

```csharp
public int Add(string dataRange, int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataRange | String | Specifies the new data range of the sparkline. |
| row | Int32 | The row index of the location. |
| column | Int32 | The column index of the location. |

### Examples

```csharp
// Called: group.Sparklines.Add(&amp;quot;A1:E1&amp;quot;, 0, 5);
public static void Method_Int32_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for sparklines
            worksheet.Cells[&quot;A1&quot;].PutValue(1);
            worksheet.Cells[&quot;B1&quot;].PutValue(2);
            worksheet.Cells[&quot;C1&quot;].PutValue(3);
            worksheet.Cells[&quot;D1&quot;].PutValue(4);
            worksheet.Cells[&quot;E1&quot;].PutValue(5);
            worksheet.Cells[&quot;A2&quot;].PutValue(5);
            worksheet.Cells[&quot;B2&quot;].PutValue(4);
            worksheet.Cells[&quot;C2&quot;].PutValue(3);
            worksheet.Cells[&quot;D2&quot;].PutValue(2);
            worksheet.Cells[&quot;E2&quot;].PutValue(1);

            // Define the CellArea for the sparklines
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 1;
            ca.StartColumn = 5;
            ca.EndColumn = 5;

            // Add sparklines to the worksheet
            int idx = worksheet.SparklineGroups.Add(SparklineType.Line, &quot;A1:E2&quot;, false, ca);
            SparklineGroup group = worksheet.SparklineGroups[idx];
            group.Sparklines.Add(&quot;A1:E1&quot;, 0, 5);
            group.Sparklines.Add(&quot;A2:E2&quot;, 1, 5);

            // Set the preset style type of the sparkline group
            group.PresetStyle = SparklinePresetStyleType.Style5;

            // Save the workbook
            workbook.Save(&quot;SparklinePresetStyleTypeExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


