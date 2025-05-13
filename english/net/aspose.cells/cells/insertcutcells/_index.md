---
title: Cells.InsertCutCells
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Insert cut range
type: docs
url: /net/aspose.cells/cells/insertcutcells/
---
## Cells.InsertCutCells method

Insert cut range.

```csharp
public void InsertCutCells(Range cutRange, int row, int column, ShiftType shiftType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cutRange | Range | The cut range. |
| row | Int32 | The row. |
| column | Int32 | The column. |
| shiftType | ShiftType | The shift type . |

### Examples

```csharp
// Called: dest.InsertCutCells(cells.CreateRange(0, 2, 3, 1), 1, 1, ShiftType.Down);
public void Cells_Method_InsertCutCells()
{
    Workbook wb = new Workbook();
    Cells dest = wb.Worksheets.Add("Sheet2").Cells;
    Cells cells = wb.Worksheets[0].Cells;
    string fml = "=SUM(C2,C2:D2,E2:F2,Sheet1!C2,Sheet1!C2:D2,Sheet2!C2,$C$1:C2,Sheet1!C1:$C$2,Sheet2!$C1:C$2)";
   // string fml = "=SUM(C2)";
    cells[2, 0].Formula = fml;
    cells[2, 2].Formula = fml;
    wb.Save(Constants.destPath + "TestRef3D.xlsx");
    dest.InsertCutCells(cells.CreateRange(0, 2, 3, 1), 1, 1, ShiftType.Down);
    Assert.AreEqual(CellValueType.IsNull, cells[2, 2].Type, "Cut Sheet1!A1.Type");
    Assert.IsNull(cells[2, 2].Formula, "Cut Sheet1!A1.Formula");
    Assert.AreEqual(
        "=SUM(Sheet2!B3,C2:D2,E2:F2,Sheet2!B3,Sheet1!C2:D2,Sheet2!C2,Sheet2!$B$2:B3,Sheet2!B2:$B$3,Sheet2!$C1:C$2)",
        //"=SUM(Sheet2!B3,D2:D2,E2:F2,Sheet2!B3,Sheet1!D2:D2,Sheet2!C2,Sheet2!$B$2:B3,Sheet2!B2:$B$3,Sheet2!$C1:C$2)", //should be this
        cells[2, 0].Formula, "Sheet2!B3.Formula");
    Assert.AreEqual(
        "=SUM(B3,Sheet2!C2:D2,Sheet1!E2:F2,Sheet2!B3,Sheet2!C2:D2,Sheet2!C2,$B$2:B3,Sheet2!B2:$B$3,Sheet2!$C1:C$2)",
        dest[3, 1].Formula, "Paste Sheet2!B4.Formula");
}
```

### See Also

* class [Range](../../range/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


