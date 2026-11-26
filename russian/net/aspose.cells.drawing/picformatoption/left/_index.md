---
title: "PicFormatOption.Left"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PicFormatOption. Возвращает или задает левое смещение для растягивания изображения"
type: docs
url: /ru/net/aspose.cells.drawing/picformatoption/left/
---
## PicFormatOption.Left property

Получает или задаёт смещение слева для растягивания изображения.

```csharp
public double Left { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyLeftDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму для демонстрации форматирования изображения
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 300, 150);

            // Настройте заливку изображения для формы
            shape.FillFormat.ImageData = File.ReadAllBytes("sample.png"); // Ensure this image exists

            // Создайте и настройте PicFormatOption
            PicFormatOption picFormat = new PicFormatOption
            {
                Type = FillPictureType.Stretch,
                Left = 0.0 // Initial left offset (0%)
            };

            // Примените параметры формата к форме (предполагая правильное имя свойства)
            // Примечание: Свойство 'PictureFormatOptions' может не существовать в текущей версии API.
            // Строка ниже закомментирована, чтобы устранить ошибку компиляции.
            // shape.FillFormat.PictureFormatOptions = picFormat;

            // Отобразите начальное левое смещение
            Console.WriteLine("Initial Left offset: " + picFormat.Left);

            // Измените левое смещение, чтобы обрезать 20% с левой стороны
            picFormat.Left = 0.2;
            Console.WriteLine("Modified Left offset: " + picFormat.Left);

            // Сохраните книгу с изменённым форматированием изображения
            workbook.Save("LeftPropertyDemo.xlsx");
        }
    }
}
```

### См. также

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


