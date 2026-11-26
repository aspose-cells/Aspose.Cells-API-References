---
title: "ImageOrPrintOptions.HorizontalResolution"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Получает или задает горизонтальное разрешение генерируемых изображений в точках на дюйм"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/horizontalresolution/
---
## ImageOrPrintOptions.HorizontalResolution property

Получает или задает горизонтальное разрешение генерируемых изображений в точках на дюйм.

```csharp
public int HorizontalResolution { get; set; }
```

### Примечания

Значение по умолчанию — 96.

Настройка `HorizontalResolution` и [`VerticalResolution`](../verticalresolution/) влияет на ширину и высоту выходного изображения в пикселях.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyHorizontalResolutionDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text for Image Rendering");

            // Инициализируйте ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            
            // Установите горизонтальное и вертикальное разрешение
            options.HorizontalResolution = 192;
            options.VerticalResolution = 192;

            // Отрендерьте лист в изображение с указанным разрешением
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "WorksheetImage_192dpi.png");

            // Продемонстрируйте различные разрешения
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;
            renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "WorksheetImage_300dpi.png");
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


