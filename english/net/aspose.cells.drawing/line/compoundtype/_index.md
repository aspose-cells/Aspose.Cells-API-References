---
title: Line.CompoundType
second_title: Aspose.Cells for .NET API Reference
description: Line property. Specifies the compound line type
type: docs
url: /net/aspose.cells.drawing/line/compoundtype/
---
## Line.CompoundType property

Specifies the compound line type

```csharp
public MsoLineStyle CompoundType { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(MsoLineStyle.Single, ts0.CompoundType);
public void Line_Property_CompoundType()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "Charts/ChartAPI/UnvisibleTrendline.xlsx");
    Chart chart = workbook.Worksheets[0].Charts[0];
    SeriesCollection sc = chart.NSeries;
    TrendlineCollection tls = sc[0].TrendLines;
    Assert.AreEqual(1, tls.Count);
    Trendline ts0 = tls[0];
    Assert.AreEqual(LineCapType.Round, ts0.CapType);
    Assert.AreEqual(MsoLineStyle.Single, ts0.CompoundType);
    Assert.AreEqual(false, ts0.IsVisible);
    Assert.AreEqual(true, ts0.DisplayEquation);
}
```

### See Also

* enum [MsoLineStyle](../../msolinestyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


