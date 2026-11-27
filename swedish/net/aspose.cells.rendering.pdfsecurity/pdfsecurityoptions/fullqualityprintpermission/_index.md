---
title: "PdfSecurityOptions.FullQualityPrintPermission"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSecurityOptions egenskap. Anger om utskrift av dokumentet till en representation från vilken en trogen digital kopia av PDF-innehållet kan genereras."
type: docs
url: /sv/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fullqualityprintpermission/
---
## PdfSecurityOptions.FullQualityPrintPermission property

Indikerar om det ska tillåtas att skriva ut dokumentet till en representation från vilken en trogen digital kopia av PDF-innehållet kan genereras.

```csharp
public bool FullQualityPrintPermission { get; set; }
```

### Anmärkningar

När den är markerad (och [`PrintPermission`](../printpermission/) är satt), begränsas utskrift till en låg nivå-representation av utseendet, möjligen med försämrad kvalitet.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyFullQualityPrintPermissionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test Full Quality Print Permission";

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.FullQualityPrintPermission = true;
            securityOptions.PrintPermission = true;

            saveOptions.SecurityOptions = securityOptions;
            workbook.Save("FullQualityPrintDemo.pdf", saveOptions);

            Console.WriteLine("PDF created with FullQualityPrintPermission enabled.");
        }
    }
}
```

### Se även

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


