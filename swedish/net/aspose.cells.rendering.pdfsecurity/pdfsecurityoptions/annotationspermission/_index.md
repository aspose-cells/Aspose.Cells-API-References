---
title: "PdfSecurityOptions.AnnotationsPermission"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSecurityOptions egenskap. Anger om det ska tillåtas att lägga till eller ändra textanteckningar samt fylla i interaktiva formulärfält"
type: docs
url: /sv/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/annotationspermission/
---
## PdfSecurityOptions.AnnotationsPermission property

Anger om det ska tillåtas att lägga till eller ändra textanteckningar, fylla i interaktiva formulärfält.

```csharp
public bool AnnotationsPermission { get; set; }
```

### Anmärkningar

om [`ModifyDocumentPermission`](../modifydocumentpermission/) också är satt, skapa eller ändra interaktiva formulärfält (inklusive signaturfält).

### Exempel

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

### Se även

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


