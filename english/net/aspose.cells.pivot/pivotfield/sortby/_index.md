---
title: PivotField.SortBy
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Sorts this pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfield/sortby/
---
## SortBy(SortOrder, int) {#sortby}

Sorts this pivot field.

```csharp
public void SortBy(SortOrder sortType, int fieldSortedBy)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sortType | SortOrder | The type of sorting this field. |
| fieldSortedBy | Int32 | The index of pivot field sorted by. -1 means sorting by data labels of this field, others mean the index of data field sorted by. |

### See Also

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int, PivotLineType, string) {#sortby_1}

Sorts this pivot field.

```csharp
public void SortBy(SortOrder sortType, int fieldSortedBy, PivotLineType dataType, string cellName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sortType | SortOrder | The type of sorting this field. |
| fieldSortedBy | Int32 | The index of pivot field sorted by. -1 means sorting by data labels of this field, others mean the index of data field sorted by. |
| dataType | PivotLineType | The type of data sorted by. |
| cellName | String | Sort by values in the row or column |

### Examples

```csharp
// Called: workbook.Worksheets[0].PivotTables[0].RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, &amp;quot;G15&amp;quot;);
[Test]
        public void Method_String_()
        {
            var workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET46200.xlsx&quot;);
            workbook.Worksheets[0].PivotTables[0].RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, &quot;F15&quot;);
            workbook.Worksheets[0].PivotTables[0].CalculateData();
            Assert.AreEqual(&quot;7&quot;, workbook.Worksheets[0].Cells[&quot;F16&quot;].StringValue);
            workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET46200.xlsx&quot;);
            workbook.Worksheets[0].PivotTables[0].RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, &quot;G15&quot;);
            workbook.Worksheets[0].PivotTables[0].CalculateData();
            Assert.AreEqual(&quot;2&quot;, workbook.Worksheets[0].Cells[&quot;G16&quot;].StringValue);
        }
```

### See Also

* enum [SortOrder](../../../aspose.cells/sortorder/)
* enum [PivotLineType](../../pivotlinetype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


