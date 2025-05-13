---
title: SubtotalSetting.GroupBy
second_title: Aspose.Cells for .NET API Reference
description: SubtotalSetting property. The field to group by as a zerobased integer offset
type: docs
url: /net/aspose.cells/subtotalsetting/groupby/
---
## SubtotalSetting.GroupBy property

The field to group by, as a zero-based integer offset

```csharp
public int GroupBy { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1, s.GroupBy);
public void SubtotalSetting_Property_GroupBy()
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


