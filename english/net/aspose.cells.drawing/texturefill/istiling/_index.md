---
title: TextureFill.IsTiling
second_title: Aspose.Cells for .NET API Reference
description: TextureFill property. Indicates whether tile picture as texture
type: docs
url: /net/aspose.cells.drawing/texturefill/istiling/
---
## TextureFill.IsTiling property

Indicates whether tile picture as texture.

```csharp
public bool IsTiling { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(chart.PlotArea.Area.FillFormat.TextureFill.IsTiling);
[Test]
        public void Property_IsTiling()
        {

            Workbook workbook = new Workbook(Constants.sourcePath + &quot;user file(ChartDataLabels).xls&quot;);
            Chart chart = workbook.Worksheets[&quot;Motivation impact&quot;].Charts[0];
            Assert.IsFalse(chart.PlotArea.Area.FillFormat.TextureFill.IsTiling);
        }
```

### See Also

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


