---
title: "Shape.Id"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает идентификатор этой фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/id/
---
## Shape.Id property

Получает идентификатор этой фигуры.

```csharp
public int Id { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIdDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Получить и отобразить ID фигуры
            int id = shape.Id;
            Console.WriteLine("Shape ID: " + id);

            // Изменить свойства фигуры
            shape.Name = "Rectangle1";
            shape.Text = "Shape with ID: " + id;

            // Сохраните книгу
            workbook.Save("ShapePropertyIdDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


