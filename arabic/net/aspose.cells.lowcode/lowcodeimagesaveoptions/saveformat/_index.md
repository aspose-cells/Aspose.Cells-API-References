---
title: "LowCodeImageSaveOptions.SaveFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeImageSaveOptions. تحصل على أو تعيين تنسيق الحفظ"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodeimagesaveoptions/saveformat/
---
## LowCodeImageSaveOptions.SaveFormat property

يحصل أو يحدد تنسيق الحفظ.

```csharp
public override SaveFormat SaveFormat { get; set; }
```

### ملاحظات

إذا تم تحديد [`ImageOptions`](../imageoptions/)، فإن ضبط هذه الخاصية سيغير أيضًا قيمة [`ImageType`](../../../aspose.cells.rendering/imageorprintoptions/imagetype/) الخاصة بها.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeImageSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells LowCode Image SaveFormat Demo");

            // تهيئة LowCodeImageSaveOptions بالقيم الافتراضية
            LowCodeImageSaveOptions options = new LowCodeImageSaveOptions();
            
            // عرض تنسيق SaveFormat الأولي (الافتراضي هو Png)
            Console.WriteLine("Initial SaveFormat: " + options.SaveFormat);

            // تكوين للإخراج بصيغة JPEG
            options.SaveFormat = SaveFormat.Jpg;
            options.ImageOptions = new ImageOrPrintOptions
            {
                Quality = 85,
                OnePagePerSheet = true,
                ImageType = ImageType.Jpeg
            };
            SaveWorksheetAsImage(worksheet, options, "output_initial.jpg");

            // تغيير إلى تنسيق PNG وحفظ مرة أخرى
            options.SaveFormat = SaveFormat.Png;
            options.ImageOptions.ImageType = ImageType.Png;
            Console.WriteLine("\nModified SaveFormat: " + options.SaveFormat);
            SaveWorksheetAsImage(worksheet, options, "output_modified.png");
        }

        private static void SaveWorksheetAsImage(Worksheet worksheet, LowCodeImageSaveOptions options, string fileName)
        {
            // تصيير ورقة العمل باستخدام الخيارات المُكوَّنة
            SheetRender renderer = new SheetRender(worksheet, options.ImageOptions);
            renderer.ToImage(0, fileName);
            Console.WriteLine($"Saved: {fileName}");
        }
    }
}
```

### انظر أيضًا

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


