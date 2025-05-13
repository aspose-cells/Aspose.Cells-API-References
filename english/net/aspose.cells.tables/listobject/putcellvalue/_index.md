---
title: ListObject.PutCellValue
second_title: Aspose.Cells for .NET API Reference
description: ListObject method. Put the value to the cell
type: docs
url: /net/aspose.cells.tables/listobject/putcellvalue/
---
## PutCellValue(int, int, object) {#putcellvalue}

Put the value to the cell.

```csharp
public void PutCellValue(int rowOffset, int columnOffset, object value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | The row offset in the table. |
| columnOffset | Int32 | The column offset in the table. |
| value | Object | The cell value. |

### Examples

```csharp
// Called: lo.PutCellValue(2, 4, 1);
public void ListObject_Method_PutCellValue()
{
    string filePath = Constants.sourcePath + "example.xlsx";
    Workbook workbook = new Workbook(filePath);
    Worksheet worksheet = workbook.Worksheets[0];
    ListObject lo = worksheet.ListObjects[0];
    lo.PutCellValue(1, 0, 1);
    lo.PutCellValue(2, 0, 1);
    lo.PutCellValue(2, 4, 1);
    Assert.AreEqual(lo.EndColumn, 5);
    Assert.AreEqual(lo.EndRow, 2);
    Assert.AreEqual(worksheet.Cells["D2"].IsFormula, true);
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## PutCellValue(int, int, object, bool) {#putcellvalue_1}

Put the value to the cell.

```csharp
public void PutCellValue(int rowOffset, int columnOffset, object value, bool isTotalsRowLabel)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | The row offset in the table. |
| columnOffset | Int32 | The column offset in the table. |
| value | Object | The cell value. |
| isTotalsRowLabel | Boolean | Indicates whether it is a label for total row,only works for total row. If False and this row is total row, a new row will be inserted. |

### Examples

```csharp
// Called: l2.PutCellValue(3, 2, "sdfsfdsfd", true);
public void ListObject_Method_PutCellValue()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    ListObject l0 = workbook.Worksheets[0].ListObjects[0];
    l0.PutCellFormula(3, 0, "=23+34", false);
    Assert.AreEqual(4, l0.EndRow);
    ListObject l1 = workbook.Worksheets[1].ListObjects[0];
    l1.PutCellFormula(3, 0, "=23+34", true);
    Assert.AreEqual(3, l1.EndRow);
    Assert.AreEqual("=23+34", workbook.Worksheets[1].Cells["A4"].Formula);
    ListObject l2 = workbook.Worksheets[2].ListObjects[0];
    l2.PutCellValue(3, 2, "sdfsfdsfd", true);

    Assert.AreEqual(3, l2.EndRow);
    Assert.AreEqual("sdfsfdsfd", workbook.Worksheets[2].Cells["C4"].StringValue);

    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


