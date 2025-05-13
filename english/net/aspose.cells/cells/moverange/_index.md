---
title: Cells.MoveRange
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Moves the range
type: docs
url: /net/aspose.cells/cells/moverange/
---
## Cells.MoveRange method

Moves the range.

```csharp
public void MoveRange(CellArea sourceArea, int destRow, int destColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceArea | CellArea | The range which should be moved. |
| destRow | Int32 | The dest row. |
| destColumn | Int32 | The dest column. |

### Examples

```csharp
// Called: cells.MoveRange(cellarea, 65535, 255);
public void Cells_Method_MoveRange()
{
    caseName = "testMoveRange_003";
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells[0, 0].PutValue(1);
    CellArea cellarea = common.setCellArea(0, 0, 0, 0);
    cells.MoveRange(cellarea, 65535, 255);

    checkMoveRange_003(workbook);
    workbook.Save(Constants.destPath + " testMoveRange.xls");
    workbook = new Workbook(Constants.destPath + " testMoveRange.xls");
    checkMoveRange_003(workbook);
    workbook.Save(Constants.destPath + " testMoveRange.xlsx");
    workbook = new Workbook(Constants.destPath + " testMoveRange.xlsx");
    checkMoveRange_003(workbook);
    workbook.Save(Constants.destPath + " testMoveRange.xml", SaveFormat.SpreadsheetML);
    workbook = new Workbook(Constants.destPath + " testMoveRange.xml");
    checkMoveRange_003(workbook);
    workbook.Save(Constants.destPath + " testMoveRange.xls"); 
}
```

### See Also

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


