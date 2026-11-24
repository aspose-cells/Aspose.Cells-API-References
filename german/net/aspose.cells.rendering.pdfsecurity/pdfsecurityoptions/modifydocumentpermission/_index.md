---
title: "PdfSecurityOptions.ModifyDocumentPermission"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSecurityOptions-Eigenschaft. Gibt an, ob das Ändern des Inhalts des Dokuments durch andere Vorgänge als die von AnnotationsPermission, FillFormsPermission und AssembleDocumentPermission gesteuerten erlaubt ist."
type: docs
url: /de/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/modifydocumentpermission/
---
## PdfSecurityOptions.ModifyDocumentPermission property

Gibt an, ob das Ändern des Inhalts des Dokuments durch andere Vorgänge als die von [`AnnotationsPermission`](../annotationspermission/), [`FillFormsPermission`](../fillformspermission/) und [`AssembleDocumentPermission`](../assembledocumentpermission/) gesteuerten, erlaubt ist.

```csharp
public bool ModifyDocumentPermission { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF Security";

            // PDF-Speicheroptionen mit Sicherheitseinstellungen konfigurieren
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            // Passwörter und Berechtigungen festlegen
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.ModifyDocumentPermission = false; // Core property demonstration
            securityOptions.PrintPermission = true;

            // Sicherheitsoptionen anwenden und speichern
            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecuredDocument.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with ModifyDocumentPermission set to false");
        }
    }
}
```

### Siehe auch

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


