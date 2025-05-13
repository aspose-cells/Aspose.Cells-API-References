---
title: SubtotalSetting.SummaryBelowData
second_title: Aspose.Cells for .NET API Reference
description: SubtotalSetting property. Indicates whether add summary below data
type: docs
url: /net/aspose.cells/subtotalsetting/summarybelowdata/
---
## SubtotalSetting.SummaryBelowData property

Indicates whether add summary below data.

```csharp
public bool SummaryBelowData { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(s.SummaryBelowData);
public void SubtotalSetting_Property_SummaryBelowData()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    CellArea ca = CellArea.CreateCellArea("A2", "C24");
    SubtotalSetting s = workbook.Worksheets[0].Cells.RetrieveSubtotalSetting(ca);
    Assert.AreEqual(s.TotalList[0], 2);
    ca = CellArea.CreateCellArea("A2", "C30");
    s = workbook.Worksheets[1].Cells.RetrieveSubtotalSetting(ca);
    Assert.IsFalse(s.SummaryBelowData);
    Assert.AreEqual(1, s.GroupBy);
    Assert.AreEqual(ConsolidationFunction.Sum, s.SubtotalFunction);
}
```

### See Also

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


