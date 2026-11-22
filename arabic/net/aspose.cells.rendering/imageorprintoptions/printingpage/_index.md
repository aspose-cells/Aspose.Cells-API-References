---
title: "ImageOrPrintOptions.PrintingPage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. تشير إلى الصفحات التي لن يتم طباعتها"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/printingpage/
---
## ImageOrPrintOptions.PrintingPage property

يشير إلى الصفحات التي لن تُطبع.

```csharp
public PrintingPageType PrintingPage { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPrintingPageDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Test Data");
            worksheet.Cells["A2"].PutValue("Non-Blank Cell");
            worksheet.Cells["A5"].PutValue("Another Non-Blank Cell");
            
            // إنشاء خيارات الصورة/الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.IgnoreBlank;
            
            // قم بعرض دفتر العمل باستخدام الخيارات
            WorkbookRender render = new WorkbookRender(workbook, options);
            
            // أخرج عدد الصفحات (سيتجاهل الصفحات الفارغة)
            Console.WriteLine("Page count with IgnoreBlank: " + render.PageCount);
            
            // غيّر إلى السلوك الافتراضي (تضمين جميع الصفحات)
            options.PrintingPage = PrintingPageType.Default;
            render = new WorkbookRender(workbook, options);
            Console.WriteLine("Page count with Default: " + render.PageCount);
        }
    }
}
```

### انظر أيضًا

* enum [PrintingPageType](../../../aspose.cells/printingpagetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


