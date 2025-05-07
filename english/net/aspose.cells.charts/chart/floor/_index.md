---
title: Chart.Floor
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Returns a Floor object that represents the walls of a 3D chart
type: docs
url: /net/aspose.cells.charts/chart/floor/
---
## Chart.Floor property

Returns a `Floor` object that represents the walls of a 3-D chart.

```csharp
public Floor Floor { get; }
```

### Remarks

This property doesn't apply to 3-D pie charts.

### Examples

```csharp
// Called: Floor floor = chart.Floor;
public static void Property_Floor()
        {
            // Instantiate the workbook object
            Workbook workbook = new Workbook();

            // Get cells collection
            Cells cells = workbook.Worksheets[0].Cells;

            // Put values in cells
            cells["A1"].PutValue(1);
            cells["A2"].PutValue(2);
            cells["A3"].PutValue(3);

            // Get charts collection
            ChartCollection charts = workbook.Worksheets[0].Charts;

            // Add a new chart
            int index = charts.Add(ChartType.Column3DStacked, 5, 0, 15, 5);

            // Get the newly added chart
            Chart chart = charts[index];

            // Set chart's nseries
            chart.NSeries.Add("A1:A3", true);

            // Show data labels
            chart.NSeries[0].DataLabels.ShowValue = true;

            // Get chart's floor
            Floor floor = chart.Floor;

            // Set floor's border as red
            floor.Border.Color = Color.Red;

            // Set fill format
            floor.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.DiagonalDown, 2);

            // Set additional properties
            floor.BackgroundColor = Color.LightBlue;
            floor.ForegroundColor = Color.DarkBlue;
            floor.Formatting = FormattingType.Custom;
            floor.InvertIfNegative = true;
            floor.Transparency = 0.5;

            // Save the file
            workbook.Save(@"FloorExample.xlsx");
            workbook.Save(@"FloorExample.pdf");
        }
```

### See Also

* class [Floor](../../floor/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


