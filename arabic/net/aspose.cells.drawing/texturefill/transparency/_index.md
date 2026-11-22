---
title: "TextureFill.Transparency"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextureFill. تعيد أو تضبط درجة شفافية المنطقة كقيمة من 0.0 غير شفاف إلى 1.0 شفاف"
type: docs
url: /ar/net/aspose.cells.drawing/texturefill/transparency/
---
## TextureFill.Transparency property

يعيد أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف).

```csharp
public double Transparency { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyTransparencyDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلًا إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // تعيين نوع التعبئة إلى نقش
            shape.Fill.FillType = FillType.Texture;

            // الوصول إلى خصائص تعبئة النسيج
            TextureFill textureFill = shape.Fill.TextureFill;

            // تعيين نوع نسيج مدمج
            textureFill.Type = TextureType.BlueTissuePaper;

            // عرض قيمة الشفافية الأولية
            Console.WriteLine("Initial Transparency: " + textureFill.Transparency);

            // تغيير الشفافية إلى 70% (0.0 = غير شفاف، 1.0 = شفاف بالكامل)
            textureFill.Transparency = 0.7;
            Console.WriteLine("Updated Transparency: " + textureFill.Transparency);

            // حفظ المصنف مع تأثير شفافية مرئي
            workbook.Save("TextureFillTransparencyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


