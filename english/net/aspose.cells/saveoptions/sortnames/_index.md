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
public static void SaveOptions_Property_SortNames()
        {
            // Create a new Workbook object
            Workbook workbook = new Workbook();
            
            // Add some data to the worksheet for demonstration purposes
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Sample Data");

            // Create an instance of DifSaveOptions
            DifSaveOptions saveOptions = new DifSaveOptions
            {
                // Set properties as per the JSON specification
                ClearData = true,
                CachedFileFolder = @"C:\Temp\CachedFiles",
                ValidateMergedAreas = true,
                MergeAreas = false,
                CreateDirectory = true,
                SortNames = true,
                SortExternalNames = false,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };


            // Save the workbook with the DifSaveOptions
            workbook.Save("E:\\VSCellsForm\\DifSaveOptionsExample.dif", saveOptions);

            // Output to console to indicate the process is complete
            Console.WriteLine("Workbook saved successfully with DifSaveOptions.");
        }
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


