---
title: SubtotalSetting.SubtotalFunction
second_title: Aspose.Cells for .NET API Reference
description: SubtotalSetting property. The subtotal function
type: docs
url: /net/aspose.cells/subtotalsetting/subtotalfunction/
---
## SubtotalSetting.SubtotalFunction property

The subtotal function.

```csharp
public ConsolidationFunction SubtotalFunction { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(ConsolidationFunction.Sum, s.SubtotalFunction);
[Test]
        public void Property_SubtotalFunction()
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

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


