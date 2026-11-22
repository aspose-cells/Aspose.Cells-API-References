---
title: "الفئة ShapeSegmentPathCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.ShapeSegmentPathCollection. تمثل مسار إنشاء يتكون من سلسلة من الحركات والخطوط والمنحنيات التي عند دمجها ستشكل شكلًا هندسيًا"
type: docs
url: /ar/net/aspose.cells.drawing/shapesegmentpathcollection/
---
## ShapeSegmentPathCollection class

يمثل مسار إنشاء يتكون من سلسلة من الحركات والخطوط والمنحنيات التي عند دمجها ستشكل شكلاً هندسياً.

```csharp
public class ShapeSegmentPathCollection : CollectionBase<ShapeSegmentPath>
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ShapeSegmentPathCollection](shapesegmentpathcollection/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/shapesegmentpathcollection/item/) { get; } | يحصل على كائن [`ShapeSegmentPath`](../shapesegmentpath/). |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells.drawing/shapesegmentpathcollection/add/)(ShapePathType) | أضف مسار مقطع في مسار الإنشاء. |
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

### أمثلة

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
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // أنشئ ShapePath للعمل مع المقاطع
                ShapePath path = new ShapePath();

                // ابدأ مسارًا جديدًا
                path.MoveTo(10, 10);

                // ارسم مقطع خط
                path.LineTo(100, 100);

                // احصل على ShapeSegmentPathCollection من المسار
                ShapeSegmentPathCollection segmentPaths = path.PathSegementList;

                // إضافة مقطع مسار مغلق
                int index = segmentPaths.Add(ShapePathType.Close);

                // عرض معلومات حول المجموعة
                Console.WriteLine($"Number of path segments: {segmentPaths.Count}");
                Console.WriteLine($"Added segment at index: {index}");

                // الوصول إلى المقطع الأول (خاصية للقراءة فقط)
                if (segmentPaths.Count > 0)
                {
                    ShapeSegmentPath firstSegment = segmentPaths[0];
                    Console.WriteLine($"First segment type: {firstSegment.Type}");
                }

                // إضافة الشكل إلى ورقة العمل
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });

                // احفظ المصنف
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

### انظر أيضًا

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ShapeSegmentPath](../shapesegmentpath/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


