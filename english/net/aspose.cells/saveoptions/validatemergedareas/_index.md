---
title: SaveOptions.ValidateMergedAreas
second_title: Aspose.Cells for .NET API Reference
description: SaveOptions property. Indicates whether validate merged cells before saving the file
type: docs
url: /net/aspose.cells/saveoptions/validatemergedareas/
---
## SaveOptions.ValidateMergedAreas property

Indicates whether validate merged cells before saving the file.

```csharp
public bool ValidateMergedAreas { get; set; }
```

### Remarks

The default value is false.

### Examples

```csharp
// Called: ValidateMergedAreas = true,
public static void Property_ValidateMergedAreas()
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

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


