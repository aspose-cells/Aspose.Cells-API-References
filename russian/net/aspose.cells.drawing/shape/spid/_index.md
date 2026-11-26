---
title: "Shape.Spid"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Указывает необязательный строковый идентификатор, который приложение может использовать для идентификации конкретной фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/spid/
---
## Shape.Spid property

Указывает необязательный строковый идентификатор, который приложение может использовать для идентификации конкретной фигуры.

```csharp
public string Spid { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySpidDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру на лист с правильными параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Получить и отобразить свойство Spid фигуры
            string spid = shape.Spid;
            Console.WriteLine("Shape SPID: " + spid);

            // Сохраните книгу
            workbook.Save("ShapePropertySpidDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


