---
title: "TextureFill.PictureFormatType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextureFill. تحصل وتضبط نوع تنسيق الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/texturefill/pictureformattype/
---
## TextureFill.PictureFormatType property

يحصل ويضبط نوع تنسيق الصورة.

```csharp
public FillPictureType PictureFormatType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyPictureFormatTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلاً مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // تعيين نوع التعبئة إلى نقش
            shape.Fill.FillType = FillType.Texture;
            TextureFill textureFill = shape.Fill.TextureFill;

            // تحميل صورة PNG بحد أدنى 1×1 بكسل (أبيض)
            string base64Image = "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=";
            textureFill.ImageData = Convert.FromBase64String(base64Image);

            // عرض نوع PictureFormatType الحالي
            Console.WriteLine("Initial PictureFormatType: " + textureFill.PictureFormatType);

            // تغيير إلى تنسيق مكدس وتمكين التكرار
            textureFill.PictureFormatType = FillPictureType.Stack;
            textureFill.IsTiling = true;

            // أضف شكلاً آخر لمقارنة التنسيق الأصلي الممدد
            Shape shape2 = worksheet.Shapes.AddRectangle(0, 0, 210, 0, 100, 200);
            shape2.Fill.FillType = FillType.Texture;
            TextureFill textureFill2 = shape2.Fill.TextureFill;
            textureFill2.ImageData = Convert.FromBase64String(base64Image);

            // حفظ المصنف مع مثالَي ملء الملمس
            workbook.Save("TextureFillPictureFormatTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [FillPictureType](../../fillpicturetype/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


