---
title: "TilePicOption.OffsetX"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TilePicOption. تحصل أو تعين إزاحة X لتكرار الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/tilepicoption/offsetx/
---
## TilePicOption.OffsetX property

يحصل أو يضبط إزاحة X لصورة البلاط.

```csharp
public double OffsetX { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TilePicOptionPropertyOffsetXDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلاً لتوضيح التكرار
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);

            // قم بتهيئة تنسيق التعبئة لاستخدام صورة مكررة
            FillFormat fillFormat = rectangle.Fill;
            fillFormat.FillType = FillType.Texture;

            // إنشاء وتكوين TilePicOption
            TilePicOption tileOptions = new TilePicOption();
            
            // اقرأ قيمة OffsetX الأولية
            Console.WriteLine("Current OffsetX value: " + tileOptions.OffsetX);

            // عيّن إزاحة X جديدة لنمط التكرار
            tileOptions.OffsetX = 15.5;

            // طبق خيارات التكرار على تعبئة الشكل
            fillFormat.TextureFill.TilePicOption = tileOptions;

            // حمّل صورة بكسل واحد 1×1 (نقطة حمراء)
            byte[] imageData = Convert.FromBase64String(
                "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            fillFormat.ImageData = imageData;

            // حفظ المصنف المعدل
            workbook.Save("TilePicOptionPropertyOffsetXDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


