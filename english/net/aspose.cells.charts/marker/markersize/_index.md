---
title: Marker.MarkerSize
second_title: Aspose.Cells for .NET API Reference
description: Marker property. Represents the marker size in unit of points. Applies to line chart scatter chart or radar chart
type: docs
url: /net/aspose.cells.charts/marker/markersize/
---
## Marker.MarkerSize property

Represents the marker size in unit of points. Applies to line chart, scatter chart, or radar chart.

```csharp
public int MarkerSize { get; set; }
```

### Examples

```csharp
// Called: aSeries.Marker.MarkerSize = 7;
[Test, Category(&quot;Bug&quot;)]
        public void Property_MarkerSize()
        {
            Workbook workbook = new Workbook();

            Workbook wb = new Workbook();
            Worksheet wsData = wb.Worksheets[0];
            wsData.Name = &quot;ChartData&quot;;


            wsData.Cells[0, 0].PutValue(0.0000000442560022338624);
            wsData.Cells[1, 0].PutValue(-2.22222222222222);

            wsData.Cells[0, 1].PutValue(0.00000141515027515068);
            wsData.Cells[1, 1].PutValue(0.000000824676349690628);


            wsData.AutoFitColumns();


            Worksheet wsChart = wb.Worksheets[wb.Worksheets.Add(SheetType.Chart)];


            wsChart.Name = &quot;tab name&quot;;

            //&apos;but this works:
            //wsChart.Name = &quot;tab_name&quot;;

            // &apos;adding chart...
            int chartIndex = wsChart.Charts.Add(ChartType.ScatterConnectedByCurvesWithoutDataMarker, 0, 0, 10, 10);
            Chart cht = wsChart.Charts[chartIndex];

            // &apos;adding series...
            int nSeriesIndex = cht.NSeries.AddR1C1(&quot;ChartData!R1C2:R2C2&quot;, true);
            Series aSeries = cht.NSeries[nSeriesIndex];
            aSeries.XValues = &quot;ChartData!A1:A2&quot;;
            aSeries.Marker.MarkerSize = 7;

            wb.Worksheets.ActiveSheetIndex = 1;


            wb.Save(Constants.destPath + &quot;spaces.html&quot;, SaveFormat.Html);
        }
```

### See Also

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


