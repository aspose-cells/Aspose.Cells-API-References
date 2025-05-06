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
// Called: SubtotalSetting s = workbook.Worksheets[0].Cells.RetrieveSubtotalSetting(ca);
[Test]
        public void Method_CellArea_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet41637.xls&quot;);
            CellArea ca = CellArea.CreateCellArea(&quot;A2&quot;, &quot;C24&quot;);
            SubtotalSetting s = workbook.Worksheets[0].Cells.RetrieveSubtotalSetting(ca);
            Assert.AreEqual(s.TotalList[0], 2);
            ca = CellArea.CreateCellArea(&quot;A2&quot;, &quot;C30&quot;);
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


