---
title: "PdfSaveOptions.ImageType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfSaveOptions. تمثّل نوع الصورة عند تحويل المخطط والشكل"
type: docs
url: /ar/net/aspose.cells/pdfsaveoptions/imagetype/
---
## PdfSaveOptions.ImageType property

تمثّل نوع الصورة عند تحويل المخطط والشكل.

```csharp
[Obsolete("Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ImageFormat ImageType { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يتم دائمًا عرض المخطط والشكل كعناصر متجهة (مثل النقطة، الخط) لضمان جودة العرض. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing.Imaging;

    public class PdfSaveOptionsPropertyImageTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // أنشئ ورقة عمل نموذجية تحتوي على بعض البيانات
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data for PDF Export";
            worksheet.Cells["A2"].Value = "Demonstrating ImageType Property";

            try
            {
                // أنشئ خيارات حفظ PDF
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // اعرض قيمة ImageType الافتراضية
                Console.WriteLine("Default ImageType: " + saveOptions.ImageType);

                // عيّن قيمة ImageType مختلفة
                saveOptions.ImageType = ImageFormat.Png;
                Console.WriteLine("Updated ImageType: " + saveOptions.ImageType);

                // احفظ دفتر العمل كملف PDF باستخدام ImageType المحدد
                workbook.Save("ImageTypeDemo.pdf", saveOptions);

                Console.WriteLine("PDF saved with ImageType setting applied.");
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

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


