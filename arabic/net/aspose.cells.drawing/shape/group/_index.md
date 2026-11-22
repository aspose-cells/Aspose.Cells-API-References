---
title: "Shape.Group"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تحصل على شكل المجموعة الذي يحتوي هذا الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/group/
---
## Shape.Group property

يحصل على مجموعة الأشكال التي تحتوي على هذا الشكل.

```csharp
public GroupShape Group { get; }
```

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyGroupDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إنشاء شكلين تجريبيين
            Shape shape1 = sheet.Shapes.AddRectangle(0, 0, 0, 100, 100, 0);
            Shape shape2 = sheet.Shapes.AddOval(0, 100, 100, 100, 100, 0);

            // تجميع الأشكال باستخدام معلمة مصفوفة Shape
            GroupShape group = sheet.Shapes.Group(new Shape[] { shape1, shape2 });

            // الوصول إلى المجموعة عبر خاصية Group للشكل الفرعي
            GroupShape retrievedGroup = shape1.Group;
            
            // إظهار استخدام خاصية Group
            retrievedGroup.Name = "MyShapeGroup";
            retrievedGroup.Placement = PlacementType.FreeFloating;

            workbook.Save("GroupShapeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [GroupShape](../../groupshape/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


