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
[Test]
        public void Property_SummaryBelowData()
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


