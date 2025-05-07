---
title: TickLabels.NumberFormat
second_title: Aspose.Cells for .NET API Reference
description: TickLabels property. Represents the format string for the TickLabels object
type: docs
url: /net/aspose.cells.charts/ticklabels/numberformat/
---
## TickLabels.NumberFormat property

Represents the format string for the TickLabels object.

```csharp
public string NumberFormat { get; set; }
```

### Remarks

The formatting string is same as a custom format string setting to a cell. For example, "$0".

### Examples

```csharp
// Called: chart.ValueAxis.TickLabels.NumberFormat = "0";
[Test]
        public void Property_NumberFormat()
        {
            // http://www.aspose.com/community/forums/thread/211080/category-axis-min-and-max-values.aspx
            Console.WriteLine("Property_NumberFormat()");
            string outFn = Constants.destPath + "Test_CategoryAxMinMaxValues_out.xlsx";

            Workbook wb = new Workbook();

            wb.Worksheets.Clear();

            Worksheet ws = wb.Worksheets.Add("New");

            Style style = wb.CreateStyle();

            style.Name = "DateTimeStyle";

            style.Custom = "dd-mm hh:mm:ss";

            DateTime dt = DateTime.Now;

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

            chart.Title.Text = "Data";

            chart.ValueAxis.Title.Text = "unit";

            chart.CategoryAxis.MinValue = dt;

            chart.CategoryAxis.MaxValue = dt.AddHours(6);

            Series aSerie = chart.NSeries[chart.NSeries.Add(String.Format("{0}!{1}{2}:{1}{3}", ws.Name, "D", 24, 29), true)];

            aSerie.XValues = String.Format("{0}!{1}{2}:{1}{3}", ws.Name, "C", 24, 29);

            aSerie.Name = "Date";

            wb.Save(outFn);
        }
```

### See Also

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


