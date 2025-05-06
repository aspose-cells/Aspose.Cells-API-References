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
[Test]
        public void Property_TotalList()
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

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


