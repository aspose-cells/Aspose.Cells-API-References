---
title: "فئة ShapeGuideCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Drawing.ShapeGuideCollection. تغلف مجموعة من إرشادات الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shapeguidecollection/
---
## ShapeGuideCollection class

يغلف مجموعة من أدلة الشكل

```csharp
public class ShapeGuideCollection : CollectionBase<ShapeGuide>
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ShapeGuideCollection](shapeguidecollection/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/shapeguidecollection/item/) { get; } | يحصل على إرشاد الشكل حسب الفهرس |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells.drawing/shapeguidecollection/add/)(string, double) | يضيف إرشادًا للشكل.(مهم: هذه الميزة متاحة حاليًا فقط لإصدارات Excel07 وما فوق) |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ShapeGuide) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ShapeGuide, IComparer&lt;ShapeGuide&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ShapeGuide, IComparer&lt;ShapeGuide&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ShapeGuide) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ShapeGuide[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ShapeGuide[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ShapeGuide[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ShapeGuide&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ShapeGuide&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ShapeGuide&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ShapeGuide&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ShapeGuide&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ShapeGuide&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ShapeGuide&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ShapeGuide&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ShapeGuide&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ShapeGuide&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapeGuide) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapeGuide, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ShapeGuide, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapeGuide) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapeGuide, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ShapeGuide, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapeGuideCollectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف شكلًا مخصصًا باستخدام MsoDrawingType صالح واضبط نوعه إلى Rectangle
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 0, 0, 200, 100);
            shape.AutoShapeType = AutoShapeType.Rectangle;
            
            // احصل على ShapeGuideCollection من تعديلات هندسة الشكل
            ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;
            
            // أضف إرشادات شكل جديدة مع الأسماء والقيم
            shapeGuides.Add("Guide1", 0.2);
            shapeGuides.Add("Guide2", 0.5);
            shapeGuides.Add("Guide3", 0.8);
            
            // استرجاع وعرض قيمة الدليل الأول
            ShapeGuide firstGuide = shapeGuides[0];
            Console.WriteLine($"First guide value: {firstGuide.Value}");
            
            // احفظ المصنف
            workbook.Save("ShapeGuideCollectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ShapeGuide](../shapeguide/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


