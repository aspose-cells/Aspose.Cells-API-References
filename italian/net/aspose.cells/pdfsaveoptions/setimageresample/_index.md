---
title: "PdfSaveOptions.SetImageResample"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PdfSaveOptions. Imposta i PPIpixels per inch desiderati delle immagini ricampionate e la qualità jpeg. Tutte le immagini saranno convertite in JPEG con l'impostazione di qualità specificata e le immagini che superano i PPIpixels per inch specificati saranno ricampionate"
type: docs
url: /it/net/aspose.cells/pdfsaveoptions/setimageresample/
---
## PdfSaveOptions.SetImageResample method

Imposta il PPI desiderato (pixel per pollice) per il ridimensionamento delle immagini e la qualità JPEG. Tutte le immagini saranno convertite in JPEG con l'impostazione di qualità specificata, e le immagini che superano il PPI specificato (pixel per pollice) saranno ridimensionate.

```csharp
public void SetImageResample(int desiredPPI, int jpegQuality)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| desiredPPI | Int32 | Pixel per pollice desiderati. 220 alta qualità. 150 qualità schermo. 96 qualità email. |
| jpegQuality | Int32 | 0 - 100% qualità JPEG. |

### Esempi

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

### Vedi anche

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


