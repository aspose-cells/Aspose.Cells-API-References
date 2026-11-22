---
title: "TilePicOption.MirrorType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TilePicOption. تحصل أو تعين نوع المرآة للتكرار"
type: docs
url: /ar/net/aspose.cells.drawing/tilepicoption/mirrortype/
---
## TilePicOption.MirrorType property

يحصل أو يضبط نوع المرآة للبلاط.

```csharp
public MirrorType MirrorType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TilePicOptionPropertyMirrorTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلاً مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 500, 500, 500);

            // تحميل بيانات صورة تجريبية (استبدل بمسار الصورة الفعلي)
            byte[] imageData = File.ReadAllBytes("sample.png");

            // أنشئ وقم بتهيئة كائن TilePicOption
            TilePicOption tileOptions = new TilePicOption();

            // عرض قيمة MirrorType الأولية
            Console.WriteLine("Current MirrorType: " + tileOptions.MirrorType);

            // قم بتكوين خيارات التجانب
            tileOptions.ScaleX = 0.5;
            tileOptions.ScaleY = 0.5;
            tileOptions.MirrorType = MirrorType.Both;

            // تطبيق تكوين البلاط باستخدام الخصائص الصحيحة
            shape.Fill.FillType = FillType.Texture;
            shape.Fill.ImageData = imageData;
            shape.Fill.TextureFill.TilePicOption = tileOptions;

            // احفظ المصنف المعدل
            workbook.Save("TilePicOptionMirrorTypeDemo.xlsx");

            Console.WriteLine("Updated MirrorType: " + tileOptions.MirrorType);
        }
    }
}
```

### انظر أيضًا

* enum [MirrorType](../../mirrortype/)
* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


