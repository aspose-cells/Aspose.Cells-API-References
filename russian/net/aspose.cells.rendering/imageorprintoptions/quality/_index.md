---
title: "ImageOrPrintOptions.Quality"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Получает или задает значение, определяющее качество сгенерированных изображений, применяемое только при сохранении страниц в формате JPEG. Значение по умолчанию — 100"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/quality/
---
## ImageOrPrintOptions.Quality property

Получает или задает значение, определяющее качество генерируемых изображений, применяемое только при сохранении страниц в формате `Jpeg`. Значение по умолчанию — 100

```csharp
public int Quality { get; set; }
```

### Примечания

Имеет эффект только при сохранении в JPEG. Значение должно быть от 0 до 100. Значение по умолчанию — 100.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyQualityDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["C3"].PutValue(DateTime.Now);

            // Создать параметры изображения с различными настройками качества
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;
            options.Quality = 100; // Highest quality

            // Отрисовать лист в изображение с высоким качеством
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "HighQualityOutput.jpg");

            // Изменить качество, чтобы продемонстрировать разницу
            options.Quality = 50; // Medium quality
            renderer.ToImage(0, "MediumQualityOutput.jpg");

            options.Quality = 10; // Low quality
            renderer.ToImage(0, "LowQualityOutput.jpg");
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


