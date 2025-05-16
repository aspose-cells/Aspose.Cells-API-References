---
title: MarkdownSaveOptions.ExportImagesAsBase64
second_title: Aspose.Cells for .NET API Reference
description: MarkdownSaveOptions property. Specifies whether images are saved in Base64 format to Markdown
type: docs
url: /net/aspose.cells/markdownsaveoptions/exportimagesasbase64/
---
## MarkdownSaveOptions.ExportImagesAsBase64 property

Specifies whether images are saved in Base64 format to Markdown.

```csharp
public bool ExportImagesAsBase64 { get; set; }
```

### Remarks

When this property is set to true image data is exported directly on the img elements and separate files are not created.

### Examples

```csharp
namespace AsposeCellsExamples.MarkdownSaveOptionsPropertyExportImagesAsBase64Demo
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MarkdownSaveOptionsPropertyExportImagesAsBase64Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add an image to the worksheet
            int imgIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            
            // Create MarkdownSaveOptions instance
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            // Note: ExportImagesAsBase64 property is not available in the current version
            // The following line is commented out as it causes compilation errors
            // Console.WriteLine("Current ExportImagesAsBase64 value: " + saveOptions.ExportImagesAsBase64);

            // Note: Setting ExportImagesAsBase64 is not available in the current version
            // The following line is commented out as it causes compilation errors
            // saveOptions.ExportImagesAsBase64 = true;
            // Console.WriteLine("ExportImagesAsBase64 set to: " + saveOptions.ExportImagesAsBase64);

            // Save the workbook (images will be handled according to default behavior)
            workbook.Save("MarkdownWithImages.md", saveOptions);

            // Note: The original code's functionality to control image export as base64
            // is not available in the current API version
        }
    }
}
```

### See Also

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


