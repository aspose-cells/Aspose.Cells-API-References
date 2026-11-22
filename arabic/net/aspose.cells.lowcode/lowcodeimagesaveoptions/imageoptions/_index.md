---
title: "LowCodeImageSaveOptions.ImageOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeImageSaveOptions. الخيارات لتصيير الصور"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodeimagesaveoptions/imageoptions/
---
## LowCodeImageSaveOptions.ImageOptions property

الخيارات الخاصة بتصيير الصور.

```csharp
public ImageOrPrintOptions ImageOptions { get; set; }
```

### ملاحظات

عند تحديد كائن واحد من [`ImageOrPrintOptions`](../../../aspose.cells.rendering/imageorprintoptions/)، سيتم استبدال [`SaveFormat`](../saveformat/) (إذا كان قد تم تحديده مسبقًا).

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeImageSaveOptionsPropertyImageOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Image Output");

            LowCodeImageSaveOptions saveOptions = new LowCodeImageSaveOptions();
            saveOptions.ImageOptions = new ImageOrPrintOptions();

            Console.WriteLine("Default Horizontal Resolution: " + saveOptions.ImageOptions.HorizontalResolution);
            
            saveOptions.ImageOptions.HorizontalResolution = 300;
            saveOptions.ImageOptions.VerticalResolution = 300;
            SheetRender highResRenderer = new SheetRender(worksheet, saveOptions.ImageOptions);
            highResRenderer.ToImage(0, "HighResolutionOutput.png");

            saveOptions.ImageOptions.HorizontalResolution = 150;
            saveOptions.ImageOptions.VerticalResolution = 150;
            SheetRender lowResRenderer = new SheetRender(worksheet, saveOptions.ImageOptions);
            lowResRenderer.ToImage(0, "LowResolutionOutput.png");
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


