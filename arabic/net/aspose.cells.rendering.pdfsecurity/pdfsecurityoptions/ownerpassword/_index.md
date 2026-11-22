---
title: "PdfSecurityOptions.OwnerPassword"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfSecurityOptions. تحصل أو تعين كلمة مرور المالك لمستند PDF المشفر"
type: docs
url: /ar/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/ownerpassword/
---
## PdfSecurityOptions.OwnerPassword property

يحصل أو يعيّن كلمة مرور المالك للمستند PDF المشفر.

```csharp
public string OwnerPassword { get; set; }
```

### ملاحظات

كلمة مرور المالك تسمح للمستخدم بفتح مستند PDF مشفر دون أي قيود وصول محددة.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyOwnerPasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Protected PDF with Owner Password";

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.PrintPermission = true;
            securityOptions.ModifyDocumentPermission = false;

            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecuredPdfWithOwnerPassword.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with owner password protection.");
        }
    }
}
```

### انظر أيضًا

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


