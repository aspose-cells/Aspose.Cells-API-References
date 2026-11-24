---
title: "PdfSecurityOptions.ExtractContentPermission"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSecurityOptions-Eigenschaft. Gibt an, ob das Kopieren oder anderweitige Extrahieren von Text und Grafiken aus dem Dokument durch andere Vorgänge als die von AccessibilityExtractContent gesteuerten erlaubt ist."
type: docs
url: /de/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermission/
---
## PdfSecurityOptions.ExtractContentPermission property

Gibt an, ob das Kopieren oder anderweitige Extrahieren von Text und Grafiken aus dem Dokument durch andere Vorgänge als die von [`AccessibilityExtractContent`](../accessibilityextractcontent/) gesteuerten erlaubt ist.

```csharp
public bool ExtractContentPermission { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Sample PDF Content";

            // PDF-Speicheroptionen mit Sicherheitseinstellungen konfigurieren
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            // Passwörter und Berechtigungen festlegen
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            
            // Demonstration der Verwendung von ExtractContentPermission
            securityOptions.ExtractContentPermission = false;
            securityOptions.PrintPermission = true;
            securityOptions.ModifyDocumentPermission = false;

            // Sicherheitsoptionen anwenden und speichern
            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecuredPDF.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with ExtractContentPermission set to false");
        }
    }
}
```

### Siehe auch

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


