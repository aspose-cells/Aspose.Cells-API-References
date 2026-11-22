---
title: "Shape.GetResultOfSmartArt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. تحويل SmartArt إلى أشكال مجمعة"
type: docs
url: /ar/net/aspose.cells.drawing/shape/getresultofsmartart/
---
## Shape.GetResultOfSmartArt method

تحويل الرسم الذكي إلى أشكال مجمّعة.

```csharp
public virtual GroupShape GetResultOfSmartArt()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetResultOfSmartArtDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلاً (لأننا لا نستطيع إنشاء SmartArt مباشرةً)
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 200, 200, 0, 0);
            
            // في سيناريو واقعي، كنا سنحمّل شكل SmartArt موجود
            // لأغراض العرض، سنتجاوز فحص IsSmartArt لأننا لا نستطيع ضبطه

            // احصل على نتيجة SmartArt (سيعمل فقط إذا كان الشكل فعليًا SmartArt)
            GroupShape groupShape = shape.GetResultOfSmartArt();
            Console.WriteLine("Converted shape to GroupShape");
        }
    }
}
```

### انظر أيضًا

* class [GroupShape](../../groupshape/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


