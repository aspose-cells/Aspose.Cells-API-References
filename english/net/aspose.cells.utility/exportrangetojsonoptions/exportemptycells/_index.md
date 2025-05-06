---
title: ExportRangeToJsonOptions.ExportEmptyCells
second_title: Aspose.Cells for .NET API Reference
description: ExportRangeToJsonOptions property. Indicates whether exporting empty cells as null
type: docs
url: /net/aspose.cells.utility/exportrangetojsonoptions/exportemptycells/
---
## ExportRangeToJsonOptions.ExportEmptyCells property

Indicates whether exporting empty cells as null.

```csharp
public bool ExportEmptyCells { get; set; }
```

### Examples

```csharp
// Called: exportOptions.ExportEmptyCells = true;
[Test]
        public void Property_ExportEmptyCells()
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

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


