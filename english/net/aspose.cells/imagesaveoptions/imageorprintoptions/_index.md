---
title: ImageSaveOptions.ImageOrPrintOptions
second_title: Aspose.Cells for .NET API Reference
description: ImageSaveOptions property. Additional image creation options
type: docs
url: /net/aspose.cells/imagesaveoptions/imageorprintoptions/
---
## ImageSaveOptions.ImageOrPrintOptions property

Additional image creation options.

```csharp
public ImageOrPrintOptions ImageOrPrintOptions { get; }
```

### Remarks

For advanced usage, please use [`WorkbookRender`](../../../aspose.cells.rendering/workbookrender/) or [`SheetRender`](../../../aspose.cells.rendering/sheetrender/).

### Examples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImageSaveOptionsPropertyImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Image Export");

            ImageSaveOptions pngOptions = new ImageSaveOptions(SaveFormat.Png);
            pngOptions.ImageOrPrintOptions.OnePagePerSheet = true;
            pngOptions.ImageOrPrintOptions.AllColumnsInOnePagePerSheet = true;

            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, pngOptions);
                Console.WriteLine("Image saved to memory stream successfully");
            }
        }
    }
}
```

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


