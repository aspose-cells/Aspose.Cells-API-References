---
title: "ImageSaveOptions.ImageOrPrintOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageSaveOptions. Дополнительные параметры создания изображения"
type: docs
url: /ru/net/aspose.cells/imagesaveoptions/imageorprintoptions/
---
## ImageSaveOptions.ImageOrPrintOptions property

Дополнительные параметры создания изображения.

```csharp
public ImageOrPrintOptions ImageOrPrintOptions { get; }
```

### Примечания

Для расширенного использования, пожалуйста, используйте [`WorkbookRender`](../../../aspose.cells.rendering/workbookrender/) или [`SheetRender`](../../../aspose.cells.rendering/sheetrender/).

### Примеры

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

### См. также

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


