---
title: "الفئة Geometry"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.Geometry. تمثل شكلاً هندسيًا"
type: docs
url: /ar/net/aspose.cells.drawing/geometry/
---
## Geometry class

يمثل شكلاً هندسياً.

```csharp
public abstract class Geometry
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ShapeAdjustValues](../../aspose.cells.drawing/geometry/shapeadjustvalues/) { get; } | يحصل على مجموعة من قيم تعديل الشكل |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    
    public class DrawingClassGeometryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلًا إلى ورقة العمل
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // الوصول إلى هندسة الشكل
            Geometry geometry = rectangle.Geometry;

            // أضف أدلة تعديل الشكل مباشرة إلى المجموعة
            geometry.ShapeAdjustValues.Add("Roundness", 0.3);
            geometry.ShapeAdjustValues.Add("Angle", 45.0);

            // احفظ المصنف المعدل
            workbook.Save("GeometryDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


