---
title: Cells.HideRows
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Hides multiple rows
type: docs
url: /net/aspose.cells/cells/hiderows/
---
## Cells.HideRows method

Hides multiple rows.

```csharp
public void HideRows(int row, int totalRows)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| totalRows | Int32 | The row number. |

### Examples

```csharp
// Called: cells.HideRows(0, firstRow);
public void Cells_Method_HideRows()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET47261/";

    var workBook = new Workbook(filePath + "Test2.xlsx");
    string RangeName = "RANGE1";
    var range = Array.Find(workBook.Worksheets.GetNamedRanges(), r => r.Name == RangeName);

    var sheet = range.Worksheet;
    var cells = sheet.Cells;
    var firstCol = range.FirstColumn;
    var firstRow = range.FirstRow;
    var maxCol = cells.MaxDisplayRange.ColumnCount;
    var maxRow = cells.MaxDisplayRange.RowCount;

    if (firstCol > 0)
    {
        cells.HideColumns(0, firstCol);
    }
    if (firstCol + range.ColumnCount < maxCol)
    {
        cells.HideColumns(firstCol + range.ColumnCount, maxCol - (firstCol + range.ColumnCount));
    }
    if (firstRow > 0)
    {
        cells.HideRows(0, firstRow);
    }
    if (firstRow + range.RowCount < maxRow)
    {
        cells.HideRows(firstRow + range.RowCount, maxRow - (firstRow + range.RowCount));
    }

    range.Worksheet.Workbook.Worksheets.ActiveSheetIndex = sheet.Index;

    var opts = new HtmlSaveOptions()
    {
        Encoding = Encoding.UTF8,
        HtmlCrossStringType = HtmlCrossType.Cross,
        PresentationPreference = true,
        ExportHiddenWorksheet = false,
        ExportActiveWorksheetOnly = true,
        ExportImagesAsBase64 = true,
        CreateDirectory = false,
        IsExpImageToTempDir = false,
        HiddenColDisplayType = HtmlHiddenColDisplayType.Remove,
        HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove
    };
    range.Worksheet.Workbook.Save(CreateFolder(filePath) + "out2.html", opts);

}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


