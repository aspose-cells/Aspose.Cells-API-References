---
title: "ShapePath.WidthPixel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapePath. Получает ширину этого пути в пикселях."
type: docs
url: /ru/net/aspose.cells.drawing/shapepath/widthpixel/
---
## ShapePath.WidthPixel property

Получает ширину этого пути в пикселях.

```csharp
public int WidthPixel { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyWidthPixelDemo
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

                // Отобразите начальное значение WidthPixel.
                Console.WriteLine("Initial WidthPixel value: " + shapePath.WidthPixel);

                // Установите новое значение ширины.
                shapePath.WidthPixel = 300;
                Console.WriteLine("Updated WidthPixel value: " + shapePath.WidthPixel);

                // Добавить форму в лист
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, shapePath.WidthPixel, 200, new ShapePath[] { shapePath });

                // Сохраните книгу
                workbook.Save("WidthPixelDemo.xlsx");
                Console.WriteLine("WidthPixel property demonstrated successfully.");
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


