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

### Examples

```csharp
// Called: field.SortBy(SortOrder.Descending, -1);
public void PivotField_Method_SortBy()
{
    Workbook book = AddDateWorkbok();
    PivotTable pivot = AddDatePivotTable(book);

    Worksheet sheet = book.Worksheets[0];

    Cells cells = sheet.Cells;
    PivotField field = pivot.RowFields[0];
    field.SortBy(SortOrder.Descending, -1);

    pivot.RefreshData();
    pivot.CalculateData();

    Assert.AreEqual("USA", cells["A18"].StringValue);

    book.Save(Constants.destPath + "TestSortBy.xlsx");
}
```

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
// Called: workbook.Worksheets[0].PivotTables[0].RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "G15");
public void PivotField_Method_SortBy()
{
    var workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    workbook.Worksheets[0].PivotTables[0].RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "F15");
    workbook.Worksheets[0].PivotTables[0].CalculateData();
    Assert.AreEqual("7", workbook.Worksheets[0].Cells["F16"].StringValue);
    workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    workbook.Worksheets[0].PivotTables[0].RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "G15");
    workbook.Worksheets[0].PivotTables[0].CalculateData();
    Assert.AreEqual("2", workbook.Worksheets[0].Cells["G16"].StringValue);
}
```

### See Also

* enum [SortOrder](../../../aspose.cells/sortorder/)
* enum [PivotLineType](../../pivotlinetype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


