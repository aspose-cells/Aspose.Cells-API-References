---
title: Axis.BaseUnitScale
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents the base unit scale for the category axis
type: docs
url: /net/aspose.cells.charts/axis/baseunitscale/
---
## Axis.BaseUnitScale property

Represents the base unit scale for the category axis.

```csharp
public TimeUnit BaseUnitScale { get; set; }
```

### Remarks

Setting this property only takes effect when the CategoryType property is set to TimeScale.

### Examples

```csharp
// Called: AssertHelper.AreEqual(TimeUnit.Months, chart.CategoryAxis.BaseUnitScale, "chart.CategoryAxis.BaseUnitScale");
private void Axis_Property_BaseUnitScale(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["Sheet1"];
            Chart chart = sheet.Charts[0];
            AssertHelper.AreEqual(TimeUnit.Months, chart.CategoryAxis.BaseUnitScale, "chart.CategoryAxis.BaseUnitScale");
        }
```

### See Also

* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


