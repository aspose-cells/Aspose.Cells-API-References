---
title: "PdfSaveOptions.SetImageResample"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PdfSaveOptions. Définit le PPIpixels souhaité par pouce pour les images rééchantillonnées et la qualité jpeg. Toutes les images seront converties en JPEG avec le paramètre de qualité spécifié et les images dont la résolution dépasse le PPI pixels par pouce spécifié seront rééchantillonnées"
type: docs
url: /fr/net/aspose.cells/pdfsaveoptions/setimageresample/
---
## PdfSaveOptions.SetImageResample method

Définit le PPI (pixels par pouce) souhaité pour le rééchantillonnage des images et la qualité JPEG. Toutes les images seront converties en JPEG avec le paramètre de qualité spécifié, et les images dont le PPI dépasse le PPI spécifié (pixels par pouce) seront rééchantillonnées.

```csharp
public void SetImageResample(int desiredPPI, int jpegQuality)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| desiredPPI | Int32 | Pixels par pouce souhaités. 220 haute qualité. 150 qualité d'écran. 96 qualité email. |
| jpegQuality | Int32 | 0 - 100 % qualité JPEG. |

### Exemples

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

### Voir aussi

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


