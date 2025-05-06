---
title: XlsbSaveOptions.CompressionType
second_title: Aspose.Cells for .NET API Reference
description: XlsbSaveOptions property. Gets and sets the compression type for ooxml file
type: docs
url: /net/aspose.cells/xlsbsaveoptions/compressiontype/
---
## XlsbSaveOptions.CompressionType property

Gets and sets the compression type for ooxml file.

```csharp
public OoxmlCompressionType CompressionType { get; set; }
```

### Remarks

The default value is OoxmlCompressionType.Level6.

### Examples

```csharp
// Called: CompressionType = OoxmlCompressionType.Level6,
public static void Property_CompressionType()
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

* enum [OoxmlCompressionType](../../ooxmlcompressiontype/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


