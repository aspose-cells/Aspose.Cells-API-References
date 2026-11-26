---
title: "ShapePath.HeightPixel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapePath. Получает высоту этого пути в пикселях."
type: docs
url: /ru/net/aspose.cells.drawing/shapepath/heightpixel/
---
## ShapePath.HeightPixel property

Получает высоту этого пути в пикселях.

```csharp
public int HeightPixel { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyHeightPixelDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создать новый путь формы
                ShapePath shapePath = new ShapePath();

                // Создайте простой прямоугольный путь.
                shapePath.MoveTo(10, 10);
                shapePath.LineTo(100, 10);
                shapePath.LineTo(100, 50);
                shapePath.LineTo(10, 50);
                shapePath.Close();

                // Отобразите текущее значение HeightPixel.
                Console.WriteLine("Initial HeightPixel value: " + shapePath.HeightPixel);

                // Установите новое значение высоты.
                shapePath.HeightPixel = 200;
                Console.WriteLine("Updated HeightPixel value: " + shapePath.HeightPixel);

                // Добавить форму в лист
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                // Сохраните книгу
                workbook.Save("HeightPixelDemo.xlsx");
                Console.WriteLine("HeightPixel property demonstrated successfully.");
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

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


