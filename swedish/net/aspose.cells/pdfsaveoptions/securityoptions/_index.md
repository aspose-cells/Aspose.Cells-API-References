---
title: "PdfSaveOptions.SecurityOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSaveOptions-egenskap. Ställ in dessa alternativ när säkerhet behövs i xls2pdf‑resultatet"
type: docs
url: /sv/net/aspose.cells/pdfsaveoptions/securityoptions/
---
## PdfSaveOptions.SecurityOptions property

Ställ in dessa alternativ när säkerhet behövs i xls2pdf‑resultatet.

```csharp
public PdfSecurityOptions SecurityOptions { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertySecurityOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till exempeldata
            workbook.Worksheets[0].Cells["A1"].Value = "Protected PDF Demo";
            
            // Skapa PDF-sparalternativ
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Konfigurera säkerhetsalternativ
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.PrintPermission = true;
            securityOptions.ModifyDocumentPermission = false;
            securityOptions.ExtractContentPermission = false;
            
            // Tilldela säkerhetsalternativ till sparalternativ
            saveOptions.SecurityOptions = securityOptions;
            
            // Spara PDF‑filen med säkerhetsinställningar
            workbook.Save("SecuredDocument.pdf", saveOptions);
            
            Console.WriteLine("PDF with security options created successfully.");
        }
    }
}
```

### Se även

* class [PdfSecurityOptions](../../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


