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
            worksheet.Cells["A1"].PutValue("Hello World");

            // Create an instance of XlsbSaveOptions
            XlsbSaveOptions saveOptions = new XlsbSaveOptions
            {
                CompressionType = OoxmlCompressionType.Level6,
                ExportAllColumnIndexes = true,
                ClearData = false,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };

            // Save the workbook as XLSB file with the specified options
            workbook.Save("XlsbSaveOptionsExample.xlsb", saveOptions);

            return;
        }
```

### See Also

* enum [OoxmlCompressionType](../../ooxmlcompressiontype/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


