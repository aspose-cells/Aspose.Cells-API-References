---
title: "ImageSaveOptions.ImageOrPrintOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageSaveOptions. خيارات إضافية لإنشاء الصور"
type: docs
url: /ar/net/aspose.cells/imagesaveoptions/imageorprintoptions/
---
## ImageSaveOptions.ImageOrPrintOptions property

خيارات إضافية لإنشاء الصورة.

```csharp
public ImageOrPrintOptions ImageOrPrintOptions { get; }
```

### ملاحظات

للاستخدام المتقدم، يرجى استخدام [`WorkbookRender`](../../../aspose.cells.rendering/workbookrender/) أو [`SheetRender`](../../../aspose.cells.rendering/sheetrender/).

### أمثلة

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

### انظر أيضًا

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


