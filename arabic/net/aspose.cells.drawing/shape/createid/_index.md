---
title: "Shape.CreateId"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تحصل وتضبط CreateId لهذا الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/createid/
---
## Shape.CreateId property

يحصل ويضبط معرف الإنشاء لهذا shape.

```csharp
public Guid CreateId { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyCreateIdDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة شكل مستطيل
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 200, 150);
            
            // أنشئ وعيّن GUID جديد كـ CreateId
            Guid createId = Guid.NewGuid();
            shape.CreateId = createId;
            
            // احفظ المصنف
            workbook.Save("ShapeCreateIdDemo.xlsx");
            
            // أعد تحميل المصنف للتحقق من بقاء CreateId
            Workbook loadedWorkbook = new Workbook("ShapeCreateIdDemo.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            
            // أخرج CreateId للتحقق
            Console.WriteLine("Original CreateId: " + createId);
            Console.WriteLine("Loaded CreateId: " + loadedShape.CreateId);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


