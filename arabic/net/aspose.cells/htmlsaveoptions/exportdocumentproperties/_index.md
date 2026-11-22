---
title: "HtmlSaveOptions.ExportDocumentProperties"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان يتم تصدير خصائص المستند. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel يرجى الحفاظ على القيمة الافتراضية"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/exportdocumentproperties/
---
## HtmlSaveOptions.ExportDocumentProperties property

تشير إلى ما إذا كان يتم تصدير خصائص المستند. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية.

```csharp
public bool ExportDocumentProperties { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportDocumentPropertiesDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض خصائص المستند
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Document";
            
            // أضف بيانات خلايا تجريبية
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // أنشئ خيارات حفظ HTML واضبط ExportDocumentProperties على false
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportDocumentProperties = false;
            
            // حفظ المصنف كملف HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with document properties export disabled.");
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


