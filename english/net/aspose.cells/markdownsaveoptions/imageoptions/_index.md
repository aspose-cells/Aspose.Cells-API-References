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
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class MarkdownSaveOptionsPropertyImageOptionsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data and an image to the worksheet
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(800);

            // Add an image to the worksheet
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpg");
            Picture pic = worksheet.Pictures[imgIndex];

            // Create MarkdownSaveOptions instance
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            // Create and configure image options
            SvgImageOptions imageOptions = new SvgImageOptions();
            imageOptions.HorizontalResolution = 300;
            imageOptions.VerticalResolution = 300;
            imageOptions.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;

            // Save the workbook with markdown options
            string outputPath = "MarkdownWithImages.md";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("Markdown document with images saved successfully.");
            Console.WriteLine("Image options used: " + imageOptions.ToString());
        }
    }
}
```

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


