---
title: Area.BackgroundColor
second_title: Aspose.Cells for .NET API Reference
description: Area property. Gets or sets the background Color of the Area
type: docs
url: /net/aspose.cells.drawing/area/backgroundcolor/
---
## Area.BackgroundColor property

Gets or sets the background Color of the [`Area`](../).

```csharp
public Color BackgroundColor { get; set; }
```

### Examples

```csharp
// Called: plotarea.Area.BackgroundColor = Color.White;
[Test]
        public void Property_BackgroundColor()
        {
            Console.WriteLine("Property_BackgroundColor()");
            string infn = path + "";
            string outfn = Constants.destPath + "TEST_ChartMajorGridLineDashStyle.xlsx";

            Workbook workbook = new Workbook();
            int sheetIndex = 0;

            Worksheet sheet = workbook.Worksheets[sheetIndex];
            sheet.Cells["A1"].PutValue(150);
            sheet.Cells["A2"].PutValue(100);
            sheet.Cells["A3"].PutValue(150);
            sheet.Cells["B1"].PutValue(33);
            sheet.Cells["B2"].PutValue(20);
            sheet.Cells["B3"].PutValue(50);

            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 15, 0, 35, 10);
            Chart chart = sheet.Charts[chartIndex];
            chart.ValueAxis.MajorGridLines.Style = LineType.Dash;

            chart.NSeries.Add("A1:B3", true);

            ChartFrame plotarea = chart.PlotArea;
            plotarea.Area.BackgroundColor = Color.White;
            plotarea.Area.ForegroundColor = Color.White;

            workbook.Save(outfn);

            infn = Constants.destPath + "TEST_ChartMajorGridLineDashStyle.xlsx";
            outfn = Constants.destPath + "TEST_ChartMajorGridLineDashStyle_out.xls";

            workbook= new Workbook(infn);
            workbook.Save(outfn);

        }
```

### See Also

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


