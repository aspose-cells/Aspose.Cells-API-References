---
title: Cells.HideColumns
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Hide multiple columns
type: docs
url: /net/aspose.cells/cells/hidecolumns/
---
## Cells.HideColumns method

Hide multiple columns.

```csharp
public void HideColumns(int column, int totalColumns)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index. |
| totalColumns | Int32 | Column number. |

### Examples

```csharp
// Called: cells.HideColumns(firstCol + rng.ColumnCount, maxCol);
private static void Method_Int32_(String xlFile, String xlRange, String outFile)
        {
            try
            {
                Workbook wb = new Workbook(xlFile);
                NameCollection names = wb.Worksheets.Names;
                Name name = names[xlRange];

                Aspose.Cells.Range rng = name.GetRange();
                Worksheet sheet = rng.Worksheet;
                Cells cells = sheet.Cells;
                int firstCol = rng.FirstColumn;
                int firstRow = rng.FirstRow;
                int maxCol = cells.MaxDisplayRange.ColumnCount;
                int maxRow = cells.MaxDisplayRange.RowCount;

                // hide all the rows and columns that are not part of the range
                if (firstCol > 0)
                {
                    cells.HideColumns(0, firstCol - 1);
                }
                if (firstCol + rng.ColumnCount < maxCol)
                {
                    cells.HideColumns(firstCol + rng.ColumnCount, maxCol);
                }
                if (firstRow > 0)
                {
                    cells.HideRows(0, firstRow - 1);
                }
                if (firstRow + rng.RowCount < maxRow)
                {
                    cells.HideRows(firstRow + rng.RowCount, maxRow);
                }

                wb.Worksheets.ActiveSheetIndex = sheet.Index;

                // export the worksheet
                HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html);
                options.Encoding = Encoding.UTF8;
                options.HtmlCrossStringType = HtmlCrossType.Cross;
                options.PresentationPreference = true;
                options.ExportHiddenWorksheet = false;
                options.ExportActiveWorksheetOnly = true;
                options.ExportImagesAsBase64 = true;// aovids the temp folder
                options.CreateDirectory = false;
                options.IsExpImageToTempDir = false;
                options.HiddenColDisplayType = HtmlHiddenColDisplayType.Remove;
                options.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove;

                wb.Save(outFile, options);

            }
            catch (Exception ex)
            {
                Console.WriteLine("Unexpected exception: " + ex.Message);
            }
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


