---
title: "PdfSecurityOptions.FillFormsPermission"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfSecurityOptions. تشير إلى ما إذا كان يُسمح بملء حقول النماذج التفاعلية الموجودة بما في ذلك حقول التوقيع حتى إذا كان ModifyDocumentPermission غير مفعّل"
type: docs
url: /ar/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fillformspermission/
---
## PdfSecurityOptions.FillFormsPermission property

تشير إلى ما إذا كان يُسمح بملء حقول النماذج التفاعلية الموجودة (بما في ذلك حقول التوقيع)، حتى إذا كان [`ModifyDocumentPermission`](../modifydocumentpermission/) غير مفعّل.

```csharp
public bool FillFormsPermission { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyFillFormsPermissionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "PDF Form Example";

            // تكوين خيارات حفظ PDF مع إعدادات الأمان
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            // تعيين كلمات المرور والأذونات
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.FillFormsPermission = true; // Key permission being demonstrated
            securityOptions.PrintPermission = true;

            // تطبيق خيارات الأمان وحفظها
            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecureFormFillEnabled.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with form filling permission enabled.");
        }
    }
}
```

### انظر أيضًا

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


