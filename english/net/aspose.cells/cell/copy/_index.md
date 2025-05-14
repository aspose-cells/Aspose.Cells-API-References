---
title: Cell.Copy
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Copies data from a source cell
type: docs
url: /net/aspose.cells/cell/copy/
---
## Cell.Copy method

Copies data from a source cell.

```csharp
public void Copy(Cell cell)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cell | Cell | Source [`Cell`](../) object. |

### Examples

```csharp
// Called: cells["C5"].Copy(cells["C4"]);
public void Cell_Method_Copy()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Cells cells = workbook.Worksheets[0].Cells;
    cells["C5"].Copy(cells["C4"]);
    string fml = "=IF(Table1[@Title]=$B5,FALSE, TRUE)";
    Assert.AreEqual(cells["C5"].Formula,
        workbook.Settings.FormulaSettings.PreservePaddingSpaces ? fml : fml.Replace(" ", ""));
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


