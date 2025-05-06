---
title: Axis.Title
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Gets the axis title
type: docs
url: /net/aspose.cells.charts/axis/title/
---
## Axis.Title property

Gets the axis' title.

```csharp
public Title Title { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(0, chart.ValueAxis.Title.RotationAngle);
[Test]
        public void Property_Title()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET46929.xlsx&quot;);
            Chart chart = workbook.Worksheets[0].Charts[1];
            Assert.AreEqual(0, chart.ValueAxis.Title.RotationAngle);
            workbook.Save(Constants.destPath + &quot;CELLSNET46929.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET46929.xlsx&quot;);
            chart = workbook.Worksheets[0].Charts[1];
            Assert.AreEqual(0, chart.ValueAxis.Title.RotationAngle);
        }
```

### See Also

* class [Title](../../title/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


