---
title: "HtmlSaveOptions.ExportRowColumnHeadings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان سيتم تصدير عناوين الصفوف والأعمدة للأوراق عند الحفظ إلى ملفات HTML"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/exportrowcolumnheadings/
---
## HtmlSaveOptions.ExportRowColumnHeadings property

تشير إلى ما إذا كان يتم تصدير رؤوس الصفوف والأعمدة للورقة عند الحفظ إلى ملفات HTML.

```csharp
public bool ExportRowColumnHeadings { get; set; }
```

### ملاحظات

القيمة الافتراضية هي false.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportRowColumnHeadingsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);

            // إنشاء خيارات حفظ HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // ضبط ExportRowColumnHeadings على false (القيمة الافتراضية هي true)
            saveOptions.ExportRowColumnHeadings = false;

            // احفظ المصنف مع تعطيل العناوين
            workbook.Save("output_without_headings.html", saveOptions);

            // الآن فعّل العناوين واحفظ مرة أخرى
            saveOptions.ExportRowColumnHeadings = true;
            workbook.Save("output_with_headings.html", saveOptions);

            Console.WriteLine("HTML files saved with different heading visibility settings.");
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


