---
title: "ShapeSegmentPathCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapeSegmentPathCollection. Возвращает объект ShapeSegmentPath"
type: docs
url: /ru/net/aspose.cells.drawing/shapesegmentpathcollection/item/
---
## ShapeSegmentPathCollection indexer

Возвращает объект [`ShapeSegmentPath`](../../shapesegmentpath/).

```csharp
public ShapeSegmentPath this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Возвращаемое значение

Возвращает объект [`ShapeSegmentPath`](../../shapesegmentpath/).

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathCollectionPropertyItemDemo
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
            ShapeSegmentPathCollection segmentPaths = path.PathSegementList;


            segmentPaths.Add(ShapePathType.Close);

            // Отобразить количество сегментов пути
            Console.WriteLine("Number of path segments: " + segmentPaths.Count);
          
            
            // Продемонстрировать чтение свойства Item
            for (int i = 0; i < segmentPaths.Count; i++)
            {
                ShapeSegmentPath segment = segmentPaths[i];
                Console.WriteLine($"Segment {i} type: {segment.Type}");
            }

            //добавить свободную форму
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });
            // Сохраните книгу
            workbook.Save("ShapeSegmentPathCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapeSegmentPath](../../shapesegmentpath/)
* class [ShapeSegmentPathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


