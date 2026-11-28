---
title: "ImageSaveOptions.ImageOrPrintOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageSaveOptions özelliği. Ek görüntü oluşturma seçenekleri"
type: docs
url: /tr/net/aspose.cells/imagesaveoptions/imageorprintoptions/
---
## ImageSaveOptions.ImageOrPrintOptions property

Ek görüntü oluşturma seçenekleri.

```csharp
public ImageOrPrintOptions ImageOrPrintOptions { get; }
```

### Açıklamalar

Gelişmiş kullanım için, lütfen [`WorkbookRender`](../../../aspose.cells.rendering/workbookrender/) veya [`SheetRender`](../../../aspose.cells.rendering/sheetrender/) kullanın.

### Örnekler

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

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


