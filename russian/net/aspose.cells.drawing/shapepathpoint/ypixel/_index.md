---
title: "ShapePathPoint.YPixel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapePathPoint. Когда объект является координатой позиции, получайте или задавайте координату y в пикселях"
type: docs
url: /ru/net/aspose.cells.drawing/shapepathpoint/ypixel/
---
## ShapePathPoint.YPixel property

Когда объект является координатой позиции, получайте или задавайте координату y в пикселях.

```csharp
public int YPixel { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyYPixelDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создайте коллекцию точек пути формы
                ShapePathPointCollection pathPoints = new ShapePathPointCollection();

                // Добавьте точку с координатами
                pathPoints.Add(100, 50);

                // Получите доступ к первой точке и продемонстрируйте свойство YPixel
                ShapePathPoint firstPoint = pathPoints[0];

                // Отобразите начальное значение YPixel (операция чтения)
                Console.WriteLine($"Initial YPixel value: {firstPoint.YPixel}");

                // Установите новое значение для YPixel (поскольку оно доступно для чтения/записи)
                firstPoint.YPixel = 150;
                Console.WriteLine($"Updated YPixel value: {firstPoint.YPixel}");

                // Создайте путь формы и используйте точку
                ShapePath path = new ShapePath();
                path.MoveTo(firstPoint.XPixel, firstPoint.YPixel);

                // Добавить свободную форму на лист
                worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path });

                // Сохраните книгу
                workbook.Save("YPixelDemo.xlsx");
                Console.WriteLine("YPixel property demonstration completed successfully.");
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

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


