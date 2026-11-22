---
title: "ImageOrPrintOptions.IsCellAutoFit"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. تشير إلى ما إذا كان عرض وارتفاع الخلايا يتم ضبطهما تلقائيًا وفقًا لقيمة الخلية. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/iscellautofit/
---
## ImageOrPrintOptions.IsCellAutoFit property

تشير إلى ما إذا كان عرض وارتفاع الخلايا يتم ضبطهما تلقائيًا وفقًا لقيمة الخلية. القيمة الافتراضية هي false.

```csharp
[Obsolete("This property is not used, please remove this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsCellAutoFit { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، هذه الخاصية غير مستخدمة، يرجى إزالة هذه الخاصية.. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أغسطس 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyIsCellAutoFitDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين نص عينة يتجاوز عرض العمود الافتراضي
            worksheet.Cells["B4"].Value = "This is a long text that demonstrates cell autofit behavior when converting to image.";
            
            // إنشاء خيارات تصيير الصورة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // عرض IsCellAutoFit كقيمة false (افتراضي)
            Console.WriteLine("Default IsCellAutoFit value: " + options.IsCellAutoFit);
            SaveAsImage(worksheet, options, "WithoutAutoFit.png");

            // تغيير IsCellAutoFit إلى true
            options.IsCellAutoFit = true;
            Console.WriteLine("Modified IsCellAutoFit value: " + options.IsCellAutoFit);
            SaveAsImage(worksheet, options, "WithAutoFit.png");

            Console.WriteLine("Images created successfully. Compare column widths in output files.");
        }

        private static void SaveAsImage(Worksheet worksheet, ImageOrPrintOptions options, string fileName)
        {
            // تكوين تنسيق الصورة
            options.ImageType = ImageType.Png;

            // تصيير ورقة العمل إلى صورة باستخدام الخيارات المحددة
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, fileName);
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


