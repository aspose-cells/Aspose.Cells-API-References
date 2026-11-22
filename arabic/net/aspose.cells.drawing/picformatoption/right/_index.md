---
title: "PicFormatOption.Right"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PicFormatOption. يحصل أو يحدد الإزاحة اليمنى لتمديد الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/picformatoption/right/
---
## PicFormatOption.Right property

يحصل أو يضبط الإزاحة اليمنى لتمديد الصورة.

```csharp
public double Right { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyRightDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل مستطيل بالأبعاد المحددة
            Shape shape = worksheet.Shapes.AddRectangle(5, 2, 10, 10, 150, 300);

            // قم بتكوين تعبئة الصورة للشكل
            shape.Fill.FillType = FillType.Texture;
            string imagePath = "sample.jpg"; // Replace with actual image path
            
            if (File.Exists(imagePath))
            {
                shape.Fill.ImageData = File.ReadAllBytes(imagePath);
            }
            else
            {
                Console.WriteLine("Image not found - using empty picture fill");
            }

            // الوصول إلى خيارات تنسيق الصورة عبر TextureFill
            PicFormatOption picFormat = shape.Fill.TextureFill.PicFormatOption;

            // اعرض وعدل خاصية Right
            Console.WriteLine("Initial Right offset: " + picFormat.Right);
            picFormat.Right = 25.5; // Set right offset to 25.5 units

            // تحقق من القيمة الجديدة واحفظ التغييرات
            Console.WriteLine("Updated Right offset: " + picFormat.Right);
            workbook.Save("RightPropertyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


