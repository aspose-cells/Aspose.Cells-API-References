---
title: "PdfSecurityOptions.UserPassword"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfSecurityOptions. تحصل على أو تعيين كلمة مرور المستخدم المطلوبة لفتح مستند PDF المشفر"
type: docs
url: /ar/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/userpassword/
---
## PdfSecurityOptions.UserPassword property

يحصل أو يعيّن كلمة مرور المستخدم المطلوبة لفتح المستند PDF المشفر.

```csharp
public string UserPassword { get; set; }
```

### ملاحظات

ستكون كلمة مرور المالك أو كلمة مرور المستخدم مطلوبة لفتح مستند PDF مشفر للعرض.

يمكن أن تكون كلمة مرور المستخدم فارغة أو null، وفي هذه الحالة لن يُطلب أي كلمة مرور من المستخدم عند فتح مستند PDF.

فتح المستند باستخدام كلمة مرور المالك الصحيحة يسمح بالوصول الكامل إلى المستند.

فتح المستند باستخدام كلمة مرور المستخدم الصحيحة (أو فتح مستند لا يحتوي على كلمة مرور مستخدم) يسمح بالوصول المحدود وفقًا للأذونات المحددة.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyUserPasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Protected PDF with User Password";

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();
            
            securityOptions.UserPassword = "user123";
            securityOptions.OwnerPassword = "owner456";
            securityOptions.PrintPermission = true;
            
            saveOptions.SecurityOptions = securityOptions;
            workbook.Save("ProtectedWithUserPassword.pdf", saveOptions);
            
            Console.WriteLine("PDF created with user password protection.");
        }
    }
}
```

### انظر أيضًا

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


