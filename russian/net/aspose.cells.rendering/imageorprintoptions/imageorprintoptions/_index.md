---
title: "ImageOrPrintOptions.ImageOrPrintOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор ImageOrPrintOptions. Ctor"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/imageorprintoptions/
---
## ImageOrPrintOptions constructor

Конструктор.

```csharp
public ImageOrPrintOptions()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Hello World!");
            
            // Продемонстрировать использование #ctor
            ImageOrPrintOptions imgOptions = new ImageOrPrintOptions();
            imgOptions.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Отрендерьте лист в изображение
            SheetRender sheetRender = new SheetRender(sheet, imgOptions);
            sheetRender.ToImage(0, "output.png");
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


