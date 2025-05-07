---
title: Enum LineCapType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.LineCapType enum. Represents the caps of a line
type: docs
url: /net/aspose.cells.drawing/linecaptype/
---
## LineCapType enumeration

Represents the caps of a line

```csharp
public enum LineCapType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Square | `0` | Square protrudes by half line width. |
| Round | `1` | Rounded ends. |
| Flat | `2` | Line ends at end point. |
| None | `3` | None cap |

### Examples

```csharp
// Called: Assert.AreEqual(LineCapType.Round, ts0.CapType);
[Test]
        public void Type_LineCapType()
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

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


