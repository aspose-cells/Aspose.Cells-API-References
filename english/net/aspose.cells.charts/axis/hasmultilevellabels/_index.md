---
title: Axis.HasMultiLevelLabels
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Indicates whether the labels shall be shown as multi level
type: docs
url: /net/aspose.cells.charts/axis/hasmultilevellabels/
---
## Axis.HasMultiLevelLabels property

Indicates whether the labels shall be shown as multi level.

```csharp
public bool HasMultiLevelLabels { get; set; }
```

### Remarks

Only valid for category axis.

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Charts[0].CategoryAxis.HasMultiLevelLabels, false);
[Test]
        public void Property_HasMultiLevelLabels()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet40010.xlsx&quot;);
            Assert.AreEqual(workbook.Worksheets[0].Charts[0].CategoryAxis.HasMultiLevelLabels, false);

        }
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


