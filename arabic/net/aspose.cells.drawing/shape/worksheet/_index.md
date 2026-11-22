---
title: "Shape.Worksheet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. يحصل على كائن Worksheet الذي يحتوي على هذا الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/worksheet/
---
## Shape.Worksheet property

يحصل على كائن [`Worksheet`](../../../aspose.cells/worksheet/) الذي يحتوي على هذا الشكل.

```csharp
public Worksheet Worksheet { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWorksheetDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة شكل إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            
            // عرض كيفية استخدام خاصية Worksheet
            Worksheet shapeWorksheet = shape.Worksheet;
            
            // أخرج اسم ورقة العمل لإظهار أن الخاصية تعمل
            Console.WriteLine("Shape belongs to worksheet: " + shapeWorksheet.Name);
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


