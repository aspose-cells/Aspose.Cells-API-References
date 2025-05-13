---
title: Axis.IsAutomaticMajorUnit
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Indicates whether the major unit of the axis is automatically assigned
type: docs
url: /net/aspose.cells.charts/axis/isautomaticmajorunit/
---
## Axis.IsAutomaticMajorUnit property

Indicates whether the major unit of the axis is automatically assigned.

```csharp
public bool IsAutomaticMajorUnit { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.ValueAxis.IsAutomaticMajorUnit, true);
public void Axis_Property_IsAutomaticMajorUnit()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Chart chart = workbook.Worksheets[0].Charts[0];
    Assert.AreEqual(chart.ValueAxis.IsAutomaticMajorUnit, true);
}
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


