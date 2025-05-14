---
title: Cells.LastCell
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the last cell in this worksheet
type: docs
url: /net/aspose.cells/cells/lastcell/
---
## Cells.LastCell property

Gets the last cell in this worksheet.

```csharp
public Cell LastCell { get; }
```

### Remarks

Returns null if there is no data in the worksheet.

### Examples

```csharp
// Called: var dataSheetDataRange = dataSheet.Cells.CreateRange(dataSheet.Cells.FirstCell.Name, dataSheet.Cells.LastCell.Name);
private static void Cells_Property_LastCell(Workbook workbook, List<string> columns)
        {
            var dataSheet = workbook.Worksheets.GetSheetByCodeName("Sheet1");
            for (int i = 0; i < columns.Count; ++i)
            {
                dataSheet.Cells[0, i].Value = columns[i];
                var sampleDataCell = dataSheet.Cells[1, i];
                sampleDataCell.Value = "Sample value";
            }
            var dataSheetDataRange = dataSheet.Cells.CreateRange(dataSheet.Cells.FirstCell.Name, dataSheet.Cells.LastCell.Name);
            dataSheetDataRange.Name = "Data0";
        }
```

### See Also

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


