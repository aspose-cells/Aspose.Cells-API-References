---
title: PasteOptions.SkipBlanks
second_title: Aspose.Cells for .NET API Reference
description: PasteOptions property. Indicates whether skips blank cells
type: docs
url: /net/aspose.cells/pasteoptions/skipblanks/
---
## PasteOptions.SkipBlanks property

Indicates whether skips blank cells.

```csharp
public bool SkipBlanks { get; set; }
```

### Examples

```csharp
// Called: destinationRange.Copy(range, new PasteOptions { SkipBlanks = false, PasteType = PasteType.All });
public void PasteOptions_Property_SkipBlanks()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Aspose.Cells.Range range = wb.Worksheets.GetRangeByName("ABC");
    Workbook workbook = new Workbook();
    Worksheet worksheet = workbook.Worksheets[0];
    Aspose.Cells.Range destinationRange = worksheet.Cells.CreateRange(0, 0, range.RowCount, range.ColumnCount);
    destinationRange.CopyData(range);
    destinationRange.Copy(range, new PasteOptions { SkipBlanks = false, PasteType = PasteType.All });
    destinationRange.CopyStyle(range);

    for (int i = 0; i < destinationRange.RowCount; i++)
    {
        for (int j = 0; j < destinationRange.ColumnCount; j++)
        {
            Cell cell = worksheet.Cells[i, j];
            if (!cell.IsFormula)
            {
                continue;
            }
            object cellValue = cell.Value;
            cell.PutValue(cellValue); //Index out of bound exception
        }
    }
}
```

### See Also

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


