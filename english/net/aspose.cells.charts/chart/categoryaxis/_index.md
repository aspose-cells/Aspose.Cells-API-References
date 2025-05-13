---
title: Chart.CategoryAxis
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets the charts X axis
type: docs
url: /net/aspose.cells.charts/chart/categoryaxis/
---
## Chart.CategoryAxis property

Gets the chart's X axis.

```csharp
public Axis CategoryAxis { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(CategoryType.CategoryScale, chart.CategoryAxis.CategoryType, "chart.CategoryAxis.CategoryType");
private void Chart_Property_CategoryAxis(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["Sheet1"];
            Chart chart = sheet.Charts[0];
            AssertHelper.AreEqual(CategoryType.CategoryScale, chart.CategoryAxis.CategoryType, "chart.CategoryAxis.CategoryType");
        }
```

### See Also

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


