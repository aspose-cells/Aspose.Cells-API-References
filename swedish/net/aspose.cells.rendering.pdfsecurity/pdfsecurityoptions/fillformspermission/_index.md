---
title: "PdfSecurityOptions.FillFormsPermission"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSecurityOptions-egenskap. Anger om det ska tillåtas att fylla i befintliga interaktiva formulärfält inklusive signaturfält även om ModifyDocumentPermission är avaktiverad"
type: docs
url: /sv/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fillformspermission/
---
## PdfSecurityOptions.FillFormsPermission property

Anger om det ska tillåtas att fylla i befintliga interaktiva formulärfält (inklusive signaturfält), även om [`ModifyDocumentPermission`](../modifydocumentpermission/) är avaktiverad.

```csharp
public bool FillFormsPermission { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "PDF Form Example";

            // Konfigurera PDF-sparalternativ med säkerhetsinställningar
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            // Ställ in lösenord och behörigheter
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.FillFormsPermission = true; // Key permission being demonstrated
            securityOptions.PrintPermission = true;

            // Tillämpa säkerhetsalternativ och spara
            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecureFormFillEnabled.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with form filling permission enabled.");
        }
    }
}
```

### Se även

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


