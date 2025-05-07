---
title: DataLabels.ShowCellRange
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Indicates whether showing cell range as the data labels
type: docs
url: /net/aspose.cells.charts/datalabels/showcellrange/
---
## DataLabels.ShowCellRange property

Indicates whether showing cell range as the data labels.

```csharp
public bool ShowCellRange { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.NSeries[0].Points[0].DataLabels.ShowCellRange, true);
[Test]
        public void Property_ShowCellRange()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA-41094.xlsx");
            Chart chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(chart.NSeries[0].Points[0].DataLabels.ShowCellRange, true);

        }
```

### See Also

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


