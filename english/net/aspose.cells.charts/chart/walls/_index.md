---
title: Chart.Walls
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Returns a Walls object that represents the walls of a 3D chart
type: docs
url: /net/aspose.cells.charts/chart/walls/
---
## Chart.Walls property

Returns a `Walls` object that represents the walls of a 3-D chart.

```csharp
public Walls Walls { get; }
```

### Remarks

This property doesn't apply to 3-D pie charts.

### Examples

```csharp
// Called: Ch.Walls.ForegroundColor = Color.LightGray;
[Test]
        public void Property_Walls()
        {
            Workbook workbook = new Workbook();
            workbook.ChangePalette(Color.LightGray, 55);
            Cells cells = workbook.Worksheets[0].Cells;

            cells["A1"].PutValue("Year");
            cells["A2"].PutValue("2002Q3");
            cells["A3"].PutValue("2003Q3");
            cells["A4"].PutValue("2004Q3");
            cells["A5"].PutValue("2005Q3");
            cells["A6"].PutValue("2006Q3");
            cells["A7"].PutValue("2007Q3");

            cells["B1"].PutValue("Meals");
            cells["B2"].PutValue(30000000);
            cells["B3"].PutValue(35000000);
            cells["B4"].PutValue(40000000);
            cells["B5"].PutValue(43000000);
            cells["B6"].PutValue(47000000);
            cells["B7"].PutValue(51000000);

            for (int i = 1; i < 7; i++)
            {
                //cells[i, 1].Style.Custom = "#,##0";
                Style style = cells[i, 1].GetStyle();
                style.Custom = "#,##0";
                cells[i, 1].SetStyle(style);
            }

            workbook.Worksheets[0].AutoFitColumn(1);

            int ChartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column3DClustered, 4, 4, 19, 13);
            Chart Ch = workbook.Worksheets[0].Charts[0];

            Ch.NSeries.Add("B2:B7", true);
            Ch.NSeries.CategoryData = "a2:a7"; //error related lower case.


            Series S;
            S = Ch.NSeries[0];
            S.Name = "=B1";

            //Change the columns border color
            S.Border.Color = Color.Red;
            //Change the fill color for all the columns in the series.
            S.Area.ForegroundColor = Color.Maroon;

            //Change the first data point column's color to some custom color in the series.
            ChartPointCollection datapoints = Ch.NSeries[0].Points;
            datapoints[0].Area.Formatting = FormattingType.Custom;
            datapoints[0].Area.FillFormat.Texture = TextureType.BlueTissuePaper;

            Title valtitle = Ch.ValueAxis.Title;
            valtitle.Text = "Meals";
            valtitle.Font.IsBold = true;

            Title cattitle = Ch.CategoryAxis.Title;
            cattitle.Text = "Years";
            cattitle.Font.IsBold = true;


            Ch.ShowLegend = false;
            Ch.Title.Text = "Adult Total Meals";
            Ch.Title.Font.IsBold = true;
            Ch.Title.Font.Size = 12;

            Ch.PlotArea.Area.ForegroundColor = Color.White;
            Ch.PlotArea.Border.IsVisible = false;

            Ch.Walls.ForegroundColor = Color.LightGray;

            workbook.Save(Constants.destPath + "Test_159083.xls");
            workbook = new Workbook(Constants.destPath + "Test_159083.xls");
        }
```

### See Also

* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


