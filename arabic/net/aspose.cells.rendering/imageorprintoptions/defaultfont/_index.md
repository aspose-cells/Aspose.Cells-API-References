---
title: "ImageOrPrintOptions.DefaultFont"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. عندما تكون الأحرف في Excel هي Unicode ولم يتم تعيين خط صحيح في نمط الخلية قد تظهر ككتل في pdfimage. قم بتعيين DefaultFont مثل MingLiu أو MS Gothic لعرض هذه الأحرف. إذا لم يتم تعيين هذه الخاصية فإن Aspose.Cells سيستخدم الخط الافتراضي للنظام لعرض هذه الأحرف Unicode."
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/defaultfont/
---
## ImageOrPrintOptions.DefaultFont property

عندما تكون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر ككتل في pdf أو صورة. اضبط DefaultFont مثل MingLiu أو MS Gothic لعرض هذه الأحرف. إذا لم يتم ضبط هذه الخاصية، سيستخدم Aspose.Cells الخط الافتراضي للنظام لعرض هذه الأحرف اليونيكود.

```csharp
public string DefaultFont { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyDefaultFontDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة نص عينة إلى الخلية
            worksheet.Cells["A1"].PutValue("Sample Text with Default Font");

            // إنشاء خيارات الصورة وتعيين الخط الافتراضي
            ImageOrPrintOptions imgOptions = new ImageOrPrintOptions
            {
                DefaultFont = "Arial", // Setting default font
                ImageType = ImageType.Png
            };

            // تحويل ورقة العمل إلى صورة
            SheetRender sheetRender = new SheetRender(worksheet, imgOptions);
            sheetRender.ToImage(0, "output.png");

            Console.WriteLine("Image generated with default font setting.");
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


