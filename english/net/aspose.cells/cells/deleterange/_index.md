---
title: Cells.DeleteRange
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Deletes a range of cells and shift cells according to the shift option
type: docs
url: /net/aspose.cells/cells/deleterange/
---
## Cells.DeleteRange method

Deletes a range of cells and shift cells according to the shift option.

```csharp
public void DeleteRange(int startRow, int startColumn, int endRow, int endColumn, 
    ShiftType shiftType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index. |
| startColumn | Int32 | Start column index. |
| endRow | Int32 | End row index. |
| endColumn | Int32 | End column index. |
| shiftType | ShiftType | Shift cells option. |

### Examples

```csharp
// Called: cells.DeleteRange(0, 1, 1, 2, ShiftType.Left);
public void Cells_Method_DeleteRange()
{
    caseName = "testDeleteRangeComment_003";
    Workbook workbook = new Workbook();
  workbook = new Workbook(Constants.sourcePath + "insertDelete\\testComment.xls");
    Worksheet sheet = workbook.Worksheets[0];
    Cells cells = sheet.Cells;
    cells.DeleteRange(0, 1, 1, 2, ShiftType.Left);

    checkComment(workbook);
    workbook.Save(Constants.destPath + "testDeleteRangeComment.xls");
    workbook = new Workbook(Constants.destPath + "testDeleteRangeComment.xls");
    checkComment(workbook);
    workbook.Save(Constants.destPath + "testDeleteRangeComment.xlsx");
    workbook = new Workbook(Constants.destPath + "testDeleteRangeComment.xlsx");
    checkComment(workbook);
    workbook.Save(Constants.destPath + "testDeleteRangeComment.xml", SaveFormat.SpreadsheetML);
     workbook = new Workbook(Constants.destPath + "testDeleteRangeComment.xml");
    checkComment(workbook);
    workbook.Save(Constants.destPath + "testDeleteRangeComment.xls");
}
```

### See Also

* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


