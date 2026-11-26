---
title: "ShapePathCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "ShapePathCollection свойство. Получает путь создания"
type: docs
url: /ru/net/aspose.cells.drawing/shapepathcollection/item/
---
## ShapePathCollection indexer

Получает путь создания.

```csharp
public ShapePath this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Возвращаемое значение

Возвращает [`ShapePath`](../../shapepath/) объект.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePathCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить пользовательскую форму (непримитивную форму) с правильными параметрами
            Shape customShape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 10, 10, 200, 200, 0, 0);

            // Получить доступ к ShapePathCollection
            ShapePathCollection shapePaths = customShape.Paths;

            // Добавить новый путь
            int pathIndex = shapePaths.Add();

            // Получить доступ к пути с помощью свойства Item
            ShapePath newPath = shapePaths[pathIndex];

            // Вывести информацию
            Console.WriteLine("Path count: " + shapePaths.Count);
            Console.WriteLine("Path segment count: " + newPath.PathSegementList.Count);

            // Сохраните книгу
            workbook.Save("ShapePathCollectionDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapePath](../../shapepath/)
* class [ShapePathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


