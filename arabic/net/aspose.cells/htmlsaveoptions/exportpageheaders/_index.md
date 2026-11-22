---
title: "HtmlSaveOptions.ExportPageHeaders"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان يتم تصدير رؤوس الصفحات"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/exportpageheaders/
---
## HtmlSaveOptions.ExportPageHeaders property

تشير إلى ما إذا كان يتم تصدير رؤوس الصفحات.

```csharp
public bool ExportPageHeaders { get; set; }
```

### ملاحظات

يعمل فقط عندما يكون [`SaveAsSingleFile`](../saveassinglefile/) صحيحًا.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportPageHeadersDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين رأس الصفحة
            worksheet.PageSetup.SetHeader(0, "Sample Header Text");
            
            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("This is a test");
            
            // تكوين خيارات حفظ HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                SaveAsSingleFile = true,
                ShowAllSheets = true,
                ExportPageHeaders = true  // This is the key property being demonstrated
            };
            
            // حفظ المصنف كملف HTML
            string outputPath = "output_with_headers.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file with page headers exported successfully.");
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


