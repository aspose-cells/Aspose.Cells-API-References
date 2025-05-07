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
// Called: var jsonData = JsonUtility.ExportRangeToJson(range, exportOptions);
[Test]
        public void Method_ExportRangeToJsonOptions_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSAPP-367.xlsx");
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
// Called: string ext = JsonUtility.ExportRangeToJson(range, exportOptions);
[Test]
        public void Method_JsonSaveOptions_()
        {
            Workbook wb = new Workbook();
            string str = File.ReadAllText(Constants.sourcePath + "CellsNet47113.json");
            Cells cells = wb.Worksheets[0].Cells;
            JsonLayoutOptions importOptions = new JsonLayoutOptions();
            importOptions.ConvertNumericOrDate = true;
            importOptions.ArrayAsTable = true;
            JsonUtility.ImportData(str, cells, 0, 0, importOptions);
            wb.Save(Constants.destPath + "CellsNet47113.csv");
            Aspose.Cells.Range range = cells.MaxDisplayRange;
            JsonSaveOptions exportOptions = new JsonSaveOptions();
            exportOptions.ExportAsString = true;
            
            string ext = JsonUtility.ExportRangeToJson(range, exportOptions);
            Assert.AreEqual(str.Replace("\r\n", "\n"), ext.Replace("\r\n", "\n"));
            TxtLoadOptions textLoadOptions = new TxtLoadOptions();
            textLoadOptions.Separator = ',';


            wb = new Workbook(Constants.sourcePath + "CellsNet47113.csv", textLoadOptions);
            cells = wb.Worksheets[0].Cells;
            range = cells.MaxDisplayRange;
            exportOptions = new JsonSaveOptions();
            exportOptions.ExportAsString = true;

            ext = JsonUtility.ExportRangeToJson(range, exportOptions);
            Assert.AreEqual(str.Replace("\r\n", "\n"), ext.Replace("\r\n", "\n"));
        }
```

### See Also

* class [Range](../../../aspose.cells/range/)
* class [JsonSaveOptions](../../../aspose.cells/jsonsaveoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


