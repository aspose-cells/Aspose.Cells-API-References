---
title: "TilePicOption.AlignmentType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TilePicOption. تحصل أو تعين المحاذاة للتبليط"
type: docs
url: /ar/net/aspose.cells.drawing/tilepicoption/alignmenttype/
---
## TilePicOption.AlignmentType property

يحصل أو يضبط المحاذاة للبلاط.

```csharp
public RectangleAlignmentType AlignmentType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TilePicOptionPropertyAlignmentTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلاً لتوضيح التكرار
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 300, 300);

            // قم بتهيئة تنسيق التعبئة لاستخدام صورة مكررة
            FillFormat fillFormat = rectangle.Fill;
            fillFormat.FillType = FillType.Texture;

            // إنشاء وتكوين TilePicOption
            TilePicOption tileOptions = new TilePicOption();
            
            // عرض قيمة AlignmentType الأولية
            Console.WriteLine("Current AlignmentType: " + tileOptions.AlignmentType);

            // تعيين المحاذاة إلى أعلى اليمين
            tileOptions.AlignmentType = RectangleAlignmentType.TopRight;
            tileOptions.ScaleX = 0.5;
            tileOptions.ScaleY = 0.5;

            // طبق خيارات التكرار على تعبئة الشكل
            fillFormat.TextureFill.TilePicOption = tileOptions;

            // تحميل صورة عينة (نقطة حمراء بحجم 1×1 بكسل)
            byte[] imageData = Convert.FromBase64String(
                "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            fillFormat.ImageData = imageData;

            // حفظ المصنف المعدل
            workbook.Save("TilePicOptionPropertyAlignmentTypeDemo.xlsx");

            // تغيير المحاذاة إلى أسفل اليسار وحفظ نسخة أخرى
            tileOptions.AlignmentType = RectangleAlignmentType.BottomLeft;
            workbook.Save("TilePicOptionPropertyAlignmentTypeDemo_BottomLeft.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [RectangleAlignmentType](../../rectanglealignmenttype/)
* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


