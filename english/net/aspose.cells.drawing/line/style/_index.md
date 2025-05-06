---
title: Line.Style
second_title: Aspose.Cells for .NET API Reference
description: Line property. Represents the style of the line
type: docs
url: /net/aspose.cells.drawing/line/style/
---
## Line.Style property

Represents the style of the line.

```csharp
public LineType Style { get; set; }
```

### Examples

```csharp
// Called: chart.ValueAxis.MajorGridLines.Style = LineType.Dash;
[Test]
        public void Property_Style()
        {
            Console.WriteLine(&quot;Property_Style()&quot;);
            string infn = path + &quot;&quot;;
            string outfn = Constants.destPath + &quot;TEST_ChartMajorGridLineDashStyle.xlsx&quot;;

            Workbook workbook = new Workbook();
            int sheetIndex = 0;

            Worksheet sheet = workbook.Worksheets[sheetIndex];
            sheet.Cells[&quot;A1&quot;].PutValue(150);
            sheet.Cells[&quot;A2&quot;].PutValue(100);
            sheet.Cells[&quot;A3&quot;].PutValue(150);
            sheet.Cells[&quot;B1&quot;].PutValue(33);
            sheet.Cells[&quot;B2&quot;].PutValue(20);
            sheet.Cells[&quot;B3&quot;].PutValue(50);

            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 15, 0, 35, 10);
            Chart chart = sheet.Charts[chartIndex];
            chart.ValueAxis.MajorGridLines.Style = LineType.Dash;

            chart.NSeries.Add(&quot;A1:B3&quot;, true);

            ChartFrame plotarea = chart.PlotArea;
            plotarea.Area.BackgroundColor = Color.White;
            plotarea.Area.ForegroundColor = Color.White;

            workbook.Save(outfn);

            infn = Constants.destPath + &quot;TEST_ChartMajorGridLineDashStyle.xlsx&quot;;
            outfn = Constants.destPath + &quot;TEST_ChartMajorGridLineDashStyle_out.xls&quot;;

            workbook= new Workbook(infn);
            workbook.Save(outfn);

        }
```

### See Also

* enum [LineType](../../linetype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


