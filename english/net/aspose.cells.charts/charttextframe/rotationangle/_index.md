---
title: ChartTextFrame.RotationAngle
second_title: Aspose.Cells for .NET API Reference
description: ChartTextFrame property. Represents text rotation angle
type: docs
url: /net/aspose.cells.charts/charttextframe/rotationangle/
---
## ChartTextFrame.RotationAngle property

Represents text rotation angle.

```csharp
public int RotationAngle { get; set; }
```

### Remarks

0: Not rotated.255: Top to Bottom.-90: Downward.90: Upward.

### Examples

```csharp
// Called: Assert.AreEqual(0, chart.ValueAxis.Title.RotationAngle);
public void ChartTextFrame_Property_RotationAngle()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Chart chart = workbook.Worksheets[0].Charts[1];
    Assert.AreEqual(0, chart.ValueAxis.Title.RotationAngle);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    chart = workbook.Worksheets[0].Charts[1];
    Assert.AreEqual(0, chart.ValueAxis.Title.RotationAngle);
}
```

### See Also

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


