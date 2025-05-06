---
title: JsonSaveOptions.ExportArea
second_title: Aspose.Cells for .NET API Reference
description: JsonSaveOptions property. Gets or sets the exporting range
type: docs
url: /net/aspose.cells/jsonsaveoptions/exportarea/
---
## JsonSaveOptions.ExportArea property

Gets or sets the exporting range.

```csharp
public CellArea ExportArea { get; set; }
```

### Examples

```csharp
// Called: ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 },
public static void Property_ExportArea()
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

* struct [CellArea](../../cellarea/)
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


