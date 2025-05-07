---
title: Chart.SizeWithWindow
second_title: Aspose.Cells for .NET API Reference
description: Chart property. True if Microsoft Excel resizes the chart to match the size of the chart sheet window
type: docs
url: /net/aspose.cells.charts/chart/sizewithwindow/
---
## Chart.SizeWithWindow property

True if Microsoft Excel resizes the chart to match the size of the chart sheet window.

```csharp
public bool SizeWithWindow { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(workbook.Worksheets[0].Charts[0].SizeWithWindow);
[Test]
        public void Property_SizeWithWindow()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET43270.xlsx");
            Assert.IsFalse(workbook.Worksheets[0].Charts[0].SizeWithWindow);
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


