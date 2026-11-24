---
title: "Enum PdfOptimizationType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.PdfOptimizationType enum. Gibt einen Optimierungstyp an"
type: docs
url: /de/net/aspose.cells.rendering/pdfoptimizationtype/
---
## PdfOptimizationType enumeration

Gibt einen Optimierungstyp an.

```csharp
public enum PdfOptimizationType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Standard | `0` | Hohe Druckqualität |
| MinimumSize | `1` | Dateigröße ist wichtiger als Druckqualität |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfOptimizationTypeDemo
    {
        public static void PdfOptimizationTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // Erstellen Sie PdfSaveOptions und setzen Sie den Optimierungstyp
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;

            // Speichern Sie die Arbeitsmappe als PDF mit dem angegebenen Optimierungstyp
            workbook.Save("OptimizedOutput.pdf", pdfSaveOptions);

            Console.WriteLine("PDF saved with optimization type: MinimumSize");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


