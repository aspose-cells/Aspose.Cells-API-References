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
// Called: row = cells.MaxRow + 1;
public static void Cells_Property_MaxRow(string folderName, string fileName, string caseName, string message)
        {
            string filePath = Constants.destPath + "AsposeCellsResult.xls";
            Workbook workbook = new Workbook();
            workbook = new Workbook(filePath);
            Cells cells = workbook.Worksheets[0].Cells;
            row = cells.MaxRow + 1;
            cells[row, 0].PutValue(folderName);
            cells[row, 1].PutValue(fileName);
            cells[row, 2].PutValue(caseName);
            cells[row, 3].PutValue(message);
            workbook.Save(filePath);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


