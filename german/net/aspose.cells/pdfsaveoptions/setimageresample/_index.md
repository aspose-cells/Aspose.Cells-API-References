---
title: "PdfSaveOptions.SetImageResample"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSaveOptions Methode. Legt die gewünschte PPI (Pixel pro Zoll) für das Resampling von Bildern und die JPEG-Qualität fest. Alle Bilder werden mit der angegebenen Qualitätseinstellung in JPEG konvertiert und Bilder, die größer als die angegebene PPI (Pixel pro Zoll) sind, werden neu gesampelt"
type: docs
url: /de/net/aspose.cells/pdfsaveoptions/setimageresample/
---
## PdfSaveOptions.SetImageResample method

Setzt die gewünschte PPI (Pixel pro Zoll) für das Resampling von Bildern und die JPEG‑Qualität. Alle Bilder werden mit der angegebenen Qualitätseinstellung in JPEG konvertiert, und Bilder, die größer als die angegebene PPI (Pixel pro Zoll) sind, werden neu gesampelt.

```csharp
public void SetImageResample(int desiredPPI, int jpegQuality)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| desiredPPI | Int32 | Gewünschte Pixel pro Zoll. 220 hohe Qualität. 150 Bildschirmqualität. 96 E-Mail-Qualität. |
| jpegQuality | Int32 | 0 - 100 % JPEG‑Qualität. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsMethodSetImageResampleWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook("Book1.xlsx");
            
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.SetImageResample(96, 80);
            
            wb.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Siehe auch

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


