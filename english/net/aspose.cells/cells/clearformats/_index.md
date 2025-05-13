---
title: Cells.ClearFormats
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Clears formatting of a range
type: docs
url: /net/aspose.cells/cells/clearformats/
---
## ClearFormats(CellArea) {#clearformats}

Clears formatting of a range.

```csharp
public void ClearFormats(CellArea range)
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

## ClearFormats(int, int, int, int) {#clearformats_1}

Clears formatting of a range.

```csharp
public void ClearFormats(int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index. |
| startColumn | Int32 | Start column index. |
| endRow | Int32 | End row index. |
| endColumn | Int32 | End column index. |

### Examples

```csharp
// Called: cells.ClearFormats(1048575, 16383, 1048575, 16383);
public void Cells_Method_ClearFormats()
{
    caseName = "testClearFormats_Excel2007_002";
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    Style style = GetStyle(workbook);
    cells[0, 0].SetStyle(style);
    cells[0, 16383].SetStyle(style);
    cells[1048575, 0].SetStyle(style);
    cells[1048575, 16383].SetStyle(style);

    cells.ClearFormats(1048575, 16383, 1048575, 16383);

    checkClearFormats_Excel2007_002(workbook);
    workbook.Save(Constants.destPath + "testClearFormats.xlsx");
    workbook = new Workbook(Constants.destPath + "testClearFormats.xlsx");
    checkClearFormats_Excel2007_002(workbook);
    workbook.Save(Constants.destPath + "testClearFormats.xml", SaveFormat.SpreadsheetML);
    workbook = new Workbook(Constants.destPath + "testClearFormats.xml");
    workbook.Save(Constants.destPath + "testClearFormats.xls");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


