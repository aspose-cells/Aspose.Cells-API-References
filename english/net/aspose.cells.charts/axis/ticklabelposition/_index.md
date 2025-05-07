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
// Called: chart.ValueAxis.TickLabelPosition = TickLabelPositionType.High;
[Test]
        public void Property_TickLabelPosition()
        {
            Workbook workbook = new Workbook();
            workbook = TestColumn.CreateChart(workbook);
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.ValueAxis.TickLabelPosition = TickLabelPositionType.High;

            checkTickLabelPositionType_High(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkTickLabelPositionType_High(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkTickLabelPositionType_High(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* enum [TickLabelPositionType](../../ticklabelpositiontype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


