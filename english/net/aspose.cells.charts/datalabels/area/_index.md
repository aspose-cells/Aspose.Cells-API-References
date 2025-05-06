---
title: DataLabels.Area
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Gets the area
type: docs
url: /net/aspose.cells.charts/datalabels/area/
---
## DataLabels.Area property

Gets the `area`.

```csharp
public override Area Area { get; }
```

### Examples

```csharp
// Called: aseries1.DataLabels.Area.BackgroundColor = Color.White;
[Test]
        public void Property_Area()
        {
            Console.WriteLine(&quot;Property_Area()&quot;);
            string outfn = Constants.destPath + &quot;TEST_ChartDataLabelFill_out.xlsx&quot;;

            Workbook workbook = new Workbook();
            int sheetIndex = 0;

            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            worksheet.Cells[&quot;A1&quot;].PutValue(150);
            worksheet.Cells[&quot;A2&quot;].PutValue(100);
            worksheet.Cells[&quot;A3&quot;].PutValue(150);
            worksheet.Cells[&quot;B1&quot;].PutValue(33);
            worksheet.Cells[&quot;B2&quot;].PutValue(20);
            worksheet.Cells[&quot;B3&quot;].PutValue(50);
            int chartIndex = worksheet.Charts.Add(ChartType.Scatter, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add(&quot;A1:B3&quot;, true);

            Series aseries1 = chart.NSeries[0];

            aseries1.DataLabels.ShowValue = true;
            aseries1.DataLabels.Area.FillFormat.Pattern = FillPattern.Solid;
            aseries1.DataLabels.Area.BackgroundColor = Color.White;

            workbook.Save(outfn);
        }
```

### See Also

* class [Area](../../../aspose.cells.drawing/area/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


