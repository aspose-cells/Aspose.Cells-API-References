---
title: JsonSaveOptions.HasHeaderRow
second_title: Aspose.Cells for .NET API Reference
description: JsonSaveOptions property. Indicates whether the range contains header row
type: docs
url: /net/aspose.cells/jsonsaveoptions/hasheaderrow/
---
## JsonSaveOptions.HasHeaderRow property

Indicates whether the range contains header row.

```csharp
public bool HasHeaderRow { get; set; }
```

### Examples

```csharp
// Called: options.HasHeaderRow = false;
public void JsonSaveOptions_Property_HasHeaderRow()
{
    Workbook workbook = new Aspose.Cells.Workbook(Constants.sourcePath + "example.xlsx");


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


