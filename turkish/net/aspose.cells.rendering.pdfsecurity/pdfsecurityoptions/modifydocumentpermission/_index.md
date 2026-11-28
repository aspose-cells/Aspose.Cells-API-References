---
title: "PdfSecurityOptions.ModifyDocumentPermission"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSecurityOptions özelliği. AnnotationsPermission, FillFormsPermission ve AssembleDocumentPermission tarafından kontrol edilen işlemler dışındaki işlemlerle belgenin içeriğinin değiştirilmesine izin verilip verilmediğini gösterir."
type: docs
url: /tr/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/modifydocumentpermission/
---
## PdfSecurityOptions.ModifyDocumentPermission property

Belgenin içeriğinin, [`AnnotationsPermission`](../annotationspermission/), [`FillFormsPermission`](../fillformspermission/) ve [`AssembleDocumentPermission`](../assembledocumentpermission/) tarafından kontrol edilen işlemler dışındaki işlemlerle değiştirilmesine izin verilip verilmediğini gösterir.

```csharp
public bool ModifyDocumentPermission { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyModifyDocumentPermissionDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF Security";

            // PDF kaydetme seçeneklerini güvenlik ayarlarıyla yapılandırın
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            // Şifreleri ve izinleri ayarlayın
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.ModifyDocumentPermission = false; // Core property demonstration
            securityOptions.PrintPermission = true;

            // Güvenlik seçeneklerini uygulayın ve kaydedin
            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecuredDocument.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with ModifyDocumentPermission set to false");
        }
    }
}
```

### Ayrıca Bakınız

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


