---
title: "HtmlSaveOptions.ExportPageFooters"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان يتم تصدير رؤوس الصفحات"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/exportpagefooters/
---
## HtmlSaveOptions.ExportPageFooters property

تشير إلى ما إذا كان يتم تصدير رؤوس الصفحات.

```csharp
public bool ExportPageFooters { get; set; }
```

### ملاحظات

يعمل فقط عندما يكون [`SaveAsSingleFile`](../saveassinglefile/) صحيحًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportPageFootersDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // إنشاء خيارات حفظ HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // تعيين ExportPageFooters إلى true لتضمين تذييلات الصفحات في الناتج
            saveOptions.ExportPageFooters = true;
            
            // تعيين الخيارات الضرورية الأخرى
            saveOptions.ExportPageHeaders = true;
            
            // حفظ المصنف إلى HTML
            workbook.Save("HtmlWithPageFooters.html", saveOptions);
            
            Console.WriteLine("HTML file with page footers exported successfully.");
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


