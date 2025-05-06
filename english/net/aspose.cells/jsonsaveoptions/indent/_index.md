---
title: JsonSaveOptions.Indent
second_title: Aspose.Cells for .NET API Reference
description: JsonSaveOptions property. Indicates the indent
type: docs
url: /net/aspose.cells/jsonsaveoptions/indent/
---
## JsonSaveOptions.Indent property

Indicates the indent.

```csharp
public string Indent { get; set; }
```

### Remarks

If the indent is null or empty, the exported json is not formatted.

### Examples

```csharp
// Called: Indent = &amp;quot;  &amp;quot;,
public static void Property_Indent()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fill some data into the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Name&quot;);
            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Age&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;John&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(30);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;Jane&quot;);
            worksheet.Cells[&quot;B3&quot;].PutValue(25);

            // Create an instance of JsonSaveOptions
            JsonSaveOptions saveOptions = new JsonSaveOptions
            {
                ExportHyperlinkType = JsonExportHyperlinkType.DisplayString,
                SkipEmptyRows = true,
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 },
                HasHeaderRow = true,
                ExportAsString = true,
                Indent = &quot;  &quot;,
                ExportNestedStructure = false,
                ExportEmptyCells = false,
                AlwaysExportAsJsonObject = false,
                ToExcelStruct = false,
                ClearData = false,
                CachedFileFolder = &quot;C:\\Temp&quot;,
                ValidateMergedAreas = true,
                MergeAreas = false,
                SortNames = false,
                SortExternalNames = false,
                RefreshChartCache = false,
                UpdateSmartArt = false
            };

            // Save the workbook as a JSON file
            workbook.Save(&quot;JsonSaveOptionsExample.json&quot;, saveOptions);

            return;
        }
```

### See Also

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


