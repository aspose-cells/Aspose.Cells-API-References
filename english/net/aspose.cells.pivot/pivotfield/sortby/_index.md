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
// Called: pTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "C3");
[Test]
        public void Method_String_()
        {
            var book = new Workbook(Constants.PivotTableSourcePath + "CELLSNET47811.xlsb");
            Worksheet ws = book.Worksheets[1];
            var pTable = ws.PivotTables[0];

            pTable.RowFields[0].IsAutoSort = true;
            pTable.RowFields[0].IsAscendSort = false;
            pTable.RowFields[0].AutoSortField = pTable.DataFields.Count - 1;

            //How can I sort with the row field by values in certain Column field. 
            // example - something like below comments. 
            //pTable.RowFields[0].IsAutoSort = true;
            //pTable.RowFields[0].IsAscendSort = false;
            //pTable.RowFields[0].AutoSortField = pTable.ColumnFields.Items[1];
            pTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "C3");

            pTable.RefreshDataOnOpeningFile = true;
            // pTable.RefreshData();
            pTable.CalculateData();
            Assert.AreEqual(83000, ws.Cells["C3"].DoubleValue);
            book.Save(Constants.PivotTableDestPath + "CELLSNET47811.xlsx");
        }
```

### See Also

* enum [SortOrder](../../../aspose.cells/sortorder/)
* enum [PivotLineType](../../pivotlinetype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


