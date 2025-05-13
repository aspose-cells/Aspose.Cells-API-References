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
public void ShapeCollection_Method_AddTextBoxInChart()
{
    Workbook workbook = new Workbook();
    Worksheet worksheet = workbook.Worksheets[0];

    int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
    Chart waterfallChart = worksheet.Charts[chartIndex];

    Cells cells = worksheet.Cells;

    cells["A1"].PutValue("Categories");
    cells["A2"].PutValue("Start");
    cells["A3"].PutValue("Positive Value 1");
    cells["A4"].PutValue("Negative Value 1");
    cells["A5"].PutValue("Positive Value 2");
    cells["A6"].PutValue("End");
    waterfallChart.NSeries.CategoryData = ("A2:A6");

    cells["B1"].PutValue("Values");
    cells["B2"].PutValue(0);
    cells["B3"].PutValue(20);
    cells["B4"].PutValue(-10);
    cells["B5"].PutValue(15);
    cells["B6"].PutValue(25);
    waterfallChart.NSeries.Add("B2:B6", true);

    /*Shape sh = waterfallChart.getShapes().addTextBox(5, 0, 0, 5, 100, 100);
    sh.setText("adding some TextBOX");*/

    Shape sh1 = waterfallChart.Shapes.AddTextBoxInChart(0, 10, 2000, 2000);
    sh1.Text = ("filter:color Value");
    Aspose.Cells.Font filterLabelFont = sh1.Characters(7, 18).Font; // duplicating words 
    filterLabelFont.Color = Color.Red;
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Chart chart = workbook.Worksheets[0].Charts[0];
    Assert.AreEqual("filter:color Value", chart.Shapes[0].Text);
}
```

### See Also

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


