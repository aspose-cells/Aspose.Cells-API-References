---
title: "Range.ToImage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Преобразует диапазон в изображение"
type: docs
url: /ru/net/aspose.cells/range/toimage/
---
## Range.ToImage method

Преобразует диапазон в изображение.

```csharp
public byte[] ToImage(ImageOrPrintOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опции | ImageOrPrintOptions | Опции для преобразования этого диапазона в изображение |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RangeMethodToImageWithImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Создайте рабочую книгу из примера файла Excel
            Workbook workbook = new Workbook("example.xlsx");
            
            // Получите первый рабочий лист и его ячейки
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Создайте диапазон A1:J25
            Aspose.Cells.Range range = cells.CreateRange("A1:J25");
            
            // Создать параметры изображения
            ImageOrPrintOptions options = new ImageOrPrintOptions()
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            
            // Преобразуйте диапазон в изображение
            byte[] imageData = range.ToImage(options);
            
            // Сохраните изображение в файл
            File.WriteAllBytes("range_output.png", imageData);
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


