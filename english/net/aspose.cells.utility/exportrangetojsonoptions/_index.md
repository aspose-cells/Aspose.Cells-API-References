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
// Called: var exportOptions = new ExportRangeToJsonOptions();
[Test]
        public void Type_ExportRangeToJsonOptions()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET51810.xlsx&quot;);
            Cells cells = workbook.Worksheets[0].Cells;


            // create &amp; set ExportRangeToJsonOptions for advanced options
            var exportOptions = new ExportRangeToJsonOptions();

             exportOptions.ExportEmptyCells = true;
            // create a range of cells containing data to be exported
            var range = cells.CreateRange(0, 0, cells.LastCell.Row + 1, cells.LastCell.Column + 1);
            // export range as JSON data


            string jsonData = JsonUtility.ExportRangeToJson(range, exportOptions);
            Assert.IsTrue(jsonData.IndexOf(&quot;\&quot;Ticket Organization\&quot;: null,&quot;) != -1);
        }
```

### See Also

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


