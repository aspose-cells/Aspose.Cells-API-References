---
title: Chart.ValueAxis
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets the charts Y axis
type: docs
url: /net/aspose.cells.charts/chart/valueaxis/
---
## Chart.ValueAxis property

Gets the chart's Y axis.

```csharp
public Axis ValueAxis { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(DisplayUnitType.HundredMillions, workbook.Worksheets[0].Charts[0].ValueAxis.DisplayUnit);
public void Chart_Property_ValueAxis()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Assert.AreEqual(DisplayUnitType.HundredMillions, workbook.Worksheets[0].Charts[0].ValueAxis.DisplayUnit);
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    Assert.AreEqual(DisplayUnitType.HundredMillions, workbook.Worksheets[0].Charts[0].ValueAxis.DisplayUnit);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual(DisplayUnitType.HundredMillions, workbook.Worksheets[0].Charts[0].ValueAxis.DisplayUnit);
}
```

### See Also

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


