---
title: TickLabels.Font
second_title: Aspose.Cells for .NET API Reference
description: TickLabels property. Returns a Font object that represents the font of the specified TickLabels object
type: docs
url: /net/aspose.cells.charts/ticklabels/font/
---
## TickLabels.Font property

Returns a `Font` object that represents the font of the specified TickLabels object.

```csharp
public Font Font { get; }
```

### Examples

```csharp
// Called: chart.CategoryAxis.TickLabels.Font.Size = 8;
[Test]
        public void Property_Font()
        {
            Workbook wb = new Workbook();

            wb.Worksheets.Clear();

            Worksheet ws = wb.Worksheets.Add("New");

            Style style = wb.CreateStyle();

            style.Name = "DateTimeStyle";

            style.Custom = "dd-mm hh:mm:ss";

            DateTime dt = DateTime.Now;

            ws.Cells[23, 2].PutValue(dt);

            ws.Cells[23, 2].SetStyle(style);

            ws.Cells[24, 2].PutValue(dt.AddHours(1));

            ws.Cells[24, 2].SetStyle(style);

            ws.Cells[25, 2].PutValue(dt.AddHours(2));

            ws.Cells[25, 2].SetStyle(style);

            ws.Cells[26, 2].PutValue(dt.AddHours(3));

            ws.Cells[26, 2].SetStyle(style);

            ws.Cells[27, 2].PutValue(dt.AddHours(4));

            ws.Cells[27, 2].SetStyle(style);

            ws.Cells[28, 2].PutValue(dt.AddHours(5));

            ws.Cells[28, 2].SetStyle(style);

            ws.Cells[29, 2].PutValue(dt.AddHours(6));

            ws.Cells[29, 2].SetStyle(style);

            ws.Cells[23, 3].PutValue(3);

            ws.Cells[24, 3].PutValue(4);

            ws.Cells[25, 3].PutValue(9);

            ws.Cells[26, 3].PutValue(13);

            ws.Cells[27, 3].PutValue(16);

            ws.Cells[28, 3].PutValue(3);

            ws.Cells[29, 3].PutValue(7);

            Chart chart = ws.Charts[ws.Charts.Add(ChartType.ScatterConnectedByLinesWithoutDataMarker, 1, 1, 22, 12)];

            chart.CategoryAxis.TickLabels.NumberFormat = "dd-mm hh:mm;@";

            chart.CategoryAxis.TickLabels.RotationAngle = 45;

            chart.CategoryAxis.TickLabels.Font.Size = 8;

            chart.Legend.Position = LegendPositionType.Bottom;

            chart.ValueAxis.TickLabels.NumberFormat = "0";

            chart.ValueAxis.MinValue = 0;

            chart.ValueAxis.MaxValue = 20;

            chart.Placement = PlacementType.Move;

            String chartSubTitle = DateTime.Now.ToString();
            string title = "Data" + "\n" + chartSubTitle;

            chart.Title.Text = title;

            FontSetting chars = chart.Title.Characters(chart.Title.Text.Length - chartSubTitle.Length, chartSubTitle.Length);

            chart.ValueAxis.Title.Text = "unit";

            Series aSerie = chart.NSeries[chart.NSeries.Add(String.Format("{0}!{1}{2}:{1}{3}", ws.Name, "D", 24, 30), true)];

            aSerie.XValues = String.Format("{0}!{1}{2}:{1}{3}", ws.Name, "C", 24, 30);

            aSerie.Name = "Date";

            wb.Save(Constants.destPath + "Test217130.xlsx");
            wb = new Workbook(Constants.destPath + "Test217130.xlsx");
            Assert.AreEqual(wb.Worksheets["New"].Charts[0].Title.Text, title);

        }
```

### See Also

* class [Font](../../../aspose.cells/font/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


