---
title: "ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. تشير إلى ما إذا كان يجب إخراج صفحة فارغة عندما لا يوجد ما للطباعة"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/
---
## ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint property

يشير إلى ما إذا كان يجب إخراج صفحة فارغة عندما لا يوجد ما للطباعة.

```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```

### ملاحظات

القيمة الافتراضية هي false.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyOutputBlankPageWhenNothingToPrintDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد فارغ
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى التي هي فارغة
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين خيارات الصورة أو الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // عرض خاصية OutputBlankPageWhenNothingToPrint
            options.OutputBlankPageWhenNothingToPrint = true;
            
            // تصيير الورقة
            SheetRender renderer = new SheetRender(worksheet, options);
            
            // ستستمر المخرجات في إنتاج صفحة فارغة واحدة بسبب إعداد الخاصية
            Console.WriteLine("Page count with OutputBlankPageWhenNothingToPrint=true: " + renderer.PageCount);
            
            // احفظ الصفحة الأولى إلى تدفق الذاكرة
            MemoryStream stream = new MemoryStream();
            renderer.ToImage(0, stream);
            Console.WriteLine("Image data length: " + stream.ToArray().Length);
            
            // الآن قم بتعيين الخاصية إلى false
            options.OutputBlankPageWhenNothingToPrint = false;
            SheetRender renderer2 = new SheetRender(worksheet, options);
            
            // ستكون المخرجات الآن بلا صفحات
            Console.WriteLine("Page count with OutputBlankPageWhenNothingToPrint=false: " + renderer2.PageCount);
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


