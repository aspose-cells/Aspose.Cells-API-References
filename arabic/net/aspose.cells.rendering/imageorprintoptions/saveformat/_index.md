---
title: "ImageOrPrintOptions.SaveFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. تحصل أو تضبط نوع تنسيق ملف الإخراج، يدعم Tiff/XPS"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/saveformat/
---
## ImageOrPrintOptions.SaveFormat property

تحصل أو تضبط نوع تنسيق ملف الإخراج، يدعم Tiff/XPS

```csharp
[Obsolete("For Tiff/Svg, use ImageType; For Xps, use Workbook.Save(string, SaveOptions) with XpsSaveOptions")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SaveFormat SaveFormat { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، بالنسبة لـ Tiff/Svg، استخدم [`ImageType`](../imagetype/); بالنسبة لـ Xps، استخدم [`Save`](../../../aspose.cells/workbook/save/) مع [`XpsSaveOptions`](../../../aspose.cells/xpssaveoptions/). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أغسطس 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واملأه ببيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells SaveFormat Demonstration");
            
            // أنشئ مثيلًا لـ ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // عرض قيمة SaveFormat الأولية
            Console.WriteLine("Initial SaveFormat: " + options.SaveFormat);

            // تعيين SaveFormat إلى TIFF وتحويل ورقة العمل
            options.SaveFormat = SaveFormat.Tiff;
            SheetRender tiffRenderer = new SheetRender(worksheet, options);
            using (FileStream tiffStream = new FileStream("output.tiff", FileMode.Create))
            {
                tiffRenderer.ToTiff(tiffStream);
            }
            Console.WriteLine("Rendered worksheet to TIFF format");

            // تغيير SaveFormat إلى XPS وتحويل مرة أخرى
            options.SaveFormat = SaveFormat.Xps;
            SheetRender xpsRenderer = new SheetRender(worksheet, options);
            using (FileStream xpsStream = new FileStream("output.xps", FileMode.Create))
            {
                // ملاحظة: SheetRender لا يدعم تنسيق XPS. سيتم حفظه كتنسيق صورة بدلاً من ذلك.
                xpsRenderer.ToImage(0, xpsStream);
            }
            Console.WriteLine("Rendered worksheet to XPS format");
        }
    }
}
```

### انظر أيضًا

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


