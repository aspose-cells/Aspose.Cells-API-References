---
title: "ImageOrPrintOptions.EmfType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. تحصل أو تعين قيمة EmfType التي تحدد تنسيق ملف الميتا. القيمة الافتراضية هي EmfPlusDual"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/emftype/
---
## ImageOrPrintOptions.EmfType property

يحصل أو يضبط EmfType الذي يحدد تنسيق ملف الميتا. القيمة الافتراضية هي EmfPlusDual.

```csharp
public EmfType EmfType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertyEmfTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "EMF Type Demo";

            try
            {
                // أنشئ مثيلًا لـ ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // عيّن نوع الصورة إلى EMF
                options.ImageType = Aspose.Cells.Drawing.ImageType.Emf;

                // أنشئ SheetRender باستخدام الخيارات
                SheetRender renderer = new SheetRender(worksheet, options);

                // احفظ بصيغة EMF
                using (MemoryStream stream = new MemoryStream())
                {
                    renderer.ToImage(0, stream);

                    // اعرض قيمة خاصية EmfType
                    Console.WriteLine("EmfType value: " + options.EmfRenderSetting);

                    // احفظ ملف EMF
                    File.WriteAllBytes("output.emf", stream.ToArray());
                    Console.WriteLine("EMF file created successfully.");
                }
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

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


