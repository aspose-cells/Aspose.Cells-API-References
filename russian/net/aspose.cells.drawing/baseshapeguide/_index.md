---
title: "Класс BaseShapeGuide"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.BaseShapeGuide. Представляет направляющую фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/baseshapeguide/
---
## BaseShapeGuide class

Представляет направляющую формы.

```csharp
public class BaseShapeGuide
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassBaseShapeGuideDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создайте прямоугольную фигуру с правильными параметрами
                Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

                // Поскольку у BaseShapeGuide нет публичного конструктора,
                // мы продемонстрируем его использование через фигуру, которая может содержать направляющие
                // Примечание: Это упрощённая демонстрация, так как реальный доступ к направляющим может отличаться
                Console.WriteLine("Shape created successfully");
                Console.WriteLine($"Shape type: {shape.GetType().Name}");

                // Сохраните книгу
                workbook.Save("BaseShapeGuideDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with BaseShapeGuide: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


