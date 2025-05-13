---
title: TickLabels.AutoScaleFont
second_title: Aspose.Cells for .NET API Reference
description: TickLabels property. True if the text in the object changes font size when the object size changes. The default value is True
type: docs
url: /net/aspose.cells.charts/ticklabels/autoscalefont/
---
## TickLabels.AutoScaleFont property

True if the text in the object changes font size when the object size changes. The default value is True.

```csharp
public bool AutoScaleFont { get; set; }
```

### Examples

```csharp
// Called: chart.CategoryAxis.TickLabels.AutoScaleFont = true;
public void TickLabels_Property_AutoScaleFont()
{
    Workbook workbook = new Workbook();

    workbook.ChangePalette(Color.Orange, 53);

    workbook.ChangePalette(Color.LightBlue, 54);

    workbook.ChangePalette(Color.LightCoral, 55);

    Color[] colors = workbook.Colors;

    //Set default font

    Style style = workbook.DefaultStyle;

    style.Font.Name = "Tahoma";

    workbook.DefaultStyle = style;

    Cells cells = workbook.Worksheets[0].Cells;

    //Put a string into a cell

    cells["A1"].PutValue("Region");

    cells["A2"].PutValue("France");

    cells["A3"].PutValue("Germany");

    cells["A4"].PutValue("England");

    cells["B1"].PutValue("Marketing Costs");

    cells["B2"].PutValue(70000);

    cells["B3"].PutValue(55000);

    cells["B4"].PutValue(30000);

    Worksheet sheet = workbook.Worksheets[0];

    //Set the name of the worksheet

    sheet.Name = "Clustered Column";

    sheet.IsGridlinesVisible = false;

    //Create chart

    int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 1, 29, 10);

    Chart chart = sheet.Charts[chartIndex];

    //Add the nseries collection to a chart 

    chart.NSeries.Add("B2:B4", true);

    //Get or set the range of category axis values

    chart.NSeries.CategoryData = "A2:A4";

    //this works also fine.

    //chart.NSeries.CategoryData = "{\"Fra\",\"Ger\",\"Eng\"}";

    chart.NSeries.IsColorVaried = true;



    for (int i = 0; i < chart.NSeries[0].Points.Count; i++)
    {

        chart.NSeries[0].Points[i].Area.ForegroundColor = colors[53 + i];

    }


    //Set properties of chart title

    chart.Title.Text = "Marketing Costs by Region";

    chart.Title.Font.IsBold = true;

    chart.Title.Font.Color = Color.Black;

    chart.Title.Font.Size = 12;

    //Set properties of categoryaxis title

    chart.CategoryAxis.Title.Text = "Region";

    chart.CategoryAxis.Title.Font.Color = Color.Black;

    chart.CategoryAxis.TickLabels.AutoScaleFont = true;

    chart.CategoryAxis.TickLabels.RotationAngle = 45;

    chart.CategoryAxis.TickLabels.Font.Size = 10;

    chart.CategoryAxis.Title.Font.IsBold = true;

    chart.CategoryAxis.Title.Font.Size = 10;

    //Set properties of valueaxis title

    chart.ValueAxis.Title.Text = "In Thousands";

    chart.ValueAxis.Title.Font.Name = "Arial";

    chart.ValueAxis.Title.Font.Color = Color.Black;

    chart.ValueAxis.Title.Font.IsBold = true;

    chart.ValueAxis.Title.Font.Size = 10;

    chart.ValueAxis.Title.RotationAngle = 90;

    chart.ValueAxis.MajorUnit = double.Parse("20000");

    chart.ValueAxis.MaxValue = double.Parse("80000");

    chart.ValueAxis.MinorUnit = double.Parse("5000");

    chart.ValueAxis.MinValue = double.Parse("0");

    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    chart = workbook.Worksheets[0].Charts[0];
    Assert.AreEqual(chart.CategoryAxis.TickLabels.RotationAngle, 45, 0.01);
}
```

### See Also

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


