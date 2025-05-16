---
title: ImageOrPrintOptions.GridlineColor
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Gets or sets gridline colr
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/gridlinecolor/
---
## ImageOrPrintOptions.GridlineColor property

Gets or sets gridline colr.

```csharp
public Color GridlineColor { get; set; }
```

### Remarks

It will ignore the gridline color settings in the source file.

### Examples

```csharp
namespace AsposeCellsExamples.ImageOrPrintOptionsPropertyGridlineColorDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing; // Added for ImageType
    using System;
    using System.Drawing;

    public class ImageOrPrintOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Create a new workbook and access the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to make gridlines visible
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.99);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(1.99);

            // Enable gridlines in the worksheet
            worksheet.IsGridlinesVisible = true;

            // Create ImageOrPrintOptions instance
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Display current gridline color from worksheet
            Console.WriteLine("Current GridlineColor: " + worksheet.GridlineColor);

            // Set new gridline color to red on the worksheet
            worksheet.GridlineColor = Color.Red;
            options.ImageType = ImageType.Png;

            // Create sheet render with configured options
            SheetRender sheetRender = new SheetRender(worksheet, options);

            // Save rendered image with modified gridlines
            sheetRender.ToImage(0, "GridlineColorDemo.png");

            Console.WriteLine("Demo executed successfully. Check output image.");
        }
    }
}
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


