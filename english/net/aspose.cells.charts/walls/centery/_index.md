---
title: Walls.CenterY
second_title: Aspose.Cells for .NET API Reference
description: Walls property. Gets the y coordinate of the leftbottom corner of Wall center in units of 1/4000 of charts height after calls Chart.Calculate method
type: docs
url: /net/aspose.cells.charts/walls/centery/
---
## Walls.CenterY property

Gets the y coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's height after calls Chart.Calculate() method.

```csharp
public int CenterY { get; }
```

### Examples

```csharp
// Called: Console.WriteLine("CenterY: " + walls.CenterY);
public static void Walls_Property_CenterY()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Add a 3D chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculate the chart to update its properties
            chart.Calculate();

            // Access the walls of the 3D chart
            Walls walls = chart.Walls;

            // Set properties of the walls
            walls.BackgroundColor = Color.LightBlue;
            walls.ForegroundColor = Color.DarkBlue;
            walls.Formatting = FormattingType.Custom;
            walls.InvertIfNegative = true;
            walls.Transparency = 0.5;

            // Access the border of the walls and set its properties
            Line border = walls.Border;
            border.Color = Color.Red;
            border.Style = LineType.Solid;

            // Print some properties of the walls
            Console.WriteLine("CenterX: " + walls.CenterX);
            Console.WriteLine("CenterY: " + walls.CenterY);
            Console.WriteLine("Width: " + walls.Width);
            Console.WriteLine("Depth: " + walls.Depth);
            Console.WriteLine("Height: " + walls.Height);
            Console.WriteLine("CenterXPx: " + walls.CenterXPx);
            Console.WriteLine("CenterYPx: " + walls.CenterYPx);
            Console.WriteLine("WidthPx: " + walls.WidthPx);
            Console.WriteLine("DepthPx: " + walls.DepthPx);
            Console.WriteLine("HeightPx: " + walls.HeightPx);

            // Save the workbook
            workbook.Save("WallsExample.xlsx");
        }
```

### See Also

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


