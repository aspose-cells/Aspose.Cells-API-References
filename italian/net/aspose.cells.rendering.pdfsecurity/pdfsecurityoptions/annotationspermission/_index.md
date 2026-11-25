---
title: "PdfSecurityOptions.AnnotationsPermission"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PdfSecurityOptions proprietà. Indica se consentire di aggiungere o modificare annotazioni di testo e compilare campi di modulo interattivi."
type: docs
url: /it/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/annotationspermission/
---
## PdfSecurityOptions.AnnotationsPermission property

Indica se consentire l'aggiunta o la modifica di annotazioni di testo, la compilazione di campi di modulo interattivi.

```csharp
public bool AnnotationsPermission { get; set; }
```

### Osservazioni

se [`ModifyDocumentPermission`](../modifydocumentpermission/) è anche impostato, creare o modificare campi di modulo interattivi (inclusi i campi firma).

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyAnnotationsPermissionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF with Annotations Permission";

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.AnnotationsPermission = true;

            saveOptions.SecurityOptions = securityOptions;
            workbook.Save("AnnotationsPermissionDemo.pdf", saveOptions);

            Console.WriteLine("PDF created with annotations permission enabled.");
        }
    }
}
```

### Vedi anche

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


