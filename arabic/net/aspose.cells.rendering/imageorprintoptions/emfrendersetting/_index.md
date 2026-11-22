---
title: "ImageOrPrintOptions.EmfRenderSetting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. إعداد لتصيير ملفات ميتا Emf في ملف المصدر"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/emfrendersetting/
---
## ImageOrPrintOptions.EmfRenderSetting property

إعداد لتصوير ملفات Emf الميتا في الملف المصدر.

```csharp
public EmfRenderSetting EmfRenderSetting { get; set; }
```

### ملاحظات

ملفات EMF المعرّفة باسم \"EMF+ Dual\" يمكن أن تحتوي على كلٍ من سجلات EMF+ وسجلات EMF. يمكن استخدام أي نوع من السجلات لتصيير الصورة، إما سجلات EMF+ فقط، أو سجلات EMF فقط. عندما يتم تعيين EmfPlusPrefer، سيتم تحليل سجلات EMF+ أثناء تصيير الصورة، وإلا سيتم تحليل سجلات EMF فقط. القيمة الافتراضية هي EmfOnly. بالنسبة للأطر التي تعتمد على .NET System.Drawing.Common، يتم تجاهل هذا الإعداد.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyEmfRenderSettingDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد بمحتوى اختبار
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "EMF Rendering Setting Test";
            worksheet.Cells["C5"].Value = "Sample Content for Image Rendering";

            // إنشاء خيارات تصيير الصورة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.TiffCompression = TiffCompression.CompressionLZW;

            // عرض الإعداد الحالي
            Console.WriteLine("Default EmfRenderSetting: " + options.EmfRenderSetting);

            // تصيير باستخدام إعدادات EMF الافتراضية
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "DefaultEmfSetting.tiff");

            // غيّر إعداد عرض EMF وأعد العرض مرة أخرى
            options.EmfRenderSetting = EmfRenderSetting.EmfPlusPrefer;
            Console.WriteLine("\nModified EmfRenderSetting: " + options.EmfRenderSetting);

            SheetRender modifiedRenderer = new SheetRender(worksheet, options);
            modifiedRenderer.ToImage(0, "ModifiedEmfSetting.tiff");

            Console.WriteLine("\nGenerated TIFF images demonstrating EMF rendering settings.");
        }
    }
}
```

### انظر أيضًا

* enum [EmfRenderSetting](../../../aspose.cells/emfrendersetting/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


