---
title: "MsoFillFormat.Texture"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoFillFormat. Получает тип заливки текстурой"
type: docs
url: /ru/net/aspose.cells.drawing/msofillformat/texture/
---
## MsoFillFormat.Texture property

Получает тип текстурного заполнения.

```csharp
public TextureType Texture { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFillFormatPropertyTextureDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную фигуру, чтобы продемонстрировать форматирование заливки
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // Получить формат заливки
            MsoFillFormat fillFormat = rectangle.FillFormat;

            try
            {
                // Отобразить текущий тип текстуры (только для чтения)
                TextureType currentTexture = fillFormat.Texture;
                Console.WriteLine("Current Texture Type: " + currentTexture);

                // Установите некоторые данные изображения, чтобы потенциально изменить текстуру
                // Это демонстрирует, как текстура может быть изменена данными изображения
                byte[] sampleImageData = new byte[] { 0x89, 0x50, 0x4E, 0x47 }; // PNG header
                fillFormat.ImageData = sampleImageData;

                // Отобразить тип текстуры снова после установки данных изображения
                TextureType updatedTexture = fillFormat.Texture;
                Console.WriteLine("Texture Type after setting image data: " + updatedTexture);

                // Сохраните книгу
                workbook.Save("TextureDemo.xlsx");
                Console.WriteLine("Texture demonstration completed successfully.");
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
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


