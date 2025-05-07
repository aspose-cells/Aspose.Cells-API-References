---
title: Axis.DisplayUnit
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents the unit label for the specified axis
type: docs
url: /net/aspose.cells.charts/axis/displayunit/
---
## Axis.DisplayUnit property

Represents the unit label for the specified axis.

```csharp
public DisplayUnitType DisplayUnit { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(DisplayUnitType.Hundreds, chart.ValueAxis.DisplayUnit, "chart.ValueAxis.DisplayUnit");
private void Property_DisplayUnit(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[0];
            AssertHelper.AreEqual(DisplayUnitType.Hundreds, chart.ValueAxis.DisplayUnit, "chart.ValueAxis.DisplayUnit");
        }
```

### See Also

* enum [DisplayUnitType](../../displayunittype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


