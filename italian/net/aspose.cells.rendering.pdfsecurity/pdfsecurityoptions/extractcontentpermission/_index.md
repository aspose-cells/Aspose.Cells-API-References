---
title: "PdfSecurityOptions.ExtractContentPermission"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PdfSecurityOptions. Indica se consentire di copiare o estrarre in altro modo testo e grafica dal documento mediante operazioni diverse da quelle controllate da AccessibilityExtractContent"
type: docs
url: /it/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermission/
---
## PdfSecurityOptions.ExtractContentPermission property

Indica se consentire di copiare o estrarre in altro modo testo e grafica dal documento mediante operazioni diverse da quelle controllate da [`AccessibilityExtractContent`](../accessibilityextractcontent/).

```csharp
public bool ExtractContentPermission { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyExtractContentPermissionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Sample PDF Content";

            // Configura le opzioni di salvataggio PDF con le impostazioni di sicurezza
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            // Imposta password e autorizzazioni
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            
            // Dimostra l'uso di ExtractContentPermission
            securityOptions.ExtractContentPermission = false;
            securityOptions.PrintPermission = true;
            securityOptions.ModifyDocumentPermission = false;

            // Applica le opzioni di sicurezza e salva
            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecuredPDF.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with ExtractContentPermission set to false");
        }
    }
}
```

### Vedi anche

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


