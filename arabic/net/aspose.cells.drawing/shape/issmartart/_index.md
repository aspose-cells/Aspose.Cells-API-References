---
title: "Shape.IsSmartArt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تشير إلى ما إذا كان الشكل فنًا ذكيًا"
type: docs
url: /ar/net/aspose.cells.drawing/shape/issmartart/
---
## Shape.IsSmartArt property

يشير إلى ما إذا كان الشكل فنًا ذكيًا.

```csharp
public bool IsSmartArt { get; }
```

### ملاحظات

فقط لملف ooxml.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsSmartArtDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل SmartArt (ملاحظة: Aspose.Cells لا يتيح إنشاء SmartArt مباشرةً في الإصدارات الحالية)
            // للتوضيح، سنقوم بفحص الأشكال الموجودة
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // تحقق مما إذا كان الشكل SmartArt
            if (shape.IsSmartArt)
            {
                Console.WriteLine("The shape is a SmartArt object");
            }
            else
            {
                Console.WriteLine("The shape is not a SmartArt object");
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


