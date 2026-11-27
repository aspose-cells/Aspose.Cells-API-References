---
title: "PdfSecurityOptions.OwnerPassword"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSecurityOptions egenskap. Hämtar eller anger ägarlösenordet för det krypterade PDF-dokumentet"
type: docs
url: /sv/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/ownerpassword/
---
## PdfSecurityOptions.OwnerPassword property

Hämtar eller anger ägarlösenordet för det krypterade PDF-dokumentet.

```csharp
public string OwnerPassword { get; set; }
```

### Anmärkningar

Ägarlösenordet tillåter användaren att öppna ett krypterat PDF-dokument utan några åtkomstrestriktioner angivna.

### Exempel

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

### Se även

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


