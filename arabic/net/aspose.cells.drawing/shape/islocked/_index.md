---
title: "Shape.IsLocked"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. يعني True أن الكائن لا يمكن تعديلها عندما تكون الورقة محمية. لاحظ أن هذه القيمة ذات معنى فقط إذا كانت الورقة أو الكائنات في الورقة محمية."
type: docs
url: /ar/net/aspose.cells.drawing/shape/islocked/
---
## Shape.IsLocked property

True يعني أن الكائن لا يمكن تعديلّه عندما تكون الورقة محمية. لاحظ أن هذه القيمة ذات معنى فقط إذا كانت ورقة العمل أو الكائنات في ورقة العمل محمية.

```csharp
public bool IsLocked { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsLockedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // حماية ورقة العمل
            worksheet.Protect(ProtectionType.All);

            // إظهار قفل/إلغاء قفل الشكل
            Console.WriteLine("Original IsLocked state: " + shape.IsLocked);

            // إلغاء قفل الشكل
            shape.IsLocked = false;
            Console.WriteLine("After unlocking, IsLocked state: " + shape.IsLocked);

            // قفل الشكل
            shape.IsLocked = true;
            Console.WriteLine("After locking, IsLocked state: " + shape.IsLocked);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


