---
title: "PdfSecurityOptions.FillFormsPermission"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PdfSecurityOptions. Indica se consentire di compilare i campi di modulo interattivi esistenti, inclusi i campi firma, anche se ModifyDocumentPermission è disattivata"
type: docs
url: /it/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fillformspermission/
---
## PdfSecurityOptions.FillFormsPermission property

Indica se consentire di compilare i campi di modulo interattivi esistenti (inclusi i campi firma), anche se [`ModifyDocumentPermission`](../modifydocumentpermission/) è disattivata.

```csharp
public bool FillFormsPermission { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyFillFormsPermissionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "PDF Form Example";

            // Configura le opzioni di salvataggio PDF con le impostazioni di sicurezza
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            // Imposta password e autorizzazioni
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.FillFormsPermission = true; // Key permission being demonstrated
            securityOptions.PrintPermission = true;

            // Applica le opzioni di sicurezza e salva
            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecureFormFillEnabled.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with form filling permission enabled.");
        }
    }
}
```

### Vedi anche

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


