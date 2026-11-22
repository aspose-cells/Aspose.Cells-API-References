---
title: "HtmlSaveOptions.ExportDataOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى قاعدة تصدير بيانات ملف HTML. القيمة الافتراضية هي All"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/exportdataoptions/
---
## HtmlSaveOptions.ExportDataOptions property

تشير إلى قاعدة تصدير بيانات ملف html. القيمة الافتراضية هي All.

```csharp
public HtmlExportDataOptions ExportDataOptions { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportDataOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل تجريبي مع بيانات اختبار
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // إنشاء خيارات حفظ HTML وتعيين ExportDataOptions
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions();
            htmlSaveOptions.ExportDataOptions = HtmlExportDataOptions.All;

            // حفظ كـ HTML مع جميع خيارات تصدير البيانات
            workbook.Save("output.html", htmlSaveOptions);

            Console.WriteLine("HTML file saved with ExportDataOptions.All");
        }
    }
}
```

### انظر أيضًا

* enum [HtmlExportDataOptions](../../htmlexportdataoptions/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


