---
title: "PdfSecurityOptions.PrintPermission"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PdfSecurityOptions. Indica se consentire di stampare il documento"
type: docs
url: /it/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/printpermission/
---
## PdfSecurityOptions.PrintPermission property

Indica se consentire la stampa del documento.

```csharp
public bool PrintPermission { get; set; }
```

### Osservazioni

Possibilmente non al livello di qualità più alto, a seconda se [`FullQualityPrintPermission`](../fullqualityprintpermission/) è anche impostata.

### Esempi

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

### Vedi anche

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


