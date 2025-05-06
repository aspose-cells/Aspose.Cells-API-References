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
public static void DifSaveOptions_Constructor()
        {
            // Create a new Workbook object
            Workbook workbook = new Workbook();
            
            // Add some data to the worksheet for demonstration purposes
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue(&quot;Sample Data&quot;);

            // Create an instance of DifSaveOptions
            DifSaveOptions saveOptions = new DifSaveOptions
            {
                // Set properties as per the JSON specification
                ClearData = true,
                CachedFileFolder = @&quot;C:\Temp\CachedFiles&quot;,
                ValidateMergedAreas = true,
                MergeAreas = false,
                CreateDirectory = true,
                SortNames = true,
                SortExternalNames = false,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };


            // Save the workbook with the DifSaveOptions
            workbook.Save(&quot;E:\\VSCellsForm\\DifSaveOptionsExample.dif&quot;, saveOptions);

            // Output to console to indicate the process is complete
            Console.WriteLine(&quot;Workbook saved successfully with DifSaveOptions.&quot;);
        }
```

### See Also

* class [DifSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


