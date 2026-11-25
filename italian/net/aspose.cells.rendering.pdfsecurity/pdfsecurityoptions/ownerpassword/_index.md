---
title: "PdfSecurityOptions.OwnerPassword"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PdfSecurityOptions. Ottiene o imposta la password del proprietario per il documento PDF crittografato"
type: docs
url: /it/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/ownerpassword/
---
## PdfSecurityOptions.OwnerPassword property

Ottiene o imposta la password del proprietario per il documento PDF crittografato.

```csharp
public string OwnerPassword { get; set; }
```

### Osservazioni

La password del proprietario consente all'utente di aprire un documento PDF crittografato senza alcuna restrizione di accesso specificata.

### Esempi

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

### Vedi anche

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


