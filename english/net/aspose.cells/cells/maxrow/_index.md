---
title: Cells.MaxRow
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Maximum row index of cell which contains data or style
type: docs
url: /net/aspose.cells/cells/maxrow/
---
## Cells.MaxRow property

Maximum row index of cell which contains data or style.

```csharp
public int MaxRow { get; }
```

### Remarks

Return -1 if there is no cell which contains data or style in the worksheet.

### Examples

```csharp
// Called: int maxRow = cells.MaxRow;
[Test]
        public void Property_MaxRow()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA40148.xls");
            Cells cells = workbook.Worksheets[0].Cells;
            int maxRow = cells.MaxRow;
            int maxColumn = cells.MaxColumn;
            for (int i = 0; i < maxRow; i++)
            {
                for (int j = 0; j < maxColumn; j++)
                {
                    Style style = cells[i, j].GetDisplayStyle();
                }

            }
            workbook.FileFormat = FileFormatType.Xlsx;
            for (int i = 0; i < maxRow; i++)
            {
                for (int j = 0; j < maxColumn; j++)
                {
                    Style style = cells[i, j].GetDisplayStyle();
                }

            }
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


