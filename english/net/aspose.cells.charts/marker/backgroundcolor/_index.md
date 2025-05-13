---
title: Marker.BackgroundColor
second_title: Aspose.Cells for .NET API Reference
description: Marker property. Represents the marker background color in a line chart scatter chart or radar chart
type: docs
url: /net/aspose.cells.charts/marker/backgroundcolor/
---
## Marker.BackgroundColor property

Represents the marker background color in a line chart, scatter chart, or radar chart.

```csharp
public Color BackgroundColor { get; set; }
```

### Examples

```csharp
// Called: aseries.Marker.BackgroundColor = Color.Yellow;
		public void Marker_Property_BackgroundColor()
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

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


