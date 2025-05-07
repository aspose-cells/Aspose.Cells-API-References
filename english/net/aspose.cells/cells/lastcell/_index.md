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
// Called: var range = cells.CreateRange(0, 0, cells.LastCell.Row + 1, cells.LastCell.Column + 1);
[Test]
        public void Property_LastCell()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET51810.xlsx");
            Cells cells = workbook.Worksheets[0].Cells;


            // create & set ExportRangeToJsonOptions for advanced options
            var exportOptions = new ExportRangeToJsonOptions();

             exportOptions.ExportEmptyCells = true;
            // create a range of cells containing data to be exported
            var range = cells.CreateRange(0, 0, cells.LastCell.Row + 1, cells.LastCell.Column + 1);
            // export range as JSON data


            string jsonData = JsonUtility.ExportRangeToJson(range, exportOptions);
            Assert.IsTrue(jsonData.IndexOf("\"Ticket Organization\": null,") != -1);
        }
```

### See Also

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


