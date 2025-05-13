---
title: JsonUtility.ExportRangeToJson
second_title: Aspose.Cells for .NET API Reference
description: JsonUtility method. Exporting the range to json file
type: docs
url: /net/aspose.cells.utility/jsonutility/exportrangetojson/
---
## ExportRangeToJson(Range, ExportRangeToJsonOptions) {#exportrangetojson_1}

Exporting the range to json file.

```csharp
[Obsolete("Use ExportRangeToJson(Range range, JsonSaveOptions options) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ExportRangeToJson(Range range, ExportRangeToJsonOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The range. |
| options | ExportRangeToJsonOptions | The options of exporting. |

### Return Value

The json string value.

### Remarks

NOTE: This member is now obsolete. Instead, please use ExportRangeToJson(Range range, JsonSaveOptions options) method. This property will be removed 6 months later since November 2022. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: JsonUtility.ExportRangeToJson(range, options);
public void JsonUtility_Method_ExportRangeToJson()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
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

* class [Range](../../../aspose.cells/range/)
* class [ExportRangeToJsonOptions](../../exportrangetojsonoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)

---

## ExportRangeToJson(Range, JsonSaveOptions) {#exportrangetojson}

Exporting the range to json file.

```csharp
public static string ExportRangeToJson(Range range, JsonSaveOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The range. |
| options | JsonSaveOptions | The options of exporting. |

### Return Value

The json string value.

### Examples

```csharp
// Called: string output = Aspose.Cells.Utility.JsonUtility.ExportRangeToJson(range, options);
public void JsonUtility_Method_ExportRangeToJson()
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

* class [Range](../../../aspose.cells/range/)
* class [JsonSaveOptions](../../../aspose.cells/jsonsaveoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


