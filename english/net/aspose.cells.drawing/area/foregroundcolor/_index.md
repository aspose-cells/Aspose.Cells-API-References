---
title: Area.ForegroundColor
second_title: Aspose.Cells for .NET API Reference
description: Area property. Gets or sets the foreground Color
type: docs
url: /net/aspose.cells.drawing/area/foregroundcolor/
---
## Area.ForegroundColor property

Gets or sets the foreground Color.

```csharp
public Color ForegroundColor { get; set; }
```

### Examples

```csharp
// Called: Ch.Walls.ForegroundColor = Color.LightGray;
[Test]
        public void Property_ForegroundColor()
        {
            Workbook workbook = new Workbook();
            workbook.ChangePalette(Color.LightGray, 55);
            Cells cells = workbook.Worksheets[0].Cells;

            cells[&quot;A1&quot;].PutValue(&quot;Year&quot;);
            cells[&quot;A2&quot;].PutValue(&quot;2002Q3&quot;);
            cells[&quot;A3&quot;].PutValue(&quot;2003Q3&quot;);
            cells[&quot;A4&quot;].PutValue(&quot;2004Q3&quot;);
            cells[&quot;A5&quot;].PutValue(&quot;2005Q3&quot;);
            cells[&quot;A6&quot;].PutValue(&quot;2006Q3&quot;);
            cells[&quot;A7&quot;].PutValue(&quot;2007Q3&quot;);

            cells[&quot;B1&quot;].PutValue(&quot;Meals&quot;);
            cells[&quot;B2&quot;].PutValue(30000000);
            cells[&quot;B3&quot;].PutValue(35000000);
            cells[&quot;B4&quot;].PutValue(40000000);
            cells[&quot;B5&quot;].PutValue(43000000);
            cells[&quot;B6&quot;].PutValue(47000000);
            cells[&quot;B7&quot;].PutValue(51000000);

            for (int i = 1; i &lt; 7; i++)
            {
                //cells[i, 1].Style.Custom = &quot;#,##0&quot;;
                Style style = cells[i, 1].GetStyle();
                style.Custom = &quot;#,##0&quot;;
                cells[i, 1].SetStyle(style);
            }

            workbook.Worksheets[0].AutoFitColumn(1);

            int ChartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column3DClustered, 4, 4, 19, 13);
            Chart Ch = workbook.Worksheets[0].Charts[0];

            Ch.NSeries.Add(&quot;B2:B7&quot;, true);
            Ch.NSeries.CategoryData = &quot;a2:a7&quot;; //error related lower case.


            Series S;
            S = Ch.NSeries[0];
            S.Name = &quot;=B1&quot;;

            //Change the columns border color
            S.Border.Color = Color.Red;
            //Change the fill color for all the columns in the series.
            S.Area.ForegroundColor = Color.Maroon;

            //Change the first data point column&apos;s color to some custom color in the series.
            ChartPointCollection datapoints = Ch.NSeries[0].Points;
            datapoints[0].Area.Formatting = FormattingType.Custom;
            datapoints[0].Area.FillFormat.Texture = TextureType.BlueTissuePaper;

            Title valtitle = Ch.ValueAxis.Title;
            valtitle.Text = &quot;Meals&quot;;
            valtitle.Font.IsBold = true;

            Title cattitle = Ch.CategoryAxis.Title;
            cattitle.Text = &quot;Years&quot;;
            cattitle.Font.IsBold = true;


            Ch.ShowLegend = false;
            Ch.Title.Text = &quot;Adult Total Meals&quot;;
            Ch.Title.Font.IsBold = true;
            Ch.Title.Font.Size = 12;

            Ch.PlotArea.Area.ForegroundColor = Color.White;
            Ch.PlotArea.Border.IsVisible = false;

            Ch.Walls.ForegroundColor = Color.LightGray;

            workbook.Save(Constants.destPath + &quot;Test_159083.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;Test_159083.xls&quot;);
        }
```

### See Also

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


