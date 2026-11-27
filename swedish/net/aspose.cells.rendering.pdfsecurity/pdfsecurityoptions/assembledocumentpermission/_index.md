---
title: "PdfSecurityOptions.AssembleDocumentPermission"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSecurityOptions egenskap. Anger om det ska tillåtas att sammanställa dokumentet, infoga, rotera eller ta bort sidor samt skapa bokmärken eller miniatyrbilder även om ModifyDocumentPermission inte är satt"
type: docs
url: /sv/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/assembledocumentpermission/
---
## PdfSecurityOptions.AssembleDocumentPermission property

Anger om det ska tillåtas att sammanställa dokumentet (infoga, rotera eller ta bort sidor samt skapa bokmärken eller miniatyrbilder), även om [`ModifyDocumentPermission`](../modifydocumentpermission/) inte är satt.

```csharp
public bool AssembleDocumentPermission { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyAssembleDocumentPermissionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF Security";

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            pdfSecurityOptions.OwnerPassword = "owner123";
            pdfSecurityOptions.UserPassword = "user123";
            pdfSecurityOptions.AssembleDocumentPermission = false;
            pdfSecurityOptions.PrintPermission = true;

            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;
            workbook.Save("secured_document.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with assemble document permission disabled.");
        }
    }
}
```

### Se även

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


