---
title: Column.Width
second_title: Aspose.Cells for .NET API Reference
description: Column property. Gets and sets the column width in unit of characters
type: docs
url: /net/aspose.cells/column/width/
---
## Column.Width property

Gets and sets the column width in unit of characters.

```csharp
public double Width { get; set; }
```

### Remarks

For spreadsheet, column width is measured as the number of characters of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.

### Examples

```csharp
// Called: sheet.Cells.Columns[0].Width = 4.75;
protected static void Property_Width(Workbook book)
        {
            for (int i = 0; i < book.Worksheets.Count; i++)
            {
                Worksheet sheet = book.Worksheets[i];
                StyleFlag styleFlagGrid = new StyleFlag();
                styleFlagGrid.Borders = true;
                sheet.Cells.InsertColumn(0);
                sheet.Cells.InsertRow(0);

                sheet.Cells.Rows[0].Height = 15.75;
                sheet.Cells.Columns[0].Width = 4.75;

                int maxRow =
                    // sheet.getCells().getMaxRow();
                sheet.Cells.MaxDisplayRange.RowCount;
                int maxCol =
                    // sheet.getCells().getMaxColumn();
                sheet.Cells.MaxDisplayRange.ColumnCount;

                for (int j = 1; j < maxRow; j++)
                {
                    sheet.Cells[j, 0].PutValue(j);
                }
                for (int k = 1; k < maxCol; k++)
                {
                    sheet.Cells[0, k].PutValue(CellsHelper.ColumnIndexToName(k - 1));
                }
            }
        }
```

### See Also

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


