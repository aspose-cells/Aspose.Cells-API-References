---
title: "TextureFill.Scale"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextureFill. تحصل وتضبط مقياس تنسيق الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/texturefill/scale/
---
## TextureFill.Scale property

يحصل على ويضبط مقياس تنسيق الصورة.

```csharp
public double Scale { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TextureFillPropertyScaleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً واحصل على تنسيق التعبئة الخاص به
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 10, 10, 500, 300);
            FillFormat fillFormat = shape.Fill;

            // تكوين ملء الملمس
            fillFormat.FillType = FillType.Texture;
            TextureFill textureFill = fillFormat.TextureFill;

            // تحميل صورة الملمس وتكوين الخصائص
            textureFill.ImageData = File.ReadAllBytes("texture.jpg");
            textureFill.Type = TextureType.Unknown; // Changed from UserDefined to Unknown
            textureFill.IsTiling = true;

            // عرض وتعديل المقياس
            Console.WriteLine("Initial Scale: " + textureFill.Scale);
            textureFill.Scale = 0.5;
            Console.WriteLine("Modified Scale: " + textureFill.Scale);

            // حفظ النتيجة
            workbook.Save("TextureFillScaleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


