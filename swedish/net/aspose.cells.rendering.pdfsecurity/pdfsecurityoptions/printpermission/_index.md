---
title: "PdfSecurityOptions.PrintPermission"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSecurityOptions-egenskap. Anger om det ska tillåtas att skriva ut dokumentet"
type: docs
url: /sv/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/printpermission/
---
## PdfSecurityOptions.PrintPermission property

Indikerar om det ska tillåtas att skriva ut dokumentet.

```csharp
public bool PrintPermission { get; set; }
```

### Anmärkningar

Möjligen inte på högsta kvalitet, beroende på om [`FullQualityPrintPermission`](../fullqualityprintpermission/) också är aktiverad.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyPrintPermissionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test Print Permission";

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.PrintPermission = true;

            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("PrintPermissionDemo.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with print permission enabled.");
        }
    }
}
```

### Se även

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


