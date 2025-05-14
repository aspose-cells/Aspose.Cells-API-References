---
title: CellArea.StartColumn
second_title: Aspose.Cells for .NET API Reference
description: CellArea field. Gets or set the start column of this area
type: docs
url: /net/aspose.cells/cellarea/startcolumn/
---
## CellArea.StartColumn field

Gets or set the start column of this area.

```csharp
public int StartColumn;
```

### Examples

```csharp
// Called: ca.StartColumn = 0;
public void CellArea_Field_StartColumn()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "InsertInRangeAndIndex.xlsx");
    Cells sourceCells = workbook.Worksheets[0].Cells;
          
    Aspose.Cells.Range sourceRange = sourceCells.CreateRange(0, 0, 1, 1);

    CellArea ca = new CellArea();
    ca.StartRow = 1;
    ca.EndRow = ca.StartRow;
    ca.StartColumn = 0;
    ca.EndColumn = 0;
    sourceCells.InsertRange(ca, 1, ShiftType.Down, true);
    Assert.AreEqual(sourceCells["A1"].Formula, "=SUM(A3:INDEX(A:A,ROW()+1))");

}
```

### See Also

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


