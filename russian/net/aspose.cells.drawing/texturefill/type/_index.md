---
title: "TextureFill.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextureFill. Получает и задает тип текстуры"
type: docs
url: /ru/net/aspose.cells.drawing/texturefill/type/
---
## TextureFill.Type property

Получает и задает тип текстуры

```csharp
public TextureType Type { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму, чтобы продемонстрировать заливку текстурой
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);

            // Установить тип заливки как текстуру
            shape.Fill.FillType = FillType.Texture;

            // Получить доступ к свойствам заливки текстурой
            TextureFill textureFill = shape.Fill.TextureFill;

            try
            {
                // Отобразить начальное значение Type
                Console.WriteLine("Initial Texture Type: " + textureFill.Type);

                // Установить другой тип текстуры
                textureFill.Type = TextureType.Granite;
                Console.WriteLine("Updated Texture Type: " + textureFill.Type);

                // Продемонстрировать другой тип текстуры
                textureFill.Type = TextureType.WaterDroplets;
                Console.WriteLine("Final Texture Type: " + textureFill.Type);

                // Сохранить рабочую книгу, чтобы увидеть эффект
                workbook.Save("TextureFillTypeDemo.xlsx");
                Console.WriteLine("Texture fill type demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [TextureType](../../texturetype/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


