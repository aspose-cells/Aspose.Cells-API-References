---
title: "Shape.ControlData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تسترجع بيانات التحكم"
type: docs
url: /ar/net/aspose.cells.drawing/shape/controldata/
---
## Shape.ControlData property

يحصل على بيانات التحكم.

```csharp
public byte[] ControlData { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyControlDataDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً بالمعلمات الصحيحة
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            
            // الوصول إلى ControlData (خاصية للقراءة فقط)
            byte[] controlData = shape.ControlData;

            // تحقق من ControlData
            if (controlData != null)
            {
                Console.WriteLine("ControlData exists with length: " + controlData.Length);
            }
            else
            {
                Console.WriteLine("No data.");
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


