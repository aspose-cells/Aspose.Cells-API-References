---
title: "PicFormatOption.Bottom"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PicFormatOption. Получает или задает нижнее смещение для растягивания изображения"
type: docs
url: /ru/net/aspose.cells.drawing/picformatoption/bottom/
---
## PicFormatOption.Bottom property

Получает или задаёт смещение снизу для растягивания изображения.

```csharp
public double Bottom { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyBottomDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Используйте существующий файл изображения (замените реальным путем к изображению)
            string imagePath = "sample.jpg";

            // Добавить прямоугольную фигуру на лист
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 200);

            // Настройте заливку shape для использования образца изображения
            // FillType определяется при установке ImageData, что задает тип Texture
            shape.FillFormat.ImageData = File.ReadAllBytes(imagePath);
            
            // Создайте и настройте параметры формата изображения
            PicFormatOption picFormat = new PicFormatOption();
            picFormat.Type = FillPictureType.Stretch;

            // Отобразить начальное значение Bottom
            Console.WriteLine("Initial Bottom value: " + picFormat.Bottom);

            // Изменить смещение Bottom и отобразить новое значение
            picFormat.Bottom = 0.3;
            Console.WriteLine("Modified Bottom value: " + picFormat.Bottom);

            // Свяжите PicFormatOption с заливкой shape (если применимо)
            // Примечание: Этот шаг может потребовать методов, специфичных для API, не показанных в предоставленном контексте
            // Для демонстрации PicFormatOption создаётся и настраивается

            // Сохраните рабочую книгу с применёнными изменениями
            workbook.Save("PicFormatOptionBottomDemo.xlsx");
        }
    }
}
```

### См. также

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


