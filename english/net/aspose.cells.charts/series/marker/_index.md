---
title: Series.Marker
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets the marker
type: docs
url: /net/aspose.cells.charts/series/marker/
---
## Series.Marker property

Gets the `marker`.

```csharp
public Marker Marker { get; }
```

### Examples

```csharp
// Called: aseries.Marker.MarkerStyle = ChartMarkerType.SquarePlus;
		public void Series_Property_Marker()
		{
			Workbook excel = new Workbook();
			Cells cells = excel.Worksheets[0].Cells;
			cells["A1"].PutValue(1);
			cells["A2"].PutValue(2);
			cells["A3"].PutValue(3);

			int chartIndex = excel.Worksheets[0].Charts.Add(ChartType.LineWithDataMarkers,  4, 4, 15, 10);
			Chart chart = excel.Worksheets[0].Charts[chartIndex];
			chart.NSeries.Add("A1:A3", true);

			for(int i = 0; i < chart.NSeries.Count; i ++)
			{
				Series aseries = chart.NSeries[i];
				aseries.Marker.MarkerStyle = ChartMarkerType.SquarePlus;
				aseries.Marker.MarkerSize = 10;
				aseries.Marker.Border.Color = Color.Red;
				aseries.Marker.BackgroundColor = Color.Yellow;
			}

            excel.Save(Constants.destPath + "chartmarker.xls");
		}
```

### See Also

* class [Marker](../../marker/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


