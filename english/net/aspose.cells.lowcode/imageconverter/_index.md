---
title: Class ImageConverter
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.LowCode.ImageConverter class. Converter for converting template file to images
type: docs
url: /net/aspose.cells.lowcode/imageconverter/
---
## ImageConverter class

Converter for converting template file to images.

```csharp
public class ImageConverter
```

## Methods

| Name | Description |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/imageconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Converts template file to images |
| static [Process](../../aspose.cells.lowcode/imageconverter/process/#process_2)(string, string) | Converts template file to images. |
| static [Process](../../aspose.cells.lowcode/imageconverter/process/#process_1)(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeSaveOptionsProvider) | Converts template file to images |

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageConverter
    {
        public static void Process(string templatePath, string outputImagePath)
        {
            Workbook workbook = new Workbook(templatePath);
            Worksheet worksheet = workbook.Worksheets[0];
            
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true,
                ImageType = ImageType.Png
            };
            
            SheetRender render = new SheetRender(worksheet, options);
            render.ToImage(0, outputImagePath);
        }
    }

    public class LowCodeClassImageConverterDemo
    {
        public static void Run()
        {
            ImageConverter.Process("template.xlsx", "res.png");
            Console.WriteLine("Image conversion completed successfully.");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


