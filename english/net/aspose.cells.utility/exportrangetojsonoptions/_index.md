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
public void Utility_Type_ExportRangeToJsonOptions()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet worksheet = workbook.Worksheets[0];
    var exportOptions = new ExportRangeToJsonOptions();
    var jObject = new JObject();
    var cells = worksheet.Cells;
    var range = cells.CreateRange(0, 0, cells.LastCell.Row + 1, cells.LastCell.Column + 1);

    var jsonData = JsonUtility.ExportRangeToJson(range, exportOptions);
    File.WriteAllText(Constants.destPath + "CELLSAPP367.txt", jsonData);
    jObject.Add(worksheet.Name, JArray.Parse(jsonData));
}
```

### See Also

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


