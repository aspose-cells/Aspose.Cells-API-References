---
title: Axis.TickLabels
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Returns a TickLabels object that represents the tickmark labels for the specified axis
type: docs
url: /net/aspose.cells.charts/axis/ticklabels/
---
## Axis.TickLabels property

Returns a `TickLabels` object that represents the tick-mark labels for the specified axis.

```csharp
public TickLabels TickLabels { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(axis.TickLabels.Font.IsBold);
[Test]
        public void Property_TickLabels()
        {
            var inputFileName = Constants.sourcePath + "CELLSNET57548.xlsx";
            var wb = new Workbook(inputFileName);

            Axis axis = wb.Worksheets["Op Earnings"].Charts[0].CategoryAxis;
            Assert.IsTrue(axis.TickLabels.Font.IsBold);
            wb.Save(Constants.destPath + "CELLSNET57548.xlsx", SaveFormat.Xlsx);
        }
```

### See Also

* class [TickLabels](../../ticklabels/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


