---
title: "ShapeCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapeCollection. Возвращает объект Shape по конкретному индексу в списке"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/item/
---
## ShapeCollection indexer (1 of 2)

Получает объект [`Shape`](../../shape/) по конкретному индексу в списке.

```csharp
public Shape this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте несколько фигур в лист с корректными параметрами
            worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            worksheet.Shapes.AddOval(2, 0, 150, 100, 100, 100);
            worksheet.Shapes.AddLine(3, 0, 300, 100, 100, 100);

            // Получить коллекцию фигур
            ShapeCollection shapes = worksheet.Shapes;

            // Продемонстрировать свойство Item, получая первую фигуру
            Shape firstShape = shapes[0];
            Console.WriteLine("First shape type: " + firstShape.Type);

            // Продемонстрировать свойство Item, получая фигуру по идентификатору
            Shape shapeById = shapes[2];
            Console.WriteLine("Shape with ID 2 type: " + shapeById.Type);
        }
    }
}
```

### См. также

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ShapeCollection indexer (2 of 2)

Получает объект [`Shape`](../../shape/) по имени фигуры.

```csharp
public Shape this[string name] { get; }
```

| Параметр | Описание |
| --- | --- |
| name | Имя фигуры. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить фигуры в лист
            ShapeCollection shapes = worksheet.Shapes;
            shapes.AddRectangle(2, 0, 2, 0, 130, 130);
            shapes.AddOval(5, 0, 2, 0, 130, 130);
            
            // Получать доступ к фигурам с помощью свойства Item
            Shape rectangle = shapes["Rectangle 1"];
            if (rectangle != null)
            {
                rectangle.FillFormat.ForeColor = System.Drawing.Color.Red;
            }
            
            Shape oval = shapes["Oval 2"];
            if (oval != null)
            {
                oval.FillFormat.ForeColor = System.Drawing.Color.Blue;
            }
            
            // Сохраните книгу
            workbook.Save("ShapeCollectionDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


