---
title: "TextureFill.Transparency"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextureFill. Возвращает или задает степень прозрачности области значением от 0.0 (непрозрачно) до 1.0 (полностью прозрачно)"
type: docs
url: /ru/net/aspose.cells.drawing/texturefill/transparency/
---
## TextureFill.Transparency property

Возвращает или задает степень прозрачности области значением от 0.0 (непрозрачный) до 1.0 (прозрачный).

```csharp
public double Transparency { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру на лист
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // Установить тип заливки как текстуру
            shape.Fill.FillType = FillType.Texture;

            // Получить доступ к свойствам заливки текстурой
            TextureFill textureFill = shape.Fill.TextureFill;

            // Установить встроенный тип текстуры
            textureFill.Type = TextureType.BlueTissuePaper;

            // Отобразить начальное значение прозрачности
            Console.WriteLine("Initial Transparency: " + textureFill.Transparency);

            // Изменить прозрачность до 70% (0.0 = непрозрачно, 1.0 = полностью прозрачно)
            textureFill.Transparency = 0.7;
            Console.WriteLine("Updated Transparency: " + textureFill.Transparency);

            // Сохранить книгу с видимым эффектом прозрачности
            workbook.Save("TextureFillTransparencyDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


