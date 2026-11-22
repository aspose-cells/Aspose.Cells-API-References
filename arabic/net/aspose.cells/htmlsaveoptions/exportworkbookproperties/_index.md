---
title: "HtmlSaveOptions.ExportWorkbookProperties"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "HtmlSaveOptions property. تشير إلى ما إذا كان يتم تصدير خصائص المصنف. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel يرجى الحفاظ على القيمة الافتراضية"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/exportworkbookproperties/
---
## HtmlSaveOptions.ExportWorkbookProperties property

تشير إلى ما إذا كان يتم تصدير خصائص دفتر العمل. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية.

```csharp
public bool ExportWorkbookProperties { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportWorkbookPropertiesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة بعض البيانات إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // تعيين خصائص المصنف
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Title";

            // إنشاء خيارات حفظ HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // إظهار ExportWorkbookProperties عن طريق تعيينه إلى false
            options.ExportWorkbookProperties = false;
            
            // حفظ المصنف كملف HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with ExportWorkbookProperties set to false");
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


