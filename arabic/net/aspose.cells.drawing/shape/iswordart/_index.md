---
title: "Shape.IsWordArt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تشير إلى ما إذا كان هذا الشكل فن كلمة"
type: docs
url: /ar/net/aspose.cells.drawing/shape/iswordart/
---
## Shape.IsWordArt property

يشير إلى ما إذا كان هذا الشكل فن كلمة.

```csharp
public bool IsWordArt { get; }
```

### ملاحظات

فقط للشكل القديم لملف xls.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsWordArtDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً من نوع WordArt مع جميع المعلمات المطلوبة
            Shape wordArt = worksheet.Shapes.AddWordArt(PresetWordArtStyle.WordArtStyle1, "Sample WordArt", 0, 0, 100, 100, 100, 100);

            // أضف شكلاً مستطيلاً عاديًا مع جميع المعلمات المطلوبة
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 150, 100, 100, 100);

            // تحقق مما إذا كانت الأشكال WordArt
            Console.WriteLine("WordArt shape is WordArt: " + wordArt.IsWordArt);
            Console.WriteLine("Rectangle shape is WordArt: " + rectangle.IsWordArt);

            // مثال على استخدام خاصية IsWordArt
            if (wordArt.IsWordArt)
            {
                Console.WriteLine("First shape is a WordArt object");
            }

            if (!rectangle.IsWordArt)
            {
                Console.WriteLine("Second shape is not a WordArt object");
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


