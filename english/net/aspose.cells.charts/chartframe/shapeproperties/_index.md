---
title: ChartFrame.ShapeProperties
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Gets the ShapeProperties object
type: docs
url: /net/aspose.cells.charts/chartframe/shapeproperties/
---
## ChartFrame.ShapeProperties property

Gets the `ShapeProperties` object.

```csharp
public ShapePropertyCollection ShapeProperties { get; }
```

### Examples

```csharp
// Called: ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;
public static void ChartFrame_Property_ShapeProperties()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Set the chart data range
            chart.SetChartDataRange("A1:B4", true);

            // Access the chart's title and set its text
            chart.Title.Text = "Sample Chart with Bevel";

            // Access the chart's plot area
            PlotArea plotArea = chart.PlotArea;

            // Access the shape properties of the plot area
            ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;

            
            // Access the 3D format properties
            Format3D format3D = shapeProperties.Format3D;

            // Access the top bevel properties
            Bevel topBevel = format3D.TopBevel;

            // Set the bevel type to "Angle"
            topBevel.Type = BevelPresetType.Angle;

            // Set the width and height of the bevel
            topBevel.Width = 10;
            topBevel.Height = 10;

            // Save the workbook
            workbook.Save("BevelPresetTypeExample.xlsx");
            workbook.Save("BevelPresetTypeExample.pdf");
        }
```

### See Also

* class [ShapePropertyCollection](../../../aspose.cells.drawing/shapepropertycollection/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


