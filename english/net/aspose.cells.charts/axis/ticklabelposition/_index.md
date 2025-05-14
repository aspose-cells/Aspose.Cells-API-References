---
title: Axis.TickLabelPosition
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents the position of tickmark labels on the specified axis
type: docs
url: /net/aspose.cells.charts/axis/ticklabelposition/
---
## Axis.TickLabelPosition property

Represents the position of tick-mark labels on the specified axis.

```csharp
public TickLabelPositionType TickLabelPosition { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Charts[0].CategoryAxis.TickLabelPosition, TickLabelPositionType.NextToAxis);
public void Axis_Property_TickLabelPosition()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.ods");
    Assert.AreEqual(1, workbook.Worksheets[0].Charts.Count);
    Assert.AreEqual(workbook.Worksheets[0].Charts[0].Legend.Position, LegendPositionType.Right);
    Assert.AreEqual(workbook.Worksheets[0].Charts[0].CategoryAxis.TickLabelPosition, TickLabelPositionType.NextToAxis);
}
```

### See Also

* enum [TickLabelPositionType](../../ticklabelpositiontype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


