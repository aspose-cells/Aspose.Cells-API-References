---
title: "Shape.CreateId"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает идентификатор создания для этой формы"
type: docs
url: /ru/net/aspose.cells.drawing/shape/createid/
---
## Shape.CreateId property

Получает и задает идентификатор создания для этой фигуры.

```csharp
public Guid CreateId { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyCreateIdDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить прямоугольную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 200, 150);
            
            // Создайте и назначьте новый GUID в качестве CreateId
            Guid createId = Guid.NewGuid();
            shape.CreateId = createId;
            
            // Сохраните книгу
            workbook.Save("ShapeCreateIdDemo.xlsx");
            
            // Перезагрузите книгу, чтобы проверить сохранность CreateId
            Workbook loadedWorkbook = new Workbook("ShapeCreateIdDemo.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Выведите CreateId для проверки
            Console.WriteLine("Original CreateId: " + createId);
            Console.WriteLine("Loaded CreateId: " + loadedShape.CreateId);
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


