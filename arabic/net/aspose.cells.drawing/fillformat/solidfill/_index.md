---
title: "FillFormat.SolidFill"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FillFormat. يحصل على كائن SolidFill"
type: docs
url: /ar/net/aspose.cells.drawing/fillformat/solidfill/
---
## FillFormat.SolidFill property

يحصل على كائن `SolidFill`.

```csharp
public SolidFill SolidFill { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertySolidFillDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة شكل مستطيل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            
            // تعيين لون التعبئة الصلبة للشكل
            shape.Fill.SolidFill.Color = System.Drawing.Color.FromArgb(135, 222, 255);
            
            // احصل على وعرض لون التعبئة الصلبة
            System.Drawing.Color fillColor = shape.Fill.SolidFill.Color;
            Console.WriteLine("Solid Fill Color - R:{0}, G:{1}, B:{2}", 
                fillColor.R, fillColor.G, fillColor.B);
            
            // احفظ المصنف
            workbook.Save("SolidFillDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SolidFill](../../solidfill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


