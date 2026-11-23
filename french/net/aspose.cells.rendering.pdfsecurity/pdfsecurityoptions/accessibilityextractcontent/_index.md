---
title: "PdfSecurityOptions.AccessibilityExtractContent"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PdfSecurityOptions. Indique s'il faut autoriser l'extraction de texte et de graphiques pour soutenir l'accessibilité des utilisateurs en situation de handicap ou à d'autres fins"
type: docs
url: /fr/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/accessibilityextractcontent/
---
## PdfSecurityOptions.AccessibilityExtractContent property

Indique s'il faut autoriser l'extraction de texte et de graphiques (pour soutenir l'accessibilité des utilisateurs handicapés ou à d'autres fins).

```csharp
public bool AccessibilityExtractContent { get; set; }
```

### Exemples

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

### Voir aussi

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


