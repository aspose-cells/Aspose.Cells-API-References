---
title: "TextureFill.PictureFormatType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextureFill. Получает и задает тип формата изображения"
type: docs
url: /ru/net/aspose.cells.drawing/texturefill/pictureformattype/
---
## TextureFill.PictureFormatType property

Получает и задает тип формата изображения.

```csharp
public FillPictureType PictureFormatType { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyPictureFormatTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // Установить тип заливки как текстуру
            shape.Fill.FillType = FillType.Texture;
            TextureFill textureFill = shape.Fill.TextureFill;

            // Загрузить минимальное PNG-изображение 1×1 пиксель (белое)
            string base64Image = "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=";
            textureFill.ImageData = Convert.FromBase64String(base64Image);

            // Отобразить текущий PictureFormatType
            Console.WriteLine("Initial PictureFormatType: " + textureFill.PictureFormatType);

            // Переключить на слойный формат и включить плитку
            textureFill.PictureFormatType = FillPictureType.Stack;
            textureFill.IsTiling = true;

            // Добавить другую фигуру для сравнения с оригинальным растянутым форматом
            Shape shape2 = worksheet.Shapes.AddRectangle(0, 0, 210, 0, 100, 200);
            shape2.Fill.FillType = FillType.Texture;
            TextureFill textureFill2 = shape2.Fill.TextureFill;
            textureFill2.ImageData = Convert.FromBase64String(base64Image);

            // Сохранить книгу с обоими примерами заливки текстурой
            workbook.Save("TextureFillPictureFormatTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [FillPictureType](../../fillpicturetype/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


