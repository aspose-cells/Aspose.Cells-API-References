---
title: "Класс ShapePath"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.ShapePath class. Представляет путь создания, состоящий из серии перемещений, линий и кривых, которые в совокупности образуют геометрическую форму"
type: docs
url: /ru/net/aspose.cells.drawing/shapepath/
---
## ShapePath class

Представляет путь создания, состоящий из серии перемещений, линий и кривых, которые при объединении образуют геометрическую форму.

```csharp
public class ShapePath
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ShapePath](shapepath/)() | Инициализирует новый экземпляр класса `ShapePath`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [HeightPixel](../../aspose.cells.drawing/shapepath/heightpixel/) { get; set; } | Получает высоту этого пути в пикселях. |
| [PathSegementList](../../aspose.cells.drawing/shapepath/pathsegementlist/) { get; } | (**Obsolete.**) Получает список [`ShapeSegmentPathCollection`](../shapesegmentpathcollection/) |
| [PathSegments](../../aspose.cells.drawing/shapepath/pathsegments/) { get; } | Получает список [`ShapeSegmentPathCollection`](../shapesegmentpathcollection/) |
| [WidthPixel](../../aspose.cells.drawing/shapepath/widthpixel/) { get; set; } | Получает ширину этого пути в пикселях. |

## Методы

| Имя | Описание |
| --- | --- |
| [ArcTo](../../aspose.cells.drawing/shapepath/arcto/)(float, float, float, float) | Добавляет эллиптическую дугу к текущей фигуре. Начальная точка является конечной точкой текущей фигуры. |
| [Close](../../aspose.cells.drawing/shapepath/close/)() | Закрывает текущую фигуру и начинает новую фигуру. Если текущая фигура содержит последовательность соединённых линий и кривых, метод замыкает контур, соединяя линией конечную точку с начальной. |
| [CubicBezierTo](../../aspose.cells.drawing/shapepath/cubicbezierto/)(float, float, float, float, float, float) | Добавляет кубическую кривую Безье к текущей фигуре. Начальная точка является конечной точкой текущей фигуры. Единица измерения: пиксель. |
| [LineTo](../../aspose.cells.drawing/shapepath/lineto/)(float, float) | Добавляет отрезок линии к текущей фигуре. Начальная точка является конечной точкой текущей фигуры. Единица измерения: пиксель. |
| [MoveTo](../../aspose.cells.drawing/shapepath/moveto/)(float, float) | Начинает новую фигуру из указанной точки без закрытия текущей фигуры. Все последующие точки, добавляемые в путь, добавляются к этой новой фигуре. Единица измерения: пиксель. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapePathDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить пользовательскую форму со всеми необходимыми параметрами
            Shape customShape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 200, 100, 0, 0);
            
            // Получить доступ к ShapePathCollection
            ShapePathCollection shapePaths = customShape.Paths;

            // Добавить новый путь и получить к нему доступ
            int pathIndex = shapePaths.Add();
            ShapePath newPath = shapePaths[pathIndex];

            // Вывести количество путей
            Console.WriteLine("Number of paths in the ShapePathCollection: " + shapePaths.Count.ToString());

            // Сохраните книгу
            workbook.Save("ShapePathDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


