---
title: PaginatedSaveOptions.CustomRenderSettings
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. Gets or sets custom settings during rendering
type: docs
url: /net/aspose.cells/paginatedsaveoptions/customrendersettings/
---
## PaginatedSaveOptions.CustomRenderSettings property

Gets or sets custom settings during rendering.

```csharp
public CustomRenderSettings CustomRenderSettings { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PaginatedSaveOptionsPropertyCustomRenderSettingsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";
            worksheet.Cells["A2"].Value = "This demonstrates CustomRenderSettings property";

            try
            {
                // Create PdfSaveOptions which inherits from PaginatedSaveOptions
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // Get the current CustomRenderSettings value
                CustomRenderSettings currentSettings = saveOptions.CustomRenderSettings;
                Console.WriteLine("Current CustomRenderSettings: " +
                    (currentSettings == null ? "null" : "CustomRenderSettings instance"));

                // Create and set new CustomRenderSettings
                CustomRenderSettings newSettings = new CustomRenderSettings();
                saveOptions.CustomRenderSettings = newSettings;

                // Verify the new settings were applied
                Console.WriteLine("New CustomRenderSettings set: " +
                    (saveOptions.CustomRenderSettings == newSettings ? "Success" : "Failed"));

                // Save the workbook with the custom render settings
                workbook.Save("CustomRenderSettingsDemo.pdf", saveOptions);
                Console.WriteLine("Workbook saved with CustomRenderSettings");
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

* class [CustomRenderSettings](../../../aspose.cells.rendering/customrendersettings/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


