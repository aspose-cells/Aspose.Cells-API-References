---
title: "Перечисление FillPictureType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.FillPictureType enum. Представляет тип заливки изображением"
type: docs
url: /ru/net/aspose.cells.drawing/fillpicturetype/
---
## FillPictureType enumeration

Представляет тип заливки изображением.

```csharp
public enum FillPictureType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Stretch | `0` | Растянуть |
| Stack | `1` | Стек |
| StackAndScale | `2` | StackAndScale |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassFillPictureTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную форму для демонстрации заливки изображением
            Shape shape = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 200, 200);

            // Установить свойства заливки изображением
            shape.Fill.Type = FillType.Texture;
            shape.Fill.PictureFormatType = FillPictureType.StackAndScale;

            // Использовать минимальное изображение 1x1 пиксель (белое) для демонстрации
            string base64Image = "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=";
            shape.Fill.ImageData = Convert.FromBase64String(base64Image);

            // Добавить другую форму с другим типом заливки
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 5, 2, 0, 200, 200);
            shape2.Fill.Type = FillType.Texture;
            shape2.Fill.PictureFormatType = FillPictureType.Stretch;
            shape2.Fill.ImageData = Convert.FromBase64String(base64Image);

            // Сохранить книгу с различными конфигурациями заливки
            workbook.Save("FillPictureTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


