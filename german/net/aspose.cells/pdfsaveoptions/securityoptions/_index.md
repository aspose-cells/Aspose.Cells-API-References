---
title: "PdfSaveOptions.SecurityOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSaveOptions-Eigenschaft. Setze diese Optionen, wenn im xls2pdf-Ergebnis Sicherheit erforderlich ist."
type: docs
url: /de/net/aspose.cells/pdfsaveoptions/securityoptions/
---
## PdfSaveOptions.SecurityOptions property

Setzen Sie diese Optionen, wenn im xls2pdf‑Ergebnis Sicherheit benötigt wird.

```csharp
public PdfSecurityOptions SecurityOptions { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertySecurityOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügen Sie Beispieldaten hinzu
            workbook.Worksheets[0].Cells["A1"].Value = "Protected PDF Demo";
            
            // PDF-Speicheroptionen erstellen
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Sicherheitsoptionen konfigurieren.
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.PrintPermission = true;
            securityOptions.ModifyDocumentPermission = false;
            securityOptions.ExtractContentPermission = false;
            
            // Weise die Sicherheitsoptionen den Speicheroptionen zu.
            saveOptions.SecurityOptions = securityOptions;
            
            // Speichere das PDF mit Sicherheitseinstellungen.
            workbook.Save("SecuredDocument.pdf", saveOptions);
            
            Console.WriteLine("PDF with security options created successfully.");
        }
    }
}
```

### Siehe auch

* class [PdfSecurityOptions](../../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


