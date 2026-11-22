---
title: "Shape.LineFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الشكل. تعيد كائن MsoLineFormat يحتوي على خصائص تنسيق الخط للشكل المحدد"
type: docs
url: /ar/net/aspose.cells.drawing/shape/lineformat/
---
## Shape.LineFormat property

يعيد كائن MsoLineFormat يحتوي على خصائص تنسيق الخط للشكل المحدد.

```csharp
[Obsolete("Use Shape.Line property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoLineFormat LineFormat { get; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام خاصية Shape.Line. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2016. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLineFormatDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف شكل مستطيل إلى الورقة الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            RectangleShape rectangle = worksheet.Shapes.AddRectangle(3, 0, 2, 0, 70, 130);
            
            // تعيين خصائص الشكل
            rectangle.Placement = PlacementType.FreeFloating;
            rectangle.Fill.FillType = FillType.Solid;
            rectangle.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            
            // عرض مثال لاستخدام LineFormat
            rectangle.LineFormat.Weight = 3; // Set line weight
            rectangle.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            rectangle.Line.SolidFill.Color = System.Drawing.Color.DarkBlue; // Correct way to set line color
            
            // احفظ المصنف
            workbook.Save("ShapeLineFormatDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [MsoLineFormat](../../msolineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


