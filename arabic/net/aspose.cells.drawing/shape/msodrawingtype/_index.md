---
title: "Shape.MsoDrawingType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. يحصل على نوع الرسم"
type: docs
url: /ar/net/aspose.cells.drawing/shape/msodrawingtype/
---
## Shape.MsoDrawingType property

يحصل على نوع الرسم.

```csharp
public MsoDrawingType MsoDrawingType { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyMsoDrawingTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل مستطيل (معلمات مصححة)
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);
            
            // احصل على وعرض MsoDrawingType للشكل
            MsoDrawingType drawingType = rectangle.MsoDrawingType;
            Console.WriteLine("Shape MsoDrawingType: " + drawingType.ToString());

            // أضف شكل خط (معلمات مصححة)
            Shape line = worksheet.Shapes.AddLine(3, 0, 3, 100, 150, 1);
            
            // احصل على وعرض MsoDrawingType للخط
            drawingType = line.MsoDrawingType;
            Console.WriteLine("Line MsoDrawingType: " + drawingType.ToString());
        }
    }
}
```

### انظر أيضًا

* enum [MsoDrawingType](../../msodrawingtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


