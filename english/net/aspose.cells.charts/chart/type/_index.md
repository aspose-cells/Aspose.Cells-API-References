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
// Called: AssertHelper.AreEqual(ChartType.Bar3DStacked, chart.Type, &amp;quot;chart.Type&amp;quot;);
private void Property_Type(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[&quot;Sheet5&quot;];
            Chart chart = sheet.Charts[0];
            AssertHelper.AreEqual(ChartType.Bar3DStacked, chart.Type, &quot;chart.Type&quot;);
        }
```

### See Also

* enum [ChartType](../../charttype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


