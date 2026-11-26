---
title: "PicFormatOption.Top"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PicFormatOption. Получает или задает верхнее смещение для растягивания изображения"
type: docs
url: /ru/net/aspose.cells.drawing/picformatoption/top/
---
## PicFormatOption.Top property

Получает или задаёт смещение сверху для растягивания изображения.

```csharp
public double Top { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyTopDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Используйте существующее изображение или укажите правильный путь к изображению
            string imagePath = "existingImage.png";

            // Добавить фигуру с правильными параметрами
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);
            
            // Примените заливку изображения с помощью ImageData
            shape.FillFormat.ImageData = File.ReadAllBytes(imagePath);

            // Создайте и настройте PicFormatOption напрямую
            PicFormatOption picFormat = new PicFormatOption();

            Console.WriteLine("Initial Top value: " + picFormat.Top);
            picFormat.Top = 0.3;

            // Предполагая, что PicFormatOption необходимо связать с форматом заливки
            // Эта часть может потребовать реализации, специфичной для API, не показанной в определениях типов
            // shape.FillFormat.SetPicFormatOption(picFormat);

            Console.WriteLine("Modified Top value: " + picFormat.Top);
            workbook.Save("TopPropertyDemo.xlsx");
        }
    }
}
```

### См. также

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


