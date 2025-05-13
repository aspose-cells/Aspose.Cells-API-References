---
title: DataLabels.Position
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Represents the position of the data label
type: docs
url: /net/aspose.cells.charts/datalabels/position/
---
## DataLabels.Position property

Represents the position of the data label.

```csharp
public LabelPositionType Position { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(LabelPositionType.Right, chart.NSeries[0].DataLabels.Position, "chart.NSeries[0].DataLabels.Position");
private void DataLabels_Property_Position(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[0];
            AssertHelper.AreEqual(LabelPositionType.Right, chart.NSeries[0].DataLabels.Position, "chart.NSeries[0].DataLabels.Position");
        }
```

### See Also

* enum [LabelPositionType](../../labelpositiontype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


