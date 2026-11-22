---
title: "Shape.IsDecorative"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تشير إلى ما إذا كان الكائن زخرفيًا"
type: docs
url: /ar/net/aspose.cells.drawing/shape/isdecorative/
---
## Shape.IsDecorative property

يشير إلى ما إذا كان الكائن زخرفيًا.

```csharp
public bool IsDecorative { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsDecorativeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة شكل مستطيل
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            
            // عيّن الشكل كزخرفي
            shape.IsDecorative = true;
            
            // احفظ المصنف
            string outputPath = "ShapeIsDecorativeDemo.xlsx";
            workbook.Save(outputPath);
            
            // أعد تحميل المصنف للتحقق من الخاصية
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            
            // أخرج النتيجة.
            Console.WriteLine("Shape IsDecorative property: " + loadedShape.IsDecorative);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


