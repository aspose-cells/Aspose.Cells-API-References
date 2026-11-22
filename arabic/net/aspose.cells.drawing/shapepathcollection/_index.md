---
title: "الفئة ShapePathCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Drawing.ShapePathCollection. تمثل معلومات مجموعة المسارات في الشكل التلقائي غير البدائي"
type: docs
url: /ar/net/aspose.cells.drawing/shapepathcollection/
---
## ShapePathCollection class

يمثل معلومات مجموعة المسارات في الشكل التلقائي NotPrimitive

```csharp
public class ShapePathCollection : CollectionBase<ShapePath>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells.drawing/shapepathcollection/count/) { get; } | يحصل على عدد المسارات |
| [Item](../../aspose.cells.drawing/shapepathcollection/item/) { get; } | يحصل على مسار الإنشاء. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells.drawing/shapepathcollection/add/)() | أضف مسار إنشاء. |
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

### أمثلة

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



            // إنشاء كائن Workbook جديد
            Workbook workbook = new Workbook("ShapePathCollectionExample_original.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];

            Shape customShape = worksheet.Shapes[0];
            
            // الوصول إلى ShapePathCollection للشكل القوسي
            ShapePathCollection shapePaths = customShape.Paths;

            if (shapePaths != null)
            {
                // أضف مسارًا جديدًا إلى ShapePathCollection
                int pathIndex = shapePaths.Add();

                // الوصول إلى ShapePath المضاف حديثًا
                ShapePath newPath = shapePaths[pathIndex];

                // عرض عدد المسارات في ShapePathCollection
                Console.WriteLine("Number of paths in the ShapePathCollection: " + shapePaths.Count);
            }
            

            // احفظ المصنف
            workbook.Save("ShapePathCollectionExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ShapePath](../shapepath/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


