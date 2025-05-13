---
title: Chart.Type
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets or sets a charts type
type: docs
url: /net/aspose.cells.charts/chart/type/
---
## Chart.Type property

Gets or sets a chart's type.

```csharp
public ChartType Type { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(ChartType.Radar, chart.Type, "chart.Type");
private void Chart_Property_Type(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[0];
            AssertHelper.AreEqual(ChartType.Radar, chart.Type, "chart.Type");
        }
```

### See Also

* enum [ChartType](../../charttype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


