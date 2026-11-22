---
title: "PdfSecurityOptions.ExtractContentPermissionObsolete"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfSecurityOptions. الإذن بنسخ أو استخراج المحتوى تم إهماله وفقًا لمرجع PDF"
type: docs
url: /ar/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermissionobsolete/
---
## PdfSecurityOptions.ExtractContentPermissionObsolete property

الإذن بنسخ أو استخراج المحتوى تم إهماله وفقًا لمرجع PDF.

```csharp
[Obsolete("Use ExtractContentPermission property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ExtractContentPermissionObsolete { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية ExtractContentPermission. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ سبتمبر 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyExtractContentPermissionObsoleteDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF Security";

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            pdfSecurityOptions.OwnerPassword = "owner123";
            pdfSecurityOptions.UserPassword = "user123";
            pdfSecurityOptions.ExtractContentPermissionObsolete = false;
            pdfSecurityOptions.ExtractContentPermission = true;

            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;
            workbook.Save("SecurePDF.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with ExtractContentPermissionObsolete set to false");
        }
    }
}
```

### انظر أيضًا

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


