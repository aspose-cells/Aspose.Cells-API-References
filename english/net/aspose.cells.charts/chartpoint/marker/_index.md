---
title: ChartPoint.Marker
second_title: Aspose.Cells for .NET API Reference
description: ChartPoint property. Gets the  marker
type: docs
url: /net/aspose.cells.charts/chartpoint/marker/
---
## ChartPoint.Marker property

Gets the ` marker`.

```csharp
public Marker Marker { get; }
```

### Examples

```csharp
// Called: chart.NSeries[0].Points[intPointIndex].Marker.MarkerStyle = ChartMarkerType.Circle;
[Test]
        public void Property_Marker()
        {
            Console.WriteLine("Property_Marker()");
            string infn = path + "TEST_ScatterChartMarker.xlsx";
            string outfn = Constants.destPath + "TEST_ScatterChartMarker_out.xlsx";


            Workbook workbook = new Workbook();
            int sheetIndex = 0;

            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            worksheet.Cells["A1"].PutValue(150);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(33);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            int chartIndex = worksheet.Charts.Add(ChartType.Scatter, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            int intPointIndex = 0;

            chart.NSeries[0].Points[intPointIndex].Marker.Border.Color = Color.Yellow;
            chart.NSeries[0].Points[intPointIndex].Marker.Area.ForegroundColor = Color.Green;
            chart.NSeries[0].Points[intPointIndex].Marker.MarkerStyle = ChartMarkerType.Circle;
            chart.NSeries[0].Points[intPointIndex].Marker.MarkerSize = 16;

            workbook.Save(outfn);
        }
```

### See Also

* class [Marker](../../marker/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


