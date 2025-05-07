---
title: Legend.IsOverLay
second_title: Aspose.Cells for .NET API Reference
description: Legend property. Gets or sets whether showing the legend without overlapping the chart
type: docs
url: /net/aspose.cells.charts/legend/isoverlay/
---
## Legend.IsOverLay property

Gets or sets whether showing the legend without overlapping the chart.

```csharp
public bool IsOverLay { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Charts[0].Legend.IsOverLay, true);
[Test]
        public void Property_IsOverLay()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet42923.xlsx");
            Assert.AreEqual(workbook.Worksheets[0].Charts[0].Legend.IsOverLay, true);
        }
```

### See Also

* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


