---
title: "Класс ShapeSegmentPathCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.ShapeSegmentPathCollection. Представляет путь создания, состоящий из серии перемещений, линий и кривых, которые в совокупности образуют геометрическую форму"
type: docs
url: /ru/net/aspose.cells.drawing/shapesegmentpathcollection/
---
## ShapeSegmentPathCollection class

Представляет путь создания, состоящий из серии перемещений, линий и кривых, которые при объединении образуют геометрическую форму.

```csharp
public class ShapeSegmentPathCollection : CollectionBase<ShapeSegmentPath>
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ShapeSegmentPathCollection](shapesegmentpathcollection/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/shapesegmentpathcollection/item/) { get; } | Получает объект [`ShapeSegmentPath`](../shapesegmentpath/). |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.drawing/shapesegmentpathcollection/add/)(ShapePathType) | Добавить сегментный путь в путь создания. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ShapeSegmentPath) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ShapeSegmentPath, IComparer&lt;ShapeSegmentPath&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ShapeSegmentPath, IComparer&lt;ShapeSegmentPath&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ShapeSegmentPath) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ShapeSegmentPath[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ShapeSegmentPath[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ShapeSegmentPath[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ShapeSegmentPath&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ShapeSegmentPath&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ShapeSegmentPath&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapeSegmentPath) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapeSegmentPath, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapeSegmentPath, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapeSegmentPath) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapeSegmentPath, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapeSegmentPath, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapeSegmentPathCollectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создать ShapePath для работы с сегментами
                ShapePath path = new ShapePath();

                // Начать новый путь
                path.MoveTo(10, 10);

                // Нарисовать линейный сегмент
                path.LineTo(100, 100);

                // Получить ShapeSegmentPathCollection из пути
                ShapeSegmentPathCollection segmentPaths = path.PathSegementList;

                // Добавить закрывающий сегмент пути
                int index = segmentPaths.Add(ShapePathType.Close);

                // Отобразить информацию о коллекции
                Console.WriteLine($"Number of path segments: {segmentPaths.Count}");
                Console.WriteLine($"Added segment at index: {index}");

                // Получить доступ к первому сегменту (только для чтения)
                if (segmentPaths.Count > 0)
                {
                    ShapeSegmentPath firstSegment = segmentPaths[0];
                    Console.WriteLine($"First segment type: {firstSegment.Type}");
                }

                // Добавить форму в лист
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });

                // Сохраните книгу
                workbook.Save("ShapeSegmentPathCollectionDemo.xlsx");
                Console.WriteLine("ShapeSegmentPathCollection demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ShapeSegmentPathCollection demo: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ShapeSegmentPath](../shapesegmentpath/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


