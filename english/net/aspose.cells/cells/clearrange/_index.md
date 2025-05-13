---
title: Cells.ClearRange
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Clears contents and formatting of a range
type: docs
url: /net/aspose.cells/cells/clearrange/
---
## ClearRange(CellArea) {#clearrange}

Clears contents and formatting of a range.

```csharp
public void ClearRange(CellArea range)
```

| Parameter | Type | Description |
| --- | --- | --- |
| range | CellArea | Range to be cleared. |

### See Also

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ClearRange(int, int, int, int) {#clearrange_1}

Clears contents and formatting of a range.

```csharp
public void ClearRange(int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index. |
| startColumn | Int32 | Start column index. |
| endRow | Int32 | End row index. |
| endColumn | Int32 | End column index. |

### Examples

```csharp
// Called: cells.ClearRange(0, 0, 1048575, 16383);
public void Cells_Method_ClearRange()
{
    caseName = "testClearRange_Excel2007_001";
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells[0, 0].PutValue(1);
    cells[0, 16383].PutValue(2);
    cells[1048575, 0].PutValue(3);
    cells[1048575, 16383].PutValue(4);
    cells.ClearRange(0, 0, 1048575, 16383);

    checkClearRange_Excel2007_001(workbook);
    workbook.Save(Constants.destPath + "testClearRange.xlsx");
    workbook = new Workbook(Constants.destPath + "testClearRange.xlsx");
    checkClearRange_Excel2007_001(workbook);
    workbook.Save(Constants.destPath + "testClearRange.xml", SaveFormat.SpreadsheetML);
    workbook = new Workbook(Constants.destPath + "testClearRange.xml");
    workbook.Save(Constants.destPath + "testClearRange.xls"); 
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


