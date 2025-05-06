---
title: FillFormat.SetPresetColorGradient
second_title: Aspose.Cells for .NET API Reference
description: FillFormat method. Sets the specified fill to a presetcolor gradient. Only applies for Excel 2007
type: docs
url: /net/aspose.cells.drawing/fillformat/setpresetcolorgradient/
---
## FillFormat.SetPresetColorGradient method

Sets the specified fill to a preset-color gradient. Only applies for Excel 2007.

```csharp
public void SetPresetColorGradient(GradientPresetType presetColor, GradientStyleType style, 
    int variant)
```

| Parameter | Type | Description |
| --- | --- | --- |
| presetColor | GradientPresetType | Preset color type |
| style | GradientStyleType | Gradient shading style. |
| variant | Int32 | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### Examples

```csharp
// Called: fillFormat.SetPresetColorGradient(GradientPresetType.Daybreak, GradientStyleType.Vertical, 1);
private void Method_Int32_(Workbook excel, Worksheet sheet, int currentRow, int currentColumn)
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

* enum [GradientPresetType](../../gradientpresettype/)
* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


