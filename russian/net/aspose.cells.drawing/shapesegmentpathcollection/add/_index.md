---
title: "ShapeSegmentPathCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeSegmentPathCollection. Добавьте сегментный путь в путь создания"
type: docs
url: /ru/net/aspose.cells.drawing/shapesegmentpathcollection/add/
---
## ShapeSegmentPathCollection.Add method

Добавить сегментный путь в путь создания.

```csharp
public int Add(ShapePathType type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | ShapePathType | Тип пути. |

### Возвращаемое значение

Возвращает позицию объекта [`ShapeSegmentPath`](../../shapesegmentpath/) в списке.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathCollectionMethodAddWithShapePathTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ShapePath path = new ShapePath();

            // Начать новый путь
            path.MoveTo(10, 10);

            // Нарисовать линейный сегмент
            path.LineTo(100, 100);

            // Получить доступ к свойству PathSegementList
            ShapeSegmentPathCollection segmentList = path.PathSegementList;

            segmentList.Add(ShapePathType.Close);

            // Отобразить количество сегментов пути
            Console.WriteLine("Number of path segments: " + segmentList.Count);

            // Итерировать каждый сегмент и отобразить его тип
            foreach (ShapeSegmentPath segment in segmentList)
            {
                Console.WriteLine("Segment type: " + segment.Type);
            }

           
            //добавить свободную форму
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });

            // Сохраните книгу, чтобы наблюдать изменения формы
            workbook.Save("ShapeSegmentPathCollectionAddDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ShapePathType](../../shapepathtype/)
* class [ShapeSegmentPathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


