---
title: "PdfSecurityOptions.AccessibilityExtractContent"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PdfSecurityOptions proprietà. Indica se consentire l'estrazione di testo e grafica a supporto dell'accessibilità per utenti con disabilità o per altri scopi."
type: docs
url: /it/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/accessibilityextractcontent/
---
## PdfSecurityOptions.AccessibilityExtractContent property

Indica se consentire l'estrazione di testo e grafica (a supporto dell'accessibilità per utenti con disabilità o per altri scopi).

```csharp
public bool AccessibilityExtractContent { get; set; }
```

### Esempi

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

### Vedi anche

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


