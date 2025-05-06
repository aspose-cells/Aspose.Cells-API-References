---
title: Marker.Area
second_title: Aspose.Cells for .NET API Reference
description: Marker property. Gets the area
type: docs
url: /net/aspose.cells.charts/marker/area/
---
## Marker.Area property

Gets the `area`.

```csharp
public Area Area { get; }
```

### Examples

```csharp
// Called: chart.NSeries[0].Points[intPointIndex].Marker.Area.ForegroundColor = Color.Green;
[Test]
        public void Property_Area()
        {
            Console.WriteLine(&quot;Property_Area()&quot;);
            string infn = path + &quot;TEST_ScatterChartMarker.xlsx&quot;;
            string outfn = Constants.destPath + &quot;TEST_ScatterChartMarker_out.xlsx&quot;;


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
            int intPointIndex = 0;

            chart.NSeries[0].Points[intPointIndex].Marker.Border.Color = Color.Yellow;
            chart.NSeries[0].Points[intPointIndex].Marker.Area.ForegroundColor = Color.Green;
            chart.NSeries[0].Points[intPointIndex].Marker.MarkerStyle = ChartMarkerType.Circle;
            chart.NSeries[0].Points[intPointIndex].Marker.MarkerSize = 16;

            workbook.Save(outfn);
        }
```

### See Also

* class [Area](../../../aspose.cells.drawing/area/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


