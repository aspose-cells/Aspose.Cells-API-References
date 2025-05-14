---
title: Chart.FirstSliceAngle
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets or sets the angle of the first piechart or doughnutchart slice in degrees clockwise from vertical. Applies only to pie 3D pie and doughnut charts 0 to 360
type: docs
url: /net/aspose.cells.charts/chart/firstsliceangle/
---
## Chart.FirstSliceAngle property

Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.

```csharp
public int FirstSliceAngle { get; set; }
```

### Examples

```csharp
// Called: chart.FirstSliceAngle = 15;
		public void Chart_Property_FirstSliceAngle()
		{
			Workbook excel = new Workbook();
			Worksheet sheet = excel.Worksheets[0];
			sheet.Cells["h3"].PutValue(1);
			sheet.Cells["h4"].PutValue(2);
			sheet.Cells["h5"].PutValue(3);

			int chartIndex = sheet.Charts.Add(ChartType.Pie, 3, 3, 8, 6);
			Chart chart = sheet.Charts[chartIndex];
			chart.NSeries.Add("h3:h5", true);
			chart.FirstSliceAngle = 15;

			excel.Save(Constants.destPath + "pieangle.xls");

		}
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


