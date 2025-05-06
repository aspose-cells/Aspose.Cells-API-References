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
// Called: saveOptions.ValidateMergedAreas = true;
public static void Property_ValidateMergedAreas()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fill some data into the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Hello&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;World&quot;);

            // Create an instance of OoxmlSaveOptions
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

            // Setting properties
            saveOptions.ExportCellName = true;
            saveOptions.UpdateZoom = true;
            saveOptions.EnableZip64 = false;
            saveOptions.EmbedOoxmlAsOleObject = false;
            saveOptions.CompressionType = OoxmlCompressionType.Level6;
            saveOptions.ClearData = false;
            saveOptions.CachedFileFolder = &quot;C:\\Temp&quot;;
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = false;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = false;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Save the workbook with the specified options
            workbook.Save(&quot;OoxmlSaveOptionsExample.xlsx&quot;, saveOptions);

            return;
        }
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


