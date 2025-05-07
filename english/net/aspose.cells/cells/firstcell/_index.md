---
title: Cells.FirstCell
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the first cell in this worksheet
type: docs
url: /net/aspose.cells/cells/firstcell/
---
## Cells.FirstCell property

Gets the first cell in this worksheet.

```csharp
public Cell FirstCell { get; }
```

### Remarks

Returns null if there is no data in the worksheet.

### Examples

```csharp
// Called: chart.SetChartDataRange($"{cells.FirstCell.Name}:{cells.LastCell.Name}", true);
[Test]
        public void Property_FirstCell()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + @"CellsApp3843.xlsx");
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                var cells = worksheet.Cells;
                var chartIndex = worksheet.Charts.Add(ChartType.Column, 1, 1, 21, 15);
                var chart = worksheet.Charts[chartIndex];
                chart.SetChartDataRange($"{cells.FirstCell.Name}:{cells.LastCell.Name}", true);
                chart.ShowLegend = true;
            }
        }
```

### See Also

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


