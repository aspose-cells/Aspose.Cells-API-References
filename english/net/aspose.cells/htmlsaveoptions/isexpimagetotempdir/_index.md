---
title: HtmlSaveOptions.IsExpImageToTempDir
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether exporting image files to temp directory. Only for saving to html stream
type: docs
url: /net/aspose.cells/htmlsaveoptions/isexpimagetotempdir/
---
## HtmlSaveOptions.IsExpImageToTempDir property

Indicates whether exporting image files to temp directory. Only for saving to html stream.

```csharp
public bool IsExpImageToTempDir { get; set; }
```

### Examples

```csharp
// Called: options.IsExpImageToTempDir = (false);
private void Property_IsExpImageToTempDir(string filePath, string fileName, string outName)
        {
            String namedRng = &quot;TestData&quot;;
            if (fileName == &quot;FilteredRows_New.xlsx&quot;)
            {
                namedRng = &quot;table1&quot;;
            }
            Workbook wb = new Workbook(filePath + fileName);
            Name name = wb.Worksheets.Names[namedRng];

            Aspose.Cells.Range rng = name.GetRange();
            Worksheet sheet = rng.Worksheet;
            Cells cells = sheet.Cells;
            int sheetIdx = sheet.Index;

            int firstCol = rng.FirstColumn;
            int firstRow = rng.FirstRow;
            int colCnt = rng.ColumnCount;
            int rowCnt = rng.RowCount;
            int maxCol = cells.MaxDisplayRange.ColumnCount;
            int maxRow = cells.MaxDisplayRange.RowCount;

            // Create a copy of the worksheet - such that only the copy is modified
            int newSheetIdx = wb.Worksheets.AddCopy(sheetIdx);

            // BUG NOTE:
            // The copied worksheet does NOT have the filter applied and therefore
            // the filtered (hidden) rows from the original sheet are now visible

            // redefine the ranges using the copied worksheet
            wb.Worksheets.ActiveSheetIndex = (newSheetIdx);
            sheet = wb.Worksheets[newSheetIdx];
            cells = sheet.Cells;
            rng = cells.CreateRange(firstRow, firstCol, rowCnt, colCnt);

            // Manually hide all the columns not part of the named range
            if (firstCol &gt; 0)
            {
                cells.HideColumns(0, firstCol);
            }
            if (firstCol + colCnt &lt; maxCol)
            {
                cells.HideColumns(firstCol + colCnt, maxCol + 1);
            }

            // Manually hide all the rows not part of the range
            if (firstRow &gt; 0)
            {
                cells.HideRows(0, firstRow);
            }
            if (firstRow + rowCnt &lt; maxRow)
            {
                cells.HideRows(firstRow + rowCnt, maxRow);
            }

            // Now export the copied worksheet
            HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html);
            options.Encoding = (Encoding.UTF8);
            options.HtmlCrossStringType = (HtmlCrossType.Cross);
            options.PresentationPreference = (true);
            options.ExportHiddenWorksheet = (false);
            options.ExportActiveWorksheetOnly = (true);
            options.ExportImagesAsBase64 = (true);
            options.CreateDirectory = (false);
            options.IsExpImageToTempDir = (false);
            options.HiddenColDisplayType = (HtmlHiddenColDisplayType.Remove);
            options.HiddenRowDisplayType = (HtmlHiddenRowDisplayType.Remove);

            wb.Save(CreateFolder(filePath) + outName, options);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


