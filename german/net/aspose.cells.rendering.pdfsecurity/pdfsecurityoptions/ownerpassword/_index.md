---
title: "PdfSecurityOptions.OwnerPassword"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSecurityOptions-Eigenschaft. Ruft das Besitzerpasswort für das verschlüsselte PDF-Dokument ab oder legt es fest"
type: docs
url: /de/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/ownerpassword/
---
## PdfSecurityOptions.OwnerPassword property

Liest oder setzt das Besitzerpasswort für das verschlüsselte PDF‑Dokument.

```csharp
public string OwnerPassword { get; set; }
```

### Hinweise

Das Besitzerpasswort ermöglicht dem Benutzer, ein verschlüsseltes PDF-Dokument zu öffnen, ohne dass irgendwelche Zugriffsrestriktionen festgelegt sind.

### Beispiele

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

### Siehe auch

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


