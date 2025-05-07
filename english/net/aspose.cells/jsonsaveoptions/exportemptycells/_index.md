---
title: JsonSaveOptions.ExportEmptyCells
second_title: Aspose.Cells for .NET API Reference
description: JsonSaveOptions property. Indicates whether exporting empty cells as null
type: docs
url: /net/aspose.cells/jsonsaveoptions/exportemptycells/
---
## JsonSaveOptions.ExportEmptyCells property

Indicates whether exporting empty cells as null.

```csharp
public bool ExportEmptyCells { get; set; }
```

### Examples

```csharp
// Called: options.ExportEmptyCells = true;
[Test]
        public void Property_ExportEmptyCells()
        {
            Workbook workbook = new Aspose.Cells.Workbook(Constants.sourcePath + "CELLSNET55308.xlsx");


            int firstRow = 0;
            int firstCol = 0;
            int lastRow = 3;
            int lastCol = 2;

            // Calculate Total Rows / Columns 
            int totalRows = lastRow - firstRow;
            int totalCols = lastCol - firstCol;

            Aspose.Cells.JsonSaveOptions options = new Aspose.Cells.JsonSaveOptions();
            options.ExportEmptyCells = true;
            options.HasHeaderRow = false;
            options.ExportNestedStructure = false;

            Worksheet worksheet = workbook.Worksheets[0];

            Aspose.Cells.Range range = worksheet.Cells.CreateRange(firstRow, firstCol, totalRows, totalCols);
            string output = Aspose.Cells.Utility.JsonUtility.ExportRangeToJson(range, options);
           Assert.IsTrue(output.IndexOf("{") == -1);
        }
```

### See Also

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


