---
title: MarkdownSaveOptions.ExportImagesAsBase64
second_title: Aspose.Cells for .NET API Reference
description: MarkdownSaveOptions property. Specifies whether images are saved in Base64 format to Markdown. The default value is true
type: docs
url: /net/aspose.cells/markdownsaveoptions/exportimagesasbase64/
---
## MarkdownSaveOptions.ExportImagesAsBase64 property

Specifies whether images are saved in Base64 format to Markdown. The default value is true.

```csharp
public bool ExportImagesAsBase64 { get; set; }
```

### Remarks

When this property is set to true image data is exported directly on the img elements and separate files are not created.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyExportImagesAsBase64Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data and an image
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("With Image");

            // Add an image to the worksheet
            int imageIndex = worksheet.Pictures.Add(1, 1, "sample.png");

            try
            {
                // Create MarkdownSaveOptions instance
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Display the default value of ExportImagesAsBase64
                Console.WriteLine("Default ExportImagesAsBase64 value: " + saveOptions.ExportImagesAsBase64);

                // Set ExportImagesAsBase64 to false to demonstrate the property
                saveOptions.ExportImagesAsBase64 = false;
                Console.WriteLine("ExportImagesAsBase64 set to: " + saveOptions.ExportImagesAsBase64);

                // Save with ExportImagesAsBase64 = false
                workbook.Save("MarkdownImagesAsFiles.md", saveOptions);

                // Set ExportImagesAsBase64 to true
                saveOptions.ExportImagesAsBase64 = true;
                Console.WriteLine("ExportImagesAsBase64 set to: " + saveOptions.ExportImagesAsBase64);

                // Save with ExportImagesAsBase64 = true
                workbook.Save("MarkdownImagesAsBase64.md", saveOptions);

                Console.WriteLine("Markdown files saved with different ExportImagesAsBase64 settings.");
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

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


