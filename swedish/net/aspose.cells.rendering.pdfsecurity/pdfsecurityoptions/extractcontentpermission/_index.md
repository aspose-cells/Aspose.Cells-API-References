---
title: "PdfSecurityOptions.ExtractContentPermission"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSecurityOptions-egenskap. Anger om det ska tillåtas att kopiera eller på annat sätt extrahera text och grafik från dokumentet genom operationer som inte styrs av AccessibilityExtractContent"
type: docs
url: /sv/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermission/
---
## PdfSecurityOptions.ExtractContentPermission property

Anger om det ska tillåtas att kopiera eller på annat sätt extrahera text och grafik från dokumentet genom operationer som inte styrs av [`AccessibilityExtractContent`](../accessibilityextractcontent/).

```csharp
public bool ExtractContentPermission { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyExtractContentPermissionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Sample PDF Content";

            // Konfigurera PDF-sparalternativ med säkerhetsinställningar
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            // Ställ in lösenord och behörigheter
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            
            // Demonstrera användning av ExtractContentPermission
            securityOptions.ExtractContentPermission = false;
            securityOptions.PrintPermission = true;
            securityOptions.ModifyDocumentPermission = false;

            // Tillämpa säkerhetsalternativ och spara
            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecuredPDF.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with ExtractContentPermission set to false");
        }
    }
}
```

### Se även

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


