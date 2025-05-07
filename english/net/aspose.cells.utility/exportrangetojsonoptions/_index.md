---
title: Class ExportRangeToJsonOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Utility.ExportRangeToJsonOptions class. Indicates the options that exporting range to json
type: docs
url: /net/aspose.cells.utility/exportrangetojsonoptions/
---
## ExportRangeToJsonOptions class

Indicates the options that exporting range to json.

```csharp
public class ExportRangeToJsonOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [ExportRangeToJsonOptions](exportrangetojsonoptions/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [ExportAsString](../../aspose.cells.utility/exportrangetojsonoptions/exportasstring/) { get; set; } | Exports the string value of the cells to json. |
| [ExportEmptyCells](../../aspose.cells.utility/exportrangetojsonoptions/exportemptycells/) { get; set; } | Indicates whether exporting empty cells as null. |
| [HasHeaderRow](../../aspose.cells.utility/exportrangetojsonoptions/hasheaderrow/) { get; set; } | Indicates whether the range contains header row. |
| [Indent](../../aspose.cells.utility/exportrangetojsonoptions/indent/) { get; set; } | Indicates the indent. |

### Examples

```csharp
// Called: ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
[Test]
        public void Type_ExportRangeToJsonOptions()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSAPP-445.xlsx");
            Cells cells = workbook.Worksheets[0].Cells;
            // Range range = cells.MaxDisplayRange;//if no data, return null
            int maxDataRow = cells.MaxDataColumn;
            int maxDataColumn = cells.MaxDataRow;
            if (maxDataRow >= 0 && maxDataColumn >= 0)
            {
                var range = cells.CreateRange(0, 0, maxDataRow + 1, maxDataColumn + 1);
                ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
                JsonUtility.ExportRangeToJson(range, options);
            }
        }
```

### See Also

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


