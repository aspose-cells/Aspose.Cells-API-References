---
title: Cell.RemoveArrayFormula
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Remove array formula
type: docs
url: /net/aspose.cells/cell/removearrayformula/
---
## Cell.RemoveArrayFormula method

Remove array formula.

```csharp
public void RemoveArrayFormula(bool leaveNormalFormula)
```

| Parameter | Type | Description |
| --- | --- | --- |
| leaveNormalFormula | Boolean | True represents converting the array formula to normal formula. |

### Examples

```csharp
// Called: cell.RemoveArrayFormula(false);
public void Cell_Method_RemoveArrayFormula()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    //cells.MemorySetting = MemorySetting.MemoryPreference;
    Cell cell = cells["A1"];
    cell.SetArrayFormula("=B1:D1", 1, 1);
    cells["B1"].PutValue("#VALUE!");
    wb.CalculateFormula();
    cell.RemoveArrayFormula(false);
    Assert.IsFalse(cell.IsFormula, "A1(Single-False).IsFormula");
    Assert.AreEqual("#VALUE!", cell.Value, "A1(Single-False).Value");

    cell.SetArrayFormula("=B1:D1", 1, 1);
    cell.RemoveArrayFormula(true);
    Assert.IsFalse(cell.IsArrayHeader, "A1(Single-True).IsArrayHeader"); //CELLSNET-43695
    Assert.IsFalse(cell.IsArrayFormula, "A1(Single-True).IsArrayHeader");
    Assert.AreEqual("=B1:D1", cell.Formula, "A1(Single-True).Formula");

    cell.SetArrayFormula("=B1:D1", 1, 3);
    cells["D1"].PutValue("#VALUE!");
    wb.CalculateFormula();
    cell.RemoveArrayFormula(false);
    for (int i = 0; i < 3; i++)
    {
        char cn = (char)('A' + i);
        cell = cells[0, i];
        Assert.IsFalse(cell.IsFormula, cn + "1(Multiple-False).IsFormula");
        Assert.AreEqual("#VALUE!", cell.Value, cn + "1(Multiple-False).Value");
    }

    cell = cells["A1"];
    cell.SetArrayFormula("=B1:D1", 1, 3);
    cell.RemoveArrayFormula(true);
    for (int i = 0; i < 3; i++)
    {
        char cn = (char)('A' + i);
        cell = cells[0, i];
        Assert.IsFalse(cell.IsArrayHeader, cn + "1(Multiple-True).IsArrayHeader");
        Assert.IsFalse(cell.IsArrayFormula, cn + "1(Multiple-True).IsInArray");
        Assert.AreEqual("=B1:D1", cell.Formula, cn + "1(Multiple-True).Formula");
    }
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


