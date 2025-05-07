---
title: TickLabels.DisplayNumberFormat
second_title: Aspose.Cells for .NET API Reference
description: TickLabels property. Gets and sets the display number format of tick labels
type: docs
url: /net/aspose.cells.charts/ticklabels/displaynumberformat/
---
## TickLabels.DisplayNumberFormat property

Gets and sets the display number format of tick labels.

```csharp
public string DisplayNumberFormat { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("m/d/yyyy", workbook.Worksheets[0].Charts[0].CategoryAxis.TickLabels.DisplayNumberFormat);
[Test]
        public void Property_DisplayNumberFormat()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + @"CellsNet47447.xlsx");
            Assert.AreEqual("m/d/yyyy", workbook.Worksheets[0].Charts[0].CategoryAxis.TickLabels.DisplayNumberFormat);
            Assert.AreEqual("General",workbook.Worksheets[0].Charts[0].ValueAxis.TickLabels.DisplayNumberFormat);

        }
```

### See Also

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


