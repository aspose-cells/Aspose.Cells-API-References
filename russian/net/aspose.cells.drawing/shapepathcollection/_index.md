---
title: "Класс ShapePathCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.ShapePathCollection class. Представляет информацию о коллекции путей в автоконтуре NotPrimitive"
type: docs
url: /ru/net/aspose.cells.drawing/shapepathcollection/
---
## ShapePathCollection class

Представляет информацию о коллекции путей в NotPrimitive autoshape.

```csharp
public class ShapePathCollection : CollectionBase<ShapePath>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells.drawing/shapepathcollection/count/) { get; } | Получает количество путей |
| [Item](../../aspose.cells.drawing/shapepathcollection/item/) { get; } | Получает путь создания. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.drawing/shapepathcollection/add/)() | Добавить путь создания. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ShapePath) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ShapePath, IComparer&lt;ShapePath&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ShapePath, IComparer&lt;ShapePath&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ShapePath) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ShapePath[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ShapePath[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ShapePath[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ShapePath&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ShapePath&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ShapePath&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ShapePath&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ShapePath&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ShapePath&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ShapePath&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ShapePath&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ShapePath&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ShapePath&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapePath) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapePath, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapePath, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapePath) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapePath, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapePath, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathCollectionDemo
    {
        public static void ShapePathCollectionExample()
        {



            // Создайте новый Workbook
            Workbook workbook = new Workbook("ShapePathCollectionExample_original.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];

            Shape customShape = worksheet.Shapes[0];
            
            // Получить доступ к ShapePathCollection дуговой фигуры
            ShapePathCollection shapePaths = customShape.Paths;

            if (shapePaths != null)
            {
                // Добавить новый путь в ShapePathCollection
                int pathIndex = shapePaths.Add();

                // Получить доступ к только что добавленному ShapePath
                ShapePath newPath = shapePaths[pathIndex];

                // Отобразить количество путей в ShapePathCollection
                Console.WriteLine("Number of paths in the ShapePathCollection: " + shapePaths.Count);
            }
            

            // Сохраните книгу
            workbook.Save("ShapePathCollectionExample.xlsx");
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ShapePath](../shapepath/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


