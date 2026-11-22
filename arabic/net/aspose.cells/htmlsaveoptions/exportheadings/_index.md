---
title: "HtmlSaveOptions.ExportHeadings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان سيتم تصدير عناوين الصفوف والأعمدة للأوراق عند الحفظ إلى ملفات HTML"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/exportheadings/
---
## HtmlSaveOptions.ExportHeadings property

تشير إلى ما إذا كان يتم تصدير رؤوس الصفوف والأعمدة للورقة عند الحفظ إلى ملفات HTML.

```csharp
[Obsolete("Use HtmlSaveOptions.ExportRowColumnHeadings instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ExportHeadings { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام خاصية HtmlSaveOptions.ExportRowColumnHeadings. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportHeadingsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // إنشاء خيارات حفظ HTML وتمكين تصدير العناوين
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportHeadings = true;

            // حفظ كـ HTML مع العناوين
            workbook.Save("output_with_headings.html", options);
            
            // حفظ مرة أخرى بدون عناوين للمقارنة
            options.ExportHeadings = false;
            workbook.Save("output_without_headings.html", options);
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


