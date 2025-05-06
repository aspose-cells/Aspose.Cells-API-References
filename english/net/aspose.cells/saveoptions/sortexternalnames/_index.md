---
title: SaveOptions.SortExternalNames
second_title: Aspose.Cells for .NET API Reference
description: SaveOptions property. Indicates whether sorting external defined names before saving file
type: docs
url: /net/aspose.cells/saveoptions/sortexternalnames/
---
## SaveOptions.SortExternalNames property

Indicates whether sorting external defined names before saving file.

```csharp
public bool SortExternalNames { get; set; }
```

### Examples

```csharp
// Called: SortExternalNames = false,
[Test]
        public void Property_SortExternalNames()
        {
            Workbook workbook = new Workbook();

            // Add some data to the worksheet for demonstration purposes
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue(&quot;Sample Data&quot;);

            // Create an instance of DifSaveOptions
            DifSaveOptions saveOptions = new DifSaveOptions
            {
                // Set properties as per the JSON specification
                ClearData = true,
                ValidateMergedAreas = true,
                MergeAreas = false,
                CreateDirectory = true,
                SortNames = true,
                SortExternalNames = false,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };


            // Save the workbook with the DifSaveOptions
            workbook.Save(&quot;DifSaveOptionsExample.dif&quot;, saveOptions);
        }
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


