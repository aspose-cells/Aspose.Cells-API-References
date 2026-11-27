---
title: "PdfSecurityOptions.ModifyDocumentPermission"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSecurityOptions egenskap. Anger om det ska tillåtas att ändra dokumentets innehåll genom operationer som inte styrs av AnnotationsPermission, FillFormsPermission och AssembleDocumentPermission"
type: docs
url: /sv/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/modifydocumentpermission/
---
## PdfSecurityOptions.ModifyDocumentPermission property

Anger om det ska tillåtas att ändra dokumentets innehåll genom operationer som inte styrs av [`AnnotationsPermission`](../annotationspermission/), [`FillFormsPermission`](../fillformspermission/) och [`AssembleDocumentPermission`](../assembledocumentpermission/).

```csharp
public bool ModifyDocumentPermission { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF Security";

            // Konfigurera PDF-sparalternativ med säkerhetsinställningar
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            // Ställ in lösenord och behörigheter
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.ModifyDocumentPermission = false; // Core property demonstration
            securityOptions.PrintPermission = true;

            // Tillämpa säkerhetsalternativ och spara
            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecuredDocument.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with ModifyDocumentPermission set to false");
        }
    }
}
```

### Se även

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


