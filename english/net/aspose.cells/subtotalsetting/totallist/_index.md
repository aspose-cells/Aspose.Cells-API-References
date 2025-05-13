---
title: SubtotalSetting.TotalList
second_title: Aspose.Cells for .NET API Reference
description: SubtotalSetting property. An array of zerobased field offsets indicating the fields to which the subtotals are added
type: docs
url: /net/aspose.cells/subtotalsetting/totallist/
---
## SubtotalSetting.TotalList property

An array of zero-based field offsets, indicating the fields to which the subtotals are added.

```csharp
public int[] TotalList { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(s.TotalList[0], 2);
public void SubtotalSetting_Property_TotalList()
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


