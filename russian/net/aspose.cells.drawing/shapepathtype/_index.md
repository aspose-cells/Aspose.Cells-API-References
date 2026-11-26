---
title: "Перечисление ShapePathType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.ShapePathType. Представляет тип сегмента пути"
type: docs
url: /ru/net/aspose.cells.drawing/shapepathtype/
---
## ShapePathType enumeration

Представляет тип сегмента пути.

```csharp
public enum ShapePathType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| LineTo | `1` | Прямой линейный сегмент |
| CubicBezierCurveTo | `3` | Кубическая кривая Безье |
| MoveTo | `0` | Начать новый путь |
| Close | `128` | Если начальная ТОЧКА и конечная ТОЧКА не совпадают, рисуется одна прямая линия, соединяющая начальную ТОЧКУ и конечную ТОЧКУ пути. |
| End | `4` | Конец текущего пути |
| Escape | `5` | Escape |
| ArcTo | `6` | Дуга |
| Unknown | `7` | Неизвестно |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создайте фигуру, чтобы продемонстрировать типы путей
                Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 10, 10, 200, 200);

                // Создайте пользовательский геометрический путь
                Geometry geometry = shape.Geometry;
                ShapePath path = new ShapePath();

                // Продемонстрируйте различные значения ShapePathType
                Console.WriteLine("Available ShapePathType values:");
                Console.WriteLine($"LineTo: {ShapePathType.LineTo}");
                Console.WriteLine($"CubicBezierCurveTo: {ShapePathType.CubicBezierCurveTo}");
                Console.WriteLine($"MoveTo: {ShapePathType.MoveTo}");
                Console.WriteLine($"Close: {ShapePathType.Close}");
                Console.WriteLine($"End: {ShapePathType.End}");

                // Примените некоторые операции с путями
                path.MoveTo(10, 10);
                path.LineTo(100, 100);
                path.Close();

                // Сохраните книгу
                workbook.Save("ShapePathTypeDemo.xlsx");
                Console.WriteLine("Demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathType: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


