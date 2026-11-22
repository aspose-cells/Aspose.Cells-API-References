---
title: "PdfSaveOptions.SecurityOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfSaveOptions. عيّن هذه الخيارات عندما تكون الأمان مطلوبًا في نتيجة xls2pdf"
type: docs
url: /ar/net/aspose.cells/pdfsaveoptions/securityoptions/
---
## PdfSaveOptions.SecurityOptions property

قم بتعيين هذه الخيارات عندما تكون الأمان مطلوبًا في نتيجة xls2pdf.

```csharp
public PdfSecurityOptions SecurityOptions { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertySecurityOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف بيانات تجريبية
            workbook.Worksheets[0].Cells["A1"].Value = "Protected PDF Demo";
            
            // أنشئ خيارات حفظ PDF
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // تكوين خيارات الأمان
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.PrintPermission = true;
            securityOptions.ModifyDocumentPermission = false;
            securityOptions.ExtractContentPermission = false;
            
            // عيّن خيارات الأمان إلى خيارات الحفظ
            saveOptions.SecurityOptions = securityOptions;
            
            // احفظ ملف PDF مع إعدادات الأمان
            workbook.Save("SecuredDocument.pdf", saveOptions);
            
            Console.WriteLine("PDF with security options created successfully.");
        }
    }
}
```

### انظر أيضًا

* class [PdfSecurityOptions](../../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


