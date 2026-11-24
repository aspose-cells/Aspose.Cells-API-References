---
title: "PdfSecurityOptions.AccessibilityExtractContent"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSecurityOptions-Eigenschaft. Gibt an, ob das Extrahieren von Text und Grafiken zur Unterstützung der Barrierefreiheit für Benutzer mit Behinderungen oder für andere Zwecke erlaubt ist."
type: docs
url: /de/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/accessibilityextractcontent/
---
## PdfSecurityOptions.AccessibilityExtractContent property

Gibt an, ob das Extrahieren von Text und Grafiken erlaubt ist (zur Unterstützung der Barrierefreiheit für Benutzer mit Behinderungen oder zu anderen Zwecken).

```csharp
public bool AccessibilityExtractContent { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyAccessibilityExtractContentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test Accessibility Extract Content";

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            pdfSecurityOptions.OwnerPassword = "owner123";
            pdfSecurityOptions.UserPassword = "user123";
            pdfSecurityOptions.AccessibilityExtractContent = true;
            pdfSecurityOptions.ExtractContentPermission = false;

            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;
            workbook.Save("AccessibilityExtractContentDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Siehe auch

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


