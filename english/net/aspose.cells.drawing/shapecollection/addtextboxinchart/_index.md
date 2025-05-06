---
title: ShapeCollection.AddTextBoxInChart
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a textbox to the chart
type: docs
url: /net/aspose.cells.drawing/shapecollection/addtextboxinchart/
---
## ShapeCollection.AddTextBoxInChart method

Adds a textbox to the chart.

```csharp
public TextBox AddTextBoxInChart(int top, int left, int height, int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| top | Int32 | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| left | Int32 | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| height | Int32 | Represents the height of textbox, in units of 1/4000 of the chart area. |
| width | Int32 | Represents the width of textbox, in units of 1/4000 of the chart area. |

### Return Value

A TextBox object.

### Examples

```csharp
// Called: Shape sh1 = waterfallChart.Shapes.AddTextBoxInChart(0, 10, 2000, 2000);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart waterfallChart = worksheet.Charts[chartIndex];

            Cells cells = worksheet.Cells;

            cells[&quot;A1&quot;].PutValue(&quot;Categories&quot;);
            cells[&quot;A2&quot;].PutValue(&quot;Start&quot;);
            cells[&quot;A3&quot;].PutValue(&quot;Positive Value 1&quot;);
            cells[&quot;A4&quot;].PutValue(&quot;Negative Value 1&quot;);
            cells[&quot;A5&quot;].PutValue(&quot;Positive Value 2&quot;);
            cells[&quot;A6&quot;].PutValue(&quot;End&quot;);
            waterfallChart.NSeries.CategoryData = (&quot;A2:A6&quot;);

            cells[&quot;B1&quot;].PutValue(&quot;Values&quot;);
            cells[&quot;B2&quot;].PutValue(0);
            cells[&quot;B3&quot;].PutValue(20);
            cells[&quot;B4&quot;].PutValue(-10);
            cells[&quot;B5&quot;].PutValue(15);
            cells[&quot;B6&quot;].PutValue(25);
            waterfallChart.NSeries.Add(&quot;B2:B6&quot;, true);

            /*Shape sh = waterfallChart.getShapes().addTextBox(5, 0, 0, 5, 100, 100);
            sh.setText(&quot;adding some TextBOX&quot;);*/

            Shape sh1 = waterfallChart.Shapes.AddTextBoxInChart(0, 10, 2000, 2000);
            sh1.Text = (&quot;filter:color Value&quot;);
            Aspose.Cells.Font filterLabelFont = sh1.Characters(7, 18).Font; // duplicating words 
            filterLabelFont.Color = Color.Red;
            workbook.Save(Constants.destPath + &quot;CellsJava46058.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsJava46058.xlsx&quot;);
            Chart chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(&quot;filter:color Value&quot;, chart.Shapes[0].Text);
        }
```

### See Also

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


