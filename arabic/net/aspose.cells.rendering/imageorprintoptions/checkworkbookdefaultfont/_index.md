---
title: "ImageOrPrintOptions.CheckWorkbookDefaultFont"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. عندما تكون الأحرف في Excel هي Unicode ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر ككتل في pdfimage. اضبط هذه الخاصية إلى true لمحاولة استخدام الخط الافتراضي للدفتر لإظهار هذه الأحرف أولاً"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/
---
## ImageOrPrintOptions.CheckWorkbookDefaultFont property

عندما تكون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر ككتل في pdf أو صورة. اضبط هذا على true لمحاولة استخدام الخط الافتراضي لدفتر العمل لعرض هذه الأحرف أولاً.

```csharp
public bool CheckWorkbookDefaultFont { get; set; }
```

### ملاحظات

القيمة الافتراضية هي true.

### أمثلة

```csharp
using System;
using System.IO;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyCheckWorkbookDefaultFontDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Sample Text");
            
            // حدد الخط الافتراضي لدفتر العمل
            workbook.DefaultStyle.Font.Name = "Arial";
            workbook.DefaultStyle.Font.Size = 12;

            // إنشاء خيارات الصورة أو الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // تمكين التحقق من الخط الافتراضي لدفتر العمل
            options.CheckWorkbookDefaultFont = true;

            // تحويل ورقة العمل إلى صورة
            SheetRender renderer = new SheetRender(sheet, options);
            using (MemoryStream stream = new MemoryStream())
            {
                renderer.ToImage(0, stream);
                
                // احفظ الصورة إلى ملف
                using (FileStream file = new FileStream("output.png", FileMode.Create))
                {
                    stream.WriteTo(file);
                }
            }
            
            Console.WriteLine("Image generated with workbook default font check.");
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


