---
title: "Sınıf ShapePathCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ShapePathCollection sınıfı. NotPrimitive otomatik şekil içinde yol koleksiyonu bilgilerini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shapepathcollection/
---
## ShapePathCollection class

NotPrimitive otomatik şekilde yol koleksiyonu bilgilerini temsil eder.

```csharp
public class ShapePathCollection : CollectionBase<ShapePath>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells.drawing/shapepathcollection/count/) { get; } | Yolların sayısını alır |
| [Item](../../aspose.cells.drawing/shapepathcollection/item/) { get; } | Bir oluşturma yolunu alır. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells.drawing/shapepathcollection/add/)() | Bir oluşturma yolu ekle. |
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

### Örnekler

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



            // Yeni bir Workbook örneği oluşturun
            Workbook workbook = new Workbook("ShapePathCollectionExample_original.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];

            Shape customShape = worksheet.Shapes[0];
            
            // Yay şeklinin ShapePathCollection'ına erişin
            ShapePathCollection shapePaths = customShape.Paths;

            if (shapePaths != null)
            {
                // ShapePathCollection'a yeni bir yol ekle
                int pathIndex = shapePaths.Add();

                // Yeni eklenen ShapePath'e erişin
                ShapePath newPath = shapePaths[pathIndex];

                // ShapePathCollection içindeki yolların sayısını göster
                Console.WriteLine("Number of paths in the ShapePathCollection: " + shapePaths.Count);
            }
            

            // Çalışma kitabını kaydedin
            workbook.Save("ShapePathCollectionExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ShapePath](../shapepath/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


