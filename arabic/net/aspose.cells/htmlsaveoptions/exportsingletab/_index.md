---
title: "HtmlSaveOptions.ExportSingleTab"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان يتم تصدير علامة التبويب الوحيدة عندما يحتوي الملف على ورقة عمل واحدة فقط. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/exportsingletab/
---
## HtmlSaveOptions.ExportSingleTab property

تشير إلى ما إذا كان يتم تصدير علامة التبويب الوحيدة عندما يحتوي الملف على ورقة عمل واحدة فقط. القيمة الافتراضية هي false.

```csharp
public bool ExportSingleTab { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportSingleTabDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد ببيانات اختبار
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // إنشاء خيارات حفظ HTML مع تعيين ExportSingleTab إلى true
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportSingleTab = true,
                ExportImagesAsBase64 = true
            };

            // حفظ المصنف كملف HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "SingleTabExport.html");
            workbook.Save(outputPath, options);

            Console.WriteLine("HTML file with single tab export created successfully: " + outputPath);
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


