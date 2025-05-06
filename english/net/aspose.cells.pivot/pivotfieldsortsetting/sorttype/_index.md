---
title: PivotFieldSortSetting.SortType
second_title: Aspose.Cells for .NET API Reference
description: PivotFieldSortSetting property. Represents the SortOrder
type: docs
url: /net/aspose.cells.pivot/pivotfieldsortsetting/sorttype/
---
## PivotFieldSortSetting.SortType property

Represents the [`SortOrder`](../../../aspose.cells/sortorder/).

```csharp
public SortOrder SortType { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(SortOrder.Ascending, workbook.Worksheets[0].PivotTables[0].RowFields[0].SortSetting.SortType);
[Test]
        public void Property_SortType()
        {
            var workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET46200_1.xlsx&quot;);
            workbook.Worksheets[0].PivotTables[0].RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, &quot;K15&quot;);
          
            Assert.AreEqual(&quot;K15&quot;, workbook.Worksheets[0].PivotTables[0].RowFields[0].SortSetting.Cell);
            workbook.Worksheets[0].PivotTables[0].RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, &quot;M15&quot;);
            Assert.AreEqual(SortOrder.Ascending, workbook.Worksheets[0].PivotTables[0].RowFields[0].SortSetting.SortType);
            Assert.AreEqual(&quot;M15&quot;, workbook.Worksheets[0].PivotTables[0].RowFields[0].SortSetting.Cell);

            workbook.Worksheets[0].PivotTables[0].RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, &quot;N15&quot;);
            Assert.AreEqual(PivotLineType.GrandTotal, workbook.Worksheets[0].PivotTables[0].RowFields[0].SortSetting.LineTypeSortedBy);
            Assert.IsTrue(string.IsNullOrEmpty(workbook.Worksheets[0].PivotTables[0].RowFields[0].SortSetting.Cell));
        }
```

### See Also

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


