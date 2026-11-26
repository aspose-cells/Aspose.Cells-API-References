---
title: "CustomGeometry.Paths"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CustomGeometry. Получает информацию о коллекции путей, когда фигура является не примитивным автошейпом"
type: docs
url: /ru/net/aspose.cells.drawing/customgeometry/paths/
---
## CustomGeometry.Paths property

Получает информацию о коллекции путей, когда фигура является NotPrimitive автоконтуром

```csharp
public ShapePathCollection Paths { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CustomGeometryPropertyPathsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить пользовательскую фигуру с непримитивной геометрией (фиксированные параметры)
            var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 0, 0, 10, 10, 400, 400);
            
            // Получить доступ к пользовательской геометрии через явное приведение типов
            CustomGeometry geometry = (CustomGeometry)shape.Geometry;
            
            // Получить коллекцию путей
            ShapePathCollection paths = geometry.Paths;
            Console.WriteLine($"Initial path count: {paths.Count}");

            // Создать новый путь фигуры, используя команды рисования
            paths.Add(); // Creates a new path in the collection
            ShapePath newPath = paths[paths.Count - 1];
            newPath.MoveTo(0, 0);
            newPath.LineTo(10000, 0);
            newPath.LineTo(10000, 10000);
            newPath.LineTo(0, 10000);
            newPath.Close();

            // Явный вызов Add не требуется, так как путь был создан в коллекции
            Console.WriteLine($"New path count after modification: {paths.Count}");

            // Сохранить, чтобы продемонстрировать постоянные изменения
            workbook.Save("CustomGeometryPathsDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapePathCollection](../../shapepathcollection/)
* class [CustomGeometry](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


