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
// Called: Console.WriteLine(&amp;quot;CenterY: &amp;quot; + walls.CenterY);
public static void Property_CenterY()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the chart
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Category&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;A&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;B&quot;);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;C&quot;);
            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Value&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(10);
            worksheet.Cells[&quot;B3&quot;].PutValue(20);
            worksheet.Cells[&quot;B4&quot;].PutValue(30);

            // Add a 3D chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add(&quot;B2:B4&quot;, true);
            chart.NSeries.CategoryData = &quot;A2:A4&quot;;

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
            Console.WriteLine(&quot;CenterX: &quot; + walls.CenterX);
            Console.WriteLine(&quot;CenterY: &quot; + walls.CenterY);
            Console.WriteLine(&quot;Width: &quot; + walls.Width);
            Console.WriteLine(&quot;Depth: &quot; + walls.Depth);
            Console.WriteLine(&quot;Height: &quot; + walls.Height);
            Console.WriteLine(&quot;CenterXPx: &quot; + walls.CenterXPx);
            Console.WriteLine(&quot;CenterYPx: &quot; + walls.CenterYPx);
            Console.WriteLine(&quot;WidthPx: &quot; + walls.WidthPx);
            Console.WriteLine(&quot;DepthPx: &quot; + walls.DepthPx);
            Console.WriteLine(&quot;HeightPx: &quot; + walls.HeightPx);

            // Save the workbook
            workbook.Save(&quot;WallsExample.xlsx&quot;);
        }
```

### See Also

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


