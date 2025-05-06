---
title: Chart.PlotArea
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets the charts plot area which includes axis tick labels
type: docs
url: /net/aspose.cells.charts/chart/plotarea/
---
## Chart.PlotArea property

Gets the chart's plot area which includes axis tick labels.

```csharp
public PlotArea PlotArea { get; }
```

### Examples

```csharp
// Called: FillFormat fillFormat = chart.PlotArea.Area.FillFormat;
private void Property_PlotArea(Workbook excel, Worksheet sheet, int currentRow, int currentColumn)
		{
			int chartIndex = sheet.Charts.Add(ChartType.Bar, 4, currentColumn + 3,
				26, currentColumn + 14);
			Chart chart = sheet.Charts[chartIndex];
			chart.ShowLegend = false;
			string startCell = CellsHelper.CellIndexToName(4, currentColumn + 1);
			string endCell = CellsHelper.CellIndexToName(currentRow, currentColumn + 1);
			chart.NSeries.Add(startCell + &quot;:&quot; + endCell, true);
			FillFormat fillFormat = chart.PlotArea.Area.FillFormat;
			fillFormat.SetPresetColorGradient(GradientPresetType.Daybreak, GradientStyleType.Vertical, 1);

			startCell = CellsHelper.CellIndexToName(4, currentColumn);
			endCell = CellsHelper.CellIndexToName(currentRow, currentColumn);
			chart.NSeries.CategoryData = startCell + &quot;:&quot; + endCell;
		}
```

### See Also

* class [PlotArea](../../plotarea/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


