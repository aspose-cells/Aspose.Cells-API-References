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
[Test]
        public void Method_ExportRangeToJsonOptions_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSAPP-445.xlsx&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            // Range range = cells.MaxDisplayRange;//if no data, return null
            int maxDataRow = cells.MaxDataColumn;
            int maxDataColumn = cells.MaxDataRow;
            if (maxDataRow &gt;= 0 &amp;&amp; maxDataColumn &gt;= 0)
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
// Called: string ext = JsonUtility.ExportRangeToJson(range, exportOptions);
[Test]
        public void Method_JsonSaveOptions_()
        {
            Workbook wb = new Workbook();
            string str = File.ReadAllText(Constants.sourcePath + &quot;CellsNet47113.json&quot;);
            Cells cells = wb.Worksheets[0].Cells;
            JsonLayoutOptions importOptions = new JsonLayoutOptions();
            importOptions.ConvertNumericOrDate = true;
            importOptions.ArrayAsTable = true;
            JsonUtility.ImportData(str, cells, 0, 0, importOptions);
            wb.Save(Constants.destPath + &quot;CellsNet47113.csv&quot;);
            Aspose.Cells.Range range = cells.MaxDisplayRange;
            JsonSaveOptions exportOptions = new JsonSaveOptions();
            exportOptions.ExportAsString = true;
            
            string ext = JsonUtility.ExportRangeToJson(range, exportOptions);
            Assert.AreEqual(str.Replace(&quot;\r\n&quot;, &quot;\n&quot;), ext.Replace(&quot;\r\n&quot;, &quot;\n&quot;));
            TxtLoadOptions textLoadOptions = new TxtLoadOptions();
            textLoadOptions.Separator = &apos;,&apos;;


            wb = new Workbook(Constants.sourcePath + &quot;CellsNet47113.csv&quot;, textLoadOptions);
            cells = wb.Worksheets[0].Cells;
            range = cells.MaxDisplayRange;
            exportOptions = new JsonSaveOptions();
            exportOptions.ExportAsString = true;

            ext = JsonUtility.ExportRangeToJson(range, exportOptions);
            Assert.AreEqual(str.Replace(&quot;\r\n&quot;, &quot;\n&quot;), ext.Replace(&quot;\r\n&quot;, &quot;\n&quot;));
        }
```

### See Also

* class [Range](../../../aspose.cells/range/)
* class [JsonSaveOptions](../../../aspose.cells/jsonsaveoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


