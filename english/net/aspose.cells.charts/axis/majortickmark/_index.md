---
title: Axis.MajorTickMark
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents the type of major tick mark for the specified axis
type: docs
url: /net/aspose.cells.charts/axis/majortickmark/
---
## Axis.MajorTickMark property

Represents the type of major tick mark for the specified axis.

```csharp
public TickMarkType MajorTickMark { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(TickMarkType.Outside, chart.ValueAxis.MajorTickMark, "chart.ValueAxis.MajorTickMark");
private void Axis_Property_MajorTickMark(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[0];
            AssertHelper.AreEqual(TickMarkType.Outside, chart.ValueAxis.MajorTickMark, "chart.ValueAxis.MajorTickMark");
        }
```

### See Also

* enum [TickMarkType](../../tickmarktype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


