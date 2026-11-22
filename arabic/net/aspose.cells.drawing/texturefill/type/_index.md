---
title: "TextureFill.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextureFill. تحصل وتعيّن نوع النسيج"
type: docs
url: /ar/net/aspose.cells.drawing/texturefill/type/
---
## TextureFill.Type property

يحصل على ويضبط نوع النسيج

```csharp
public TextureType Type { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلاً لتوضيح تعبئة النسيج
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);

            // تعيين نوع التعبئة إلى نقش
            shape.Fill.FillType = FillType.Texture;

            // الوصول إلى خصائص تعبئة النسيج
            TextureFill textureFill = shape.Fill.TextureFill;

            try
            {
                // اعرض القيمة الأولية للنوع
                Console.WriteLine("Initial Texture Type: " + textureFill.Type);

                // عيّن نوع نسيج مختلف
                textureFill.Type = TextureType.Granite;
                Console.WriteLine("Updated Texture Type: " + textureFill.Type);

                // اعرض مثالًا على نوع نسيج آخر
                textureFill.Type = TextureType.WaterDroplets;
                Console.WriteLine("Final Texture Type: " + textureFill.Type);

                // حفظ المصنف لرؤية التأثير
                workbook.Save("TextureFillTypeDemo.xlsx");
                Console.WriteLine("Texture fill type demonstration completed successfully.");
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
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


