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
// Called: cells.DeleteRange(5, 5, 6, 6, ShiftType.Up);
[Test]
        public void Method_ShiftType_()
        {
            caseName = &quot;testDeleteRangeFormual_074&quot;;
            Workbook workbook = new Workbook();
            workbook = new Workbook(Constants.sourcePath + &quot;insertDelete\\testformual3.xls&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            cells.DeleteRange(5, 5, 6, 6, ShiftType.Up);

            checkDeleteRangeFormual(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkDeleteRangeFormual(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkDeleteRangeFormual(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
            checkDeleteRangeFormual(workbook);
            Util.SaveAsBuffer(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


