---
title: "PdfSecurityOptions.AnnotationsPermission"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSecurityOptions özelliği. Metin açıklamaları eklemeye veya değiştirmeye ve etkileşimli form alanlarını doldurmaya izin verilip verilmediğini gösterir."
type: docs
url: /tr/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/annotationspermission/
---
## PdfSecurityOptions.AnnotationsPermission property

Metin açıklamaları eklenmesine veya değiştirilmesine, etkileşimli form alanlarının doldurulmasına izin verilip verilmediğini gösterir.

```csharp
public bool AnnotationsPermission { get; set; }
```

### Açıklamalar

Eğer [`ModifyDocumentPermission`](../modifydocumentpermission/) da ayarlanmışsa, etkileşimli form alanlarını (imza alanları dahil) oluşturabilir veya değiştirebilirsiniz.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyAnnotationsPermissionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF with Annotations Permission";

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.AnnotationsPermission = true;

            saveOptions.SecurityOptions = securityOptions;
            workbook.Save("AnnotationsPermissionDemo.pdf", saveOptions);

            Console.WriteLine("PDF created with annotations permission enabled.");
        }
    }
}
```

### Ayrıca Bakınız

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


