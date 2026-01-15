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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SaveOptionsPropertySortExternalNamesDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Create a sample worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to make the example meaningful
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Create OoxmlSaveOptions instance which inherits from SaveOptions
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

                // Display the default value of SortExternalNames property
                Console.WriteLine("Default SortExternalNames value: " + saveOptions.SortExternalNames);

                // Set SortExternalNames to true
                saveOptions.SortExternalNames = true;
                Console.WriteLine("SortExternalNames set to: " + saveOptions.SortExternalNames);

                // Save the workbook with the specified save options
                workbook.Save("SortExternalNamesDemo.xlsx", saveOptions);

                Console.WriteLine("Workbook saved with SortExternalNames enabled.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


