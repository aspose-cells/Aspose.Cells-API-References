---
title: "فئة ShapePathPoint"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Drawing.ShapePathPoint. حدد إحداثيات الموقع أو علامات الزاوية. إحداثيات الموقع تمثل إحداثيات مسار في مساحة إحداثية مثل X/Y. علامات الزاوية تشير إلى تغييرات زاوية في مسار مثل الزاوية الابتدائية وزاوية الانحراف لقوس"
type: docs
url: /ar/net/aspose.cells.drawing/shapepathpoint/
---
## ShapePathPoint class

حدد إحداثيات الموقع أو علامات الزاوية. تمثل إحداثيات الموقع إحداثيات مسار في مساحة إحداثية (مثال: X/Y). تشير علامات الزاوية إلى تغييرات زاوية في مسار (مثال: زوايا البداية والامتداد لقوس).

```csharp
public class ShapePathPoint
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Type](../../aspose.cells.drawing/shapepathpoint/type/) { get; } | يحدد نوع القيمة للكائن الحالي. |
| [X](../../aspose.cells.drawing/shapepathpoint/x/) { get; set; } | (**Obsolete.**) يحصل ويضبط إحداثي x لهذا إحداثي الموقع. الوحدة EMUs. |
| [XAngle](../../aspose.cells.drawing/shapepathpoint/xangle/) { get; set; } | عندما يكون الكائن علامة زاوية، احصل أو اضبط الزاوية الأولى بالدرجات. |
| [XPixel](../../aspose.cells.drawing/shapepathpoint/xpixel/) { get; set; } | عندما يكون الكائن إحداثيًا موقعًا، احصل أو اضبط إحداثي x بالبكسل. |
| [Y](../../aspose.cells.drawing/shapepathpoint/y/) { get; set; } | (**Obsolete.**) يحصل على إحداثي y لهذا إحداثي الموقع. الوحدة EMUs. |
| [YAngle](../../aspose.cells.drawing/shapepathpoint/yangle/) { get; set; } | عندما يكون الكائن علامة زاوية، احصل أو اضبط الزاوية الثانية بالدرجات. |
| [YPixel](../../aspose.cells.drawing/shapepathpoint/ypixel/) { get; set; } | عندما يكون الكائن إحداثيًا موقعًا، احصل أو اضبط إحداثي y بالبكسل. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathPointDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // إضافة شكل سيحتوي على نقاط مسار مع جميع المعلمات المطلوبة
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 10, 10, 200, 200);
                
                // احصل على نقاط مسار الهندسة
                CustomGeometry geometry = shape.Geometry as CustomGeometry;
                if (geometry != null && geometry.Paths.Count > 0)
                {
                    ShapePath path = geometry.Paths[0];
                    
                    // الوصول إلى نقطة مسار موجودة (إن وجدت)
                    if (path.PathSegementList.Count > 0)
                    {
                        // احصل على النقطة الأولى (قد تختلف التنفيذ الفعلي بناءً على نوع الجزء)
                        ShapePathPoint point = path.PathSegementList[0].Points[0];
                        
                        // عرض إحداثيات النقطة
                        Console.WriteLine($"ShapePathPoint at X: {point.X}, Y: {point.Y}");
                    }
                }
                
                // احفظ المصنف
                workbook.Save("ShapePathPointDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathPoint: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


