---
title: "MsoFillFormat.Texture"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoFillFormat. تحصل على نوع تعبئة النسيج"
type: docs
url: /ar/net/aspose.cells.drawing/msofillformat/texture/
---
## MsoFillFormat.Texture property

الحصول على نوع ملء النسيج.

```csharp
public TextureType Texture { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFillFormatPropertyTextureDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل مستطيل لتوضيح تنسيق التعبئة
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // احصل على تنسيق التعبئة
            MsoFillFormat fillFormat = rectangle.FillFormat;

            try
            {
                // اعرض نوع النسيج الحالي (خاصية للقراءة فقط)
                TextureType currentTexture = fillFormat.Texture;
                Console.WriteLine("Current Texture Type: " + currentTexture);

                // اضبط بعض بيانات الصورة لتغيير النسيج محتملًا
                // هذا يوضح كيف يمكن أن يتأثر النسيج ببيانات الصورة
                byte[] sampleImageData = new byte[] { 0x89, 0x50, 0x4E, 0x47 }; // PNG header
                fillFormat.ImageData = sampleImageData;

                // اعرض نوع النسيج مرة أخرى بعد ضبط بيانات الصورة
                TextureType updatedTexture = fillFormat.Texture;
                Console.WriteLine("Texture Type after setting image data: " + updatedTexture);

                // احفظ المصنف
                workbook.Save("TextureDemo.xlsx");
                Console.WriteLine("Texture demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [TextureType](../../texturetype/)
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


