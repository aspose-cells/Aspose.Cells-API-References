---
title: "PdfSecurityOptions.AccessibilityExtractContent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSecurityOptions. Indica si se permite extraer texto y gráficos en apoyo a la accesibilidad para usuarios con discapacidades o para otros propósitos."
type: docs
url: /es/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/accessibilityextractcontent/
---
## PdfSecurityOptions.AccessibilityExtractContent property

Indica si se permite extraer texto y gráficos (en apoyo de la accesibilidad para usuarios con discapacidades o para otros propósitos).

```csharp
public bool AccessibilityExtractContent { get; set; }
```

### Ejemplos

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

### Ver también

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


