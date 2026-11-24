---
title: "PdfSecurityOptions.PrintPermission"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSecurityOptions-Eigenschaft. Gibt an, ob das Drucken des Dokuments erlaubt ist."
type: docs
url: /de/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/printpermission/
---
## PdfSecurityOptions.PrintPermission property

Gibt an, ob das Drucken des Dokuments erlaubt ist.

```csharp
public bool PrintPermission { get; set; }
```

### Hinweise

Möglicherweise nicht in höchster Qualität, abhängig davon, ob [`FullQualityPrintPermission`](../fullqualityprintpermission/) ebenfalls gesetzt ist.

### Beispiele

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

### Siehe auch

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


