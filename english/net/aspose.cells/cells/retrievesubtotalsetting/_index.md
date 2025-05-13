---
title: Cells.RetrieveSubtotalSetting
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Retrieves subtotals setting of the range
type: docs
url: /net/aspose.cells/cells/retrievesubtotalsetting/
---
## Cells.RetrieveSubtotalSetting method

Retrieves subtotals setting of the range.

```csharp
public SubtotalSetting RetrieveSubtotalSetting(CellArea ca)
```

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The range |

### Examples

```csharp
// Called: s = workbook.Worksheets[1].Cells.RetrieveSubtotalSetting(ca);
public void Cells_Method_RetrieveSubtotalSetting()
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

* class [SubtotalSetting](../../subtotalsetting/)
* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


