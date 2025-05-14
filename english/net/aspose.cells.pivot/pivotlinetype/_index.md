---
title: Enum PivotLineType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotLineType enum. Specifies the type of the PivotLine
type: docs
url: /net/aspose.cells.pivot/pivotlinetype/
---
## PivotLineType enumeration

Specifies the type of the PivotLine.

```csharp
public enum PivotLineType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Regular | `0` | Regular PivotLine with pivot items. |
| Subtotal | `1` | Subtotal line. |
| GrandTotal | `2` | Grand Total line. |
| Blank | `3` | Blank line after each group. |

### Examples

```csharp
// Called: pTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "C3");
public void Pivot_Type_PivotLineType()
{
    var book = new Workbook(Constants.PivotTableSourcePath + "example.xlsb");
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
    book.Save(Constants.PivotTableDestPath + "example.xlsx");
}
```

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


