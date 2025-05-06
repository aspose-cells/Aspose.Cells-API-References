---
title: ChartTextFrame.RotationAngle
second_title: Aspose.Cells for .NET API Reference
description: ChartTextFrame property. Represents text rotation angle
type: docs
url: /net/aspose.cells.charts/charttextframe/rotationangle/
---
## ChartTextFrame.RotationAngle property

Represents text rotation angle.

```csharp
public int RotationAngle { get; set; }
```

### Remarks

0: Not rotated.255: Top to Bottom.-90: Downward.90: Upward.

### Examples

```csharp
// Called: chart.ValueAxis.Title.RotationAngle = 90;
[Test]
        public void Property_RotationAngle()
        {
            Workbook workbook = new Workbook();

            workbook.ChangePalette(Color.Orange, 53);

            workbook.ChangePalette(Color.LightBlue, 54);

            workbook.ChangePalette(Color.LightCoral, 55);

            Color[] colors = workbook.Colors;

            //Set default font

            Style style = workbook.DefaultStyle;

            style.Font.Name = &quot;Tahoma&quot;;

            workbook.DefaultStyle = style;

            Cells cells = workbook.Worksheets[0].Cells;

            //Put a string into a cell

            cells[&quot;A1&quot;].PutValue(&quot;Region&quot;);

            cells[&quot;A2&quot;].PutValue(&quot;France&quot;);

            cells[&quot;A3&quot;].PutValue(&quot;Germany&quot;);

            cells[&quot;A4&quot;].PutValue(&quot;England&quot;);

            cells[&quot;B1&quot;].PutValue(&quot;Marketing Costs&quot;);

            cells[&quot;B2&quot;].PutValue(70000);

            cells[&quot;B3&quot;].PutValue(55000);

            cells[&quot;B4&quot;].PutValue(30000);

            Worksheet sheet = workbook.Worksheets[0];

            //Set the name of the worksheet

            sheet.Name = &quot;Clustered Column&quot;;

            sheet.IsGridlinesVisible = false;

            //Create chart

            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 1, 29, 10);

            Chart chart = sheet.Charts[chartIndex];

            //Add the nseries collection to a chart 

            chart.NSeries.Add(&quot;B2:B4&quot;, true);

            //Get or set the range of category axis values

            chart.NSeries.CategoryData = &quot;A2:A4&quot;;

            //this works also fine.

            //chart.NSeries.CategoryData = &quot;{\&quot;Fra\&quot;,\&quot;Ger\&quot;,\&quot;Eng\&quot;}&quot;;

            chart.NSeries.IsColorVaried = true;



            for (int i = 0; i &lt; chart.NSeries[0].Points.Count; i++)
            {

                chart.NSeries[0].Points[i].Area.ForegroundColor = colors[53 + i];

            }


            //Set properties of chart title

            chart.Title.Text = &quot;Marketing Costs by Region&quot;;

            chart.Title.Font.IsBold = true;

            chart.Title.Font.Color = Color.Black;

            chart.Title.Font.Size = 12;

            //Set properties of categoryaxis title

            chart.CategoryAxis.Title.Text = &quot;Region&quot;;

            chart.CategoryAxis.Title.Font.Color = Color.Black;

            chart.CategoryAxis.TickLabels.AutoScaleFont = true;

            chart.CategoryAxis.TickLabels.RotationAngle = 45;

            chart.CategoryAxis.TickLabels.Font.Size = 10;

            chart.CategoryAxis.Title.Font.IsBold = true;

            chart.CategoryAxis.Title.Font.Size = 10;

            //Set properties of valueaxis title

            chart.ValueAxis.Title.Text = &quot;In Thousands&quot;;

            chart.ValueAxis.Title.Font.Name = &quot;Arial&quot;;

            chart.ValueAxis.Title.Font.Color = Color.Black;

            chart.ValueAxis.Title.Font.IsBold = true;

            chart.ValueAxis.Title.Font.Size = 10;

            chart.ValueAxis.Title.RotationAngle = 90;

            chart.ValueAxis.MajorUnit = double.Parse(&quot;20000&quot;);

            chart.ValueAxis.MaxValue = double.Parse(&quot;80000&quot;);

            chart.ValueAxis.MinorUnit = double.Parse(&quot;5000&quot;);

            chart.ValueAxis.MinValue = double.Parse(&quot;0&quot;);

            workbook.Save(Constants.destPath + &quot;Test_174463.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;Test_174463.xlsx&quot;);
            chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(chart.CategoryAxis.TickLabels.RotationAngle, 45, 0.01);
        }
```

### See Also

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


