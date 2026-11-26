---
title: "ShapePathPoint.XPixel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapePathPoint. Когда объект является координатой позиции, получайте или задавайте координату x в пикселях"
type: docs
url: /ru/net/aspose.cells.drawing/shapepathpoint/xpixel/
---
## ShapePathPoint.XPixel property

Когда объект является координатой позиции, получайте или задавайте координату x в пикселях.

```csharp
public int XPixel { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyXPixelDemo
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

                // Добавить точки с координатами
                pathPoints.Add(100, 50);
                pathPoints.Add(200, 100);

                // Получить доступ к первой точке и продемонстрировать свойство XPixel
                ShapePathPoint firstPoint = pathPoints[0];

                // Отобразить значение XPixel (операция чтения)
                Console.WriteLine($"Initial XPixel value: {firstPoint.XPixel}");

                // Установить новое значение для XPixel (поскольку оно доступно для чтения/записи)
                firstPoint.XPixel = 150;
                Console.WriteLine($"Updated XPixel value: {firstPoint.XPixel}");

                // Создать путь фигуры и добавить точки
                ShapePath path = new ShapePath();
                path.MoveTo(firstPoint.XPixel, firstPoint.YPixel);

                // Добавить вторую точку
                ShapePathPoint secondPoint = pathPoints[1];
                path.LineTo(secondPoint.XPixel, secondPoint.YPixel);
                path.Close();

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
                workbook.Save("XPixelDemo.xlsx");
                Console.WriteLine("XPixel property demonstration completed successfully.");
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


