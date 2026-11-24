---
title: "PdfSecurityOptions.AssembleDocumentPermission"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSecurityOptions-Eigenschaft. Gibt an, ob das Zusammenstellen des Dokuments (Einfügen, Drehen oder Löschen von Seiten sowie Erstellen von Lesezeichen oder Miniaturbildern) erlaubt ist, selbst wenn ModifyDocumentPermission nicht gesetzt ist."
type: docs
url: /de/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/assembledocumentpermission/
---
## PdfSecurityOptions.AssembleDocumentPermission property

Gibt an, ob das Zusammenstellen des Dokuments (Einfügen, Drehen oder Löschen von Seiten sowie Erstellen von Lesezeichen oder Miniaturbildern) erlaubt ist, selbst wenn [`ModifyDocumentPermission`](../modifydocumentpermission/) nicht gesetzt ist.

```csharp
public bool AssembleDocumentPermission { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyAssembleDocumentPermissionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF Security";

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            pdfSecurityOptions.OwnerPassword = "owner123";
            pdfSecurityOptions.UserPassword = "user123";
            pdfSecurityOptions.AssembleDocumentPermission = false;
            pdfSecurityOptions.PrintPermission = true;

            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;
            workbook.Save("secured_document.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with assemble document permission disabled.");
        }
    }
}
```

### Siehe auch

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


