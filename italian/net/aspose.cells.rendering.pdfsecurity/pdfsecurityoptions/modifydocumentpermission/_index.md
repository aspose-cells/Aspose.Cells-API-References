---
title: "PdfSecurityOptions.ModifyDocumentPermission"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PdfSecurityOptions proprietà. Indica se consentire di modificare il contenuto del documento mediante operazioni diverse da quelle controllate da AnnotationsPermission, FillFormsPermission e AssembleDocumentPermission."
type: docs
url: /it/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/modifydocumentpermission/
---
## PdfSecurityOptions.ModifyDocumentPermission property

Indica se consentire di modificare il contenuto del documento mediante operazioni diverse da quelle controllate da [`AnnotationsPermission`](../annotationspermission/), [`FillFormsPermission`](../fillformspermission/) e [`AssembleDocumentPermission`](../assembledocumentpermission/).

```csharp
public bool ModifyDocumentPermission { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyModifyDocumentPermissionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF Security";

            // Configura le opzioni di salvataggio PDF con le impostazioni di sicurezza
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            // Imposta password e autorizzazioni
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.ModifyDocumentPermission = false; // Core property demonstration
            securityOptions.PrintPermission = true;

            // Applica le opzioni di sicurezza e salva
            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecuredDocument.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with ModifyDocumentPermission set to false");
        }
    }
}
```

### Vedi anche

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


