---
title: Chart.IsCellReferedByChart
second_title: Aspose.Cells for .NET API Reference
description: Chart method. Returns whether the cell refered by the chart
type: docs
url: /net/aspose.cells.charts/chart/iscellreferedbychart/
---
## Chart.IsCellReferedByChart method

Returns whether the cell refered by the chart.

```csharp
public bool IsCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | The sheet Index.-1 means the worksheet which contains current chart. |
| rowIndex | Int32 | The row index |
| columnIndex | Int32 | The column index |

### Examples

```csharp
// Called: Assert.IsTrue(chart.IsCellReferedByChart(-1, 2, 0));
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET53185.xlsx");
            Chart chart = workbook.Worksheets[0].Charts[0];
            Assert.IsTrue(chart.IsCellReferedByChart(-1, 2, 0));

        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


