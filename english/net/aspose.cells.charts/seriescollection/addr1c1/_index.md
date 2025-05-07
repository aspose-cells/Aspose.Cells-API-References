---
title: SeriesCollection.AddR1C1
second_title: Aspose.Cells for .NET API Reference
description: SeriesCollection method. Adds the Series collection to a chart
type: docs
url: /net/aspose.cells.charts/seriescollection/addr1c1/
---
## SeriesCollection.AddR1C1 method

Adds the [`Series`](../../series/) collection to a chart.

```csharp
public int AddR1C1(string area, bool isVertical)
```

| Parameter | Type | Description |
| --- | --- | --- |
| area | String | Specifies values from which to plot the data series |
| isVertical | Boolean | Specifies whether to plot the series from a range of cell values by row or by column. |

### Return Value

Return the first index of the added ASeries in the NSeries.

### Remarks

If set data on contiguous cells, use colon to seperate them.For example, R[1]C[1]:R[3]C[2].If set data on contiguous cells, use comma to seperate them.For example,(R[1]C[1],R[3]C[2]).

### Examples

```csharp
// Called: int nSeriesIndex = cht.NSeries.AddR1C1("ChartData!R1C2:R2C2", true);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook();

            Workbook wb = new Workbook();
            Worksheet wsData = wb.Worksheets[0];
            wsData.Name = "ChartData";


            wsData.Cells[0, 0].PutValue(0.0000000442560022338624);
            wsData.Cells[1, 0].PutValue(-2.22222222222222);

            wsData.Cells[0, 1].PutValue(0.00000141515027515068);
            wsData.Cells[1, 1].PutValue(0.000000824676349690628);


            wsData.AutoFitColumns();


            Worksheet wsChart = wb.Worksheets[wb.Worksheets.Add(SheetType.Chart)];


            //wsChart.Name = "tab name";

            //'but this works:
            //wsChart.Name = "tab_name";

            // 'adding chart...
            int chartIndex = wsChart.Charts.Add(ChartType.ScatterConnectedByCurvesWithoutDataMarker, 0, 0, 10, 10);
            Chart cht = wsChart.Charts[chartIndex];

            // 'adding series...
            int nSeriesIndex = cht.NSeries.AddR1C1("ChartData!R1C2:R2C2", true);
            Series aSeries = cht.NSeries[nSeriesIndex];
            aSeries.XValues = "ChartData!A1:A2";
            aSeries.Marker.MarkerSize = 7;

            wb.Worksheets.ActiveSheetIndex = 1;


            wb.Save(Constants.destPath + "spaces.html", SaveFormat.Html);
        }
```

### See Also

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


