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

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


