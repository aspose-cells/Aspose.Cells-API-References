---
title: "PdfSaveOptions.SetImageResample"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSaveOptions-metoden. Anger önskad PPI-pixlar per tum för omprovtagning av bilder och jpeg-kvalitet. Alla bilder kommer att konverteras till JPEG med den angivna kvalitetsinställningen och bilder som är större än den angivna PPI-pixlar per tum kommer att omprovtagas."
type: docs
url: /sv/net/aspose.cells/pdfsaveoptions/setimageresample/
---
## PdfSaveOptions.SetImageResample method

Anger önskad PPI (pixlar per tum) för omprovningsbilder och JPEG-kvalitet. Alla bilder kommer att konverteras till JPEG med den angivna kvalitetsinställningen, och bilder som är större än den angivna PPI (pixlar per tum) kommer att omprovas.

```csharp
public void SetImageResample(int desiredPPI, int jpegQuality)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| desiredPPI | Int32 | Önskade pixlar per tum. 220 hög kvalitet. 150 skärmkvalitet. 96 e-postkvalitet. |
| jpegQuality | Int32 | 0 - 100 % JPEG-kvalitet. |

### Exempel

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

### Se även

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


