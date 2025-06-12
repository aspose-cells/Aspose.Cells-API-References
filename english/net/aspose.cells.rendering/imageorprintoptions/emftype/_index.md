---
title: ImageOrPrintOptions.EmfType
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Gets or sets an EmfType that specifies the format of the Metafile.. The default value is EmfPlusDual
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/emftype/
---
## ImageOrPrintOptions.EmfType property

Gets or sets an EmfType that specifies the format of the Metafile.. The default value is EmfPlusDual.

```csharp
public EmfType EmfType { get; set; }
```

### Examples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyEmfTypeDemo
    {
        public static void Run()
        {
            // Create a workbook and add test data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("EMF Type Demonstration");

            // Initialize image options for EMF output
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Emf;
            options.OnlyArea = true;

            // First render with default EmfType
            MemoryStream stream1 = new MemoryStream();
            SheetRender renderer1 = new SheetRender(worksheet, options);
            renderer1.ToImage(0, stream1);
            Console.WriteLine($"Default EMF size: {stream1.Length} bytes");

            // Second render with EmfOnly type
            options.EmfRenderSetting = EmfRenderSetting.EmfOnly;
            MemoryStream stream2 = new MemoryStream();
            SheetRender renderer2 = new SheetRender(worksheet, options);
            renderer2.ToImage(0, stream2);
            Console.WriteLine($"EMF-only size: {stream2.Length} bytes");

            // Clean up
            stream1.Dispose();
            stream2.Dispose();
        }
    }
}
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


