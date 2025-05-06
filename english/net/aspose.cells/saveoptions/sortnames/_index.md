---
title: SaveOptions.SortNames
second_title: Aspose.Cells for .NET API Reference
description: SaveOptions property. Indicates whether sorting defined names before saving file
type: docs
url: /net/aspose.cells/saveoptions/sortnames/
---
## SaveOptions.SortNames property

Indicates whether sorting defined names before saving file.

```csharp
public bool SortNames { get; set; }
```

### Examples

```csharp
// Called: SortNames = true,
public static void Property_SortNames()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Hello World&quot;);

            // Create an instance of XlsbSaveOptions
            XlsbSaveOptions saveOptions = new XlsbSaveOptions
            {
                CompressionType = OoxmlCompressionType.Level6,
                ExportAllColumnIndexes = true,
                ClearData = false,
                CachedFileFolder = &quot;C:\\Temp&quot;,
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };

            // Save the workbook as XLSB file with the specified options
            workbook.Save(&quot;XlsbSaveOptionsExample.xlsb&quot;, saveOptions);

            return;
        }
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


