---
title: "الفئة PictureCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.PictureCollection. تغلف مجموعة من كائنات Picture"
type: docs
url: /ar/net/aspose.cells.drawing/picturecollection/
---
## PictureCollection class

تغلف مجموعة من كائنات [`Picture`](../picture/).

```csharp
public class PictureCollection : CollectionBase<Picture>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/picturecollection/item/) { get; } | يحصل على عنصر [`Picture`](../picture/) في الفهرس المحدد. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_2)(int, int, Stream) | يضيف صورة إلى المجموعة. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_4)(int, int, string) | يضيف صورة إلى المجموعة. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add)(int, int, int, int, Stream) | يضيف صورة إلى المجموعة. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_1)(int, int, int, int, string) | يضيف صورة إلى المجموعة. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_3)(int, int, Stream, int, int) | يضيف صورة إلى المجموعة. |
| [Add](../../aspose.cells.drawing/picturecollection/add/#add_5)(int, int, string, int, int) | يضيف صورة إلى المجموعة. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Picture) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Picture, IComparer&lt;Picture&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Picture, IComparer&lt;Picture&gt;) |  |
| [Camera](../../aspose.cells.drawing/picturecollection/camera/)(int, int, string) | يأخذ صورة للنطاق. |
| [Clear](../../aspose.cells.drawing/picturecollection/clear/#clear)() | امسح جميع الصور. (طريقتان) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Picture) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Picture[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Picture[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Picture[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Picture&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Picture&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Picture&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Picture&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Picture&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Picture&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Picture&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Picture&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Picture&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Picture&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Picture) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Picture, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Picture, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Picture) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Picture, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Picture, int, int) |  |
| [RemoveAt](../../aspose.cells.drawing/picturecollection/removeat/#removeat)(int) | إزالة الأشكال عند الفهرس المحدد (طريقتان) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PictureCollectionDemo
    {
        public static void PictureCollectionExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى في المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى PictureCollection في ورقة العمل
            PictureCollection pictures = worksheet.Pictures;

            // إضافة صورة باستخدام مسار ملف
            int pictureIndex1 = pictures.Add(1, 1, 5, 5, "PictureCollectionExample.jpg");

            // إضافة صورة باستخدام stream
            using (FileStream stream = new FileStream("PictureCollectionExample2.jpg", FileMode.Open))
            {
                int pictureIndex2 = pictures.Add(6, 1, 10, 5, stream);
            }

            // إضافة صورة مع التحجيم
            int pictureIndex3 = pictures.Add(11, 1, "PictureCollectionExample3.jpg", 50, 50);

            // الوصول إلى صورة من المجموعة
            Picture picture = pictures[pictureIndex1];

            // تعديل خصائص الصورة
            picture.Left = 10;
            picture.Top = 10;

            // مسح جميع الصور من المجموعة
            pictures.Clear();

            // حفظ المصنف
            workbook.Save("PictureCollectionExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Picture](../picture/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


