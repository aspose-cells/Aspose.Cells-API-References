---
title: "PicFormatOption.Right"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PicFormatOption. Возвращает или задает правое смещение для растягивания изображения"
type: docs
url: /ru/net/aspose.cells.drawing/picformatoption/right/
---
## PicFormatOption.Right property

Получает или задаёт смещение справа для растягивания изображения.

```csharp
public double Right { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyRightDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму с указанными размерами
            Shape shape = worksheet.Shapes.AddRectangle(5, 2, 10, 10, 150, 300);

            // Настройте заливку изображения для формы
            shape.Fill.FillType = FillType.Texture;
            string imagePath = "sample.jpg"; // Replace with actual image path
            
            if (File.Exists(imagePath))
            {
                shape.Fill.ImageData = File.ReadAllBytes(imagePath);
            }
            else
            {
                Console.WriteLine("Image not found - using empty picture fill");
            }

            // Получите доступ к параметрам формата изображения через TextureFill
            PicFormatOption picFormat = shape.Fill.TextureFill.PicFormatOption;

            // Отобразите и измените свойство Right
            Console.WriteLine("Initial Right offset: " + picFormat.Right);
            picFormat.Right = 25.5; // Set right offset to 25.5 units

            // Проверьте новое значение и сохраните изменения
            Console.WriteLine("Updated Right offset: " + picFormat.Right);
            workbook.Save("RightPropertyDemo.xlsx");
        }
    }
}
```

### См. также

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


