---
title: MarkdownSaveOptions.ImageOptions
second_title: Aspose.Cells for .NET API Reference
description: MarkdownSaveOptions property. Get the ImageOrPrintOptions object before exporting
type: docs
url: /net/aspose.cells/markdownsaveoptions/imageoptions/
---
## MarkdownSaveOptions.ImageOptions property

Get the ImageOrPrintOptions object before exporting

```csharp
public ImageOrPrintOptions ImageOptions { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class MarkdownSaveOptionsPropertyImageOptionsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Create a sample worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to make the example meaningful
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "Image Options Demo";

            try
            {
                // Create MarkdownSaveOptions instance
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Access the ImageOptions property (read-only)
                ImageOrPrintOptions imageOptions = saveOptions.ImageOptions;

                // Display the current values of ImageOptions properties
                Console.WriteLine("ImageOptions properties:");
                Console.WriteLine($"HorizontalResolution: {imageOptions.HorizontalResolution}");
                Console.WriteLine($"VerticalResolution: {imageOptions.VerticalResolution}");
                Console.WriteLine($"ImageType: {imageOptions.ImageType}");
                Console.WriteLine($"Quality: {imageOptions.Quality}");
                Console.WriteLine($"Transparent: {imageOptions.Transparent}");

                // Save the workbook with the current options
                workbook.Save("ImageOptionsDemo.md", saveOptions);

                Console.WriteLine("Markdown file saved successfully with ImageOptions demonstrated.");
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

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


