---
title: "TextureFill.Scale"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextureFill. Получает и задает масштаб формата изображения"
type: docs
url: /ru/net/aspose.cells.drawing/texturefill/scale/
---
## TextureFill.Scale property

Получает и задает масштаб формата изображения.

```csharp
public double Scale { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TextureFillPropertyScaleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить фигуру и получить её формат заливки
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 10, 10, 500, 300);
            FillFormat fillFormat = shape.Fill;

            // Настроить заполнение текстурой
            fillFormat.FillType = FillType.Texture;
            TextureFill textureFill = fillFormat.TextureFill;

            // Загрузить изображение текстуры и настроить свойства
            textureFill.ImageData = File.ReadAllBytes("texture.jpg");
            textureFill.Type = TextureType.Unknown; // Changed from UserDefined to Unknown
            textureFill.IsTiling = true;

            // Отобразить и изменить масштаб
            Console.WriteLine("Initial Scale: " + textureFill.Scale);
            textureFill.Scale = 0.5;
            Console.WriteLine("Modified Scale: " + textureFill.Scale);

            // Сохранить результат
            workbook.Save("TextureFillScaleDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


