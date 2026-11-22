---
title: "فئة ShapePath"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Drawing.ShapePath. تمثل مسار إنشاء يتكون من سلسلة من الحركات والخطوط والمنحنيات التي عند تجميعها ستشكل شكلًا هندسيًا"
type: docs
url: /ar/net/aspose.cells.drawing/shapepath/
---
## ShapePath class

يمثل مسار إنشاء يتكون من سلسلة من الحركات والخطوط والمنحنيات التي عند دمجها ستشكل شكلاً هندسياً.

```csharp
public class ShapePath
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ShapePath](shapepath/)() | ينشئ نسخة جديدة من الفئة `ShapePath`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [HeightPixel](../../aspose.cells.drawing/shapepath/heightpixel/) { get; set; } | يحصل على ارتفاع هذا المسار بوحدة البكسل. |
| [PathSegementList](../../aspose.cells.drawing/shapepath/pathsegementlist/) { get; } | (**مهمل.**) يحصل على قائمة [`ShapeSegmentPathCollection`](../shapesegmentpathcollection/) |
| [PathSegments](../../aspose.cells.drawing/shapepath/pathsegments/) { get; } | يحصل على قائمة [`ShapeSegmentPathCollection`](../shapesegmentpathcollection/) |
| [WidthPixel](../../aspose.cells.drawing/shapepath/widthpixel/) { get; set; } | يحصل على عرض هذا المسار بوحدة البكسل. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [ArcTo](../../aspose.cells.drawing/shapepath/arcto/)(float, float, float, float) | يضيف قوسًا بيضاويًا إلى الشكل الحالي. نقطة البداية هي نقطة النهاية للشكل الحالي. |
| [Close](../../aspose.cells.drawing/shapepath/close/)() | يغلق الشكل الحالي ويبدأ شكلًا جديدًا. إذا كان الشكل الحالي يحتوي على سلسلة من الخطوط والمنحنيات المتصلة، فإن الطريقة تغلق الحلقة بربط خط من نقطة النهاية إلى نقطة البداية. |
| [CubicBezierTo](../../aspose.cells.drawing/shapepath/cubicbezierto/)(float, float, float, float, float, float) | يضيف منحنى بيزيه مكعب إلى الشكل الحالي. نقطة البداية هي نقطة النهاية للشكل الحالي. الوحدة: بكسل. |
| [LineTo](../../aspose.cells.drawing/shapepath/lineto/)(float, float) | يضيف مقطع خط إلى الشكل الحالي. نقطة البداية هي نقطة النهاية للشكل الحالي. الوحدة: بكسل. |
| [MoveTo](../../aspose.cells.drawing/shapepath/moveto/)(float, float) | يبدأ شكلًا جديدًا من النقطة المحددة دون إغلاق الشكل الحالي. جميع النقاط اللاحقة المضافة إلى المسار تُضاف إلى هذا الشكل الجديد. الوحدة: بكسل. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapePathDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلًا مخصصًا مع جميع المعلمات المطلوبة
            Shape customShape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 200, 100, 0, 0);
            
            // الوصول إلى ShapePathCollection
            ShapePathCollection shapePaths = customShape.Paths;

            // أضف مسارًا جديدًا وابدأ بالوصول إليه
            int pathIndex = shapePaths.Add();
            ShapePath newPath = shapePaths[pathIndex];

            // إخراج عدد المسارات
            Console.WriteLine("Number of paths in the ShapePathCollection: " + shapePaths.Count.ToString());

            // احفظ المصنف
            workbook.Save("ShapePathDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


