---
title: XlsbSaveOptions.ExportAllColumnIndexes
second_title: Aspose.Cells for .NET API Reference
description: XlsbSaveOptions property. Indicates whether exporting all column indexes for cells
type: docs
url: /net/aspose.cells/xlsbsaveoptions/exportallcolumnindexes/
---
## XlsbSaveOptions.ExportAllColumnIndexes property

Indicates whether exporting all column indexes for cells.

```csharp
public bool ExportAllColumnIndexes { get; set; }
```

### Remarks

The default value is true.

### Examples

```csharp
// Called: ExportAllColumnIndexes = true,
public static void XlsbSaveOptions_Property_ExportAllColumnIndexes()
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

* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


