---
title: ListObject.PutCellFormula
second_title: Aspose.Cells for .NET API Reference
description: ListObject method. Put the formula to the cell in the table
type: docs
url: /net/aspose.cells.tables/listobject/putcellformula/
---
## PutCellFormula(int, int, string) {#putcellformula}

Put the formula to the cell in the table.

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | The row offset in the table. |
| columnOffset | Int32 | The column offset in the table. |
| formula | String | The formula of the cell. |

### Examples

```csharp
// Called: table.PutCellFormula(4, 2, "=C3");
public void ListObject_Method_PutCellFormula()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Cells cells = wb.Worksheets[0].Cells;
    ListObject table = wb.Worksheets[0].ListObjects[0];
    table.PutCellValue(4, 0, "88");
    table.PutCellValue(4, 1, 88);
    table.PutCellFormula(4, 2, "=C3");
    Assert.AreEqual("88", table.ListColumns[0].TotalsRowLabel);

    wb.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## PutCellFormula(int, int, string, bool) {#putcellformula_1}

Put the formula to the cell in the table.

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula, bool isTotalsRowFormula)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | The row offset in the table. |
| columnOffset | Int32 | The column offset in the table. |
| formula | String | The formula of the cell. |
| isTotalsRowFormula | Boolean |  |

### Examples

```csharp
// Called: l1.PutCellFormula(3, 0, "=23+34", true);
public void ListObject_Method_PutCellFormula()
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


