---
title: "PdfSecurityOptions.FullQualityPrintPermission"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PdfSecurityOptions proprietà. Indica se consentire di stampare il documento in una rappresentazione da cui potrebbe essere generata una copia digitale fedele del contenuto PDF."
type: docs
url: /it/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fullqualityprintpermission/
---
## PdfSecurityOptions.FullQualityPrintPermission property

Indica se consentire la stampa del documento in una rappresentazione da cui possa essere generata una fedele copia digitale del contenuto PDF.

```csharp
public bool FullQualityPrintPermission { get; set; }
```

### Osservazioni

Quando è chiaro (e [`PrintPermission`](../printpermission/) è impostato), la stampa è limitata a una rappresentazione di basso livello dell'aspetto, possibilmente di qualità degradata.

### Esempi

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

### Vedi anche

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


