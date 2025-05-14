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
public void ChartTextFrame_Property_IsDeleted()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Chart chart = workbook.Worksheets[0].Charts[0];
    Assert.IsFalse(chart.NSeries[2].DataLabels.IsDeleted);
}
```

### See Also

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


