---
title: Axis.CustomDisplayUnit
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Specifies a custom value for the display unit
type: docs
url: /net/aspose.cells.charts/axis/customdisplayunit/
---
## Axis.CustomDisplayUnit property

Specifies a custom value for the display unit.

```csharp
public double CustomDisplayUnit { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1.0000000000000005E-8, chart.ValueAxis.CustomDisplayUnit);
public void Axis_Property_CustomDisplayUnit()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Chart chart = workbook.Worksheets[0].Charts[0];
    Assert.AreEqual(1.0000000000000005E-8, chart.ValueAxis.CustomDisplayUnit);
    workbook.Save(Constants.destPath + "example.pdf");
}
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


