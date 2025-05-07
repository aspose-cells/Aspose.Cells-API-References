---
title: DifSaveOptions.DifSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: DifSaveOptions constructor. Creates the options for saving DIF file
type: docs
url: /net/aspose.cells/difsaveoptions/difsaveoptions/
---
## DifSaveOptions constructor

Creates the options for saving DIF file.

```csharp
public DifSaveOptions()
```

### Examples

```csharp
// Called: DifSaveOptions saveOptions = new DifSaveOptions
[Test]
        public void DifSaveOptions_Constructor()
        {
            Workbook workbook = new Workbook();

            // Add some data to the worksheet for demonstration purposes
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Sample Data");

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
            workbook.Save("DifSaveOptionsExample.dif", saveOptions);
        }
```

### See Also

* class [DifSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


