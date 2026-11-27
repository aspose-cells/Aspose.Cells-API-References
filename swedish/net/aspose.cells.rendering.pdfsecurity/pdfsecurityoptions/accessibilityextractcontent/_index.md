---
title: "PdfSecurityOptions.AccessibilityExtractContent"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSecurityOptions egenskap. Anger om extrahering av text och grafik för att stödja tillgänglighet för användare med funktionsnedsättningar eller för andra ändamål ska tillåtas."
type: docs
url: /sv/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/accessibilityextractcontent/
---
## PdfSecurityOptions.AccessibilityExtractContent property

Anger om det ska tillåtas att extrahera text och grafik (för att stödja tillgänglighet för användare med funktionsnedsättningar eller för andra ändamål).

```csharp
public bool AccessibilityExtractContent { get; set; }
```

### Exempel

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

### Se även

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


