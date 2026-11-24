---
title: "PdfSecurityOptions.AnnotationsPermission"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSecurityOptions-Eigenschaft. Gibt an, ob das Hinzufügen oder Ändern von Textanmerkungen und das Ausfüllen interaktiver Formularfelder erlaubt ist."
type: docs
url: /de/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/annotationspermission/
---
## PdfSecurityOptions.AnnotationsPermission property

Gibt an, ob das Hinzufügen oder Ändern von Textanmerkungen sowie das Ausfüllen interaktiver Formularfelder erlaubt ist.

```csharp
public bool AnnotationsPermission { get; set; }
```

### Hinweise

Wenn [`ModifyDocumentPermission`](../modifydocumentpermission/) ebenfalls gesetzt ist, können interaktive Formularfelder (einschließlich Signaturfelder) erstellt oder geändert werden.

### Beispiele

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

### Siehe auch

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


