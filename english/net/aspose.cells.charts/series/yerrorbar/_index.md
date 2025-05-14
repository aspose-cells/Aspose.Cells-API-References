---
title: Series.YErrorBar
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents Y direction error bar of the series
type: docs
url: /net/aspose.cells.charts/series/yerrorbar/
---
## Series.YErrorBar property

Represents Y direction error bar of the series.

```csharp
public ErrorBar YErrorBar { get; }
```

### Examples

```csharp
// Called: ErrorBar errorbar = chart.NSeries[0].YErrorBar;
private void Series_Property_YErrorBar(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["Sheet2"];
            Chart chart = sheet.Charts[0];
            ErrorBar errorbar = chart.NSeries[0].YErrorBar;
            AssertHelper.AreEqual(ErrorBarType.Percent, errorbar.Type, "chart.NSeries[0].YErrorBar.Type");
        }
```

### See Also

* class [ErrorBar](../../errorbar/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


