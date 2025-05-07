---
title: ChartTextFrame.IsDeleted
second_title: Aspose.Cells for .NET API Reference
description: ChartTextFrame property. Indicates whether this data labels is deleted
type: docs
url: /net/aspose.cells.charts/charttextframe/isdeleted/
---
## ChartTextFrame.IsDeleted property

Indicates whether this data labels is deleted.

```csharp
public bool IsDeleted { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(chart.NSeries[2].DataLabels.IsDeleted);
[Test]
        public void Property_IsDeleted()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET44379.xlsx");
            workbook.Save(Constants.destPath + "CELLSNET44379.xlsx");
            workbook = new Workbook(Constants.destPath + "CELLSNET44379.xlsx");
            Chart chart = workbook.Worksheets[0].Charts[0];
            Assert.IsFalse(chart.NSeries[2].DataLabels.IsDeleted);
        }
```

### See Also

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


