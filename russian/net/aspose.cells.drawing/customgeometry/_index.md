---
title: "Класс CustomGeometry"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.CustomGeometry. Представляет пользовательскую геометрическую форму"
type: docs
url: /ru/net/aspose.cells.drawing/customgeometry/
---
## CustomGeometry class

Представляет пользовательскую геометрическую форму.

```csharp
public class CustomGeometry : Geometry
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Paths](../../aspose.cells.drawing/customgeometry/paths/) { get; } | Получает информацию о коллекции путей, когда фигура является NotPrimitive автоконтуром |
| [ShapeAdjustValues](../../aspose.cells.drawing/geometry/shapeadjustvalues/) { get; } | Получает коллекцию значений настройки формы (унаследовано от [`Geometry`](../geometry/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassCustomGeometryDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить NotPrimitive автоконтур с правильными параметрами
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 0, 0, 0, 0, 200, 300);

            // Получить экземпляр CustomGeometry из фигуры
            CustomGeometry customGeometry = shape.Geometry as CustomGeometry;

            // Создать новый путь в коллекции путей геометрии
            int pathIndex = customGeometry.Paths.Add();
            ShapePath path = customGeometry.Paths[pathIndex];

            // Добавить сегменты пути с помощью прямых вызовов методов
            path.MoveTo(0, 0);
            path.LineTo(1000, 0);
            path.LineTo(1000, 1000);
            path.LineTo(0, 1000);
            path.Close();

            // Сохраните книгу
            workbook.Save("CustomGeometryDemo.xlsx");
        }
    }
}
```

### См. также

* class [Geometry](../geometry/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


