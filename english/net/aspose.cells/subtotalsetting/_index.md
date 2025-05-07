---
title: Class SubtotalSetting
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.SubtotalSetting class. Represents the setting of the subtotal 
type: docs
url: /net/aspose.cells/subtotalsetting/
---
## SubtotalSetting class

Represents the setting of the subtotal .

```csharp
public class SubtotalSetting
```

## Properties

| Name | Description |
| --- | --- |
| [GroupBy](../../aspose.cells/subtotalsetting/groupby/) { get; } | The field to group by, as a zero-based integer offset |
| [SubtotalFunction](../../aspose.cells/subtotalsetting/subtotalfunction/) { get; } | The subtotal function. |
| [SummaryBelowData](../../aspose.cells/subtotalsetting/summarybelowdata/) { get; } | Indicates whether add summary below data. |
| [TotalList](../../aspose.cells/subtotalsetting/totallist/) { get; } | An array of zero-based field offsets, indicating the fields to which the subtotals are added. |

### Examples

```csharp
// Called: SubtotalSetting s = workbook.Worksheets[0].Cells.RetrieveSubtotalSetting(ca);
[Test]
        public void Type_SubtotalSetting()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet41637.xls");
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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


