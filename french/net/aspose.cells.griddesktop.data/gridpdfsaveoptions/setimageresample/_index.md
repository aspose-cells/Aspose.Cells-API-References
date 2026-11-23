---
title: "GridPdfSaveOptions.SetImageResample"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GridPdfSaveOptions. Définit le PPI souhaité (pixels par pouce) des images rééchantillonnées et la qualité JPEG. Toutes les images seront converties en JPEG avec le paramètre de qualité spécifié et les images dont la résolution dépasse le PPI spécifié seront rééchantillonnées."
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridpdfsaveoptions/setimageresample/
---
## GridPdfSaveOptions.SetImageResample method

Définit le PPI (pixels par pouce) souhaité pour le rééchantillonnage des images et la qualité JPEG. Toutes les images seront converties en JPEG avec le paramètre de qualité spécifié, et les images dont le PPI dépasse le PPI spécifié (pixels par pouce) seront rééchantillonnées.

```csharp
public void SetImageResample(int desiredPPI, int jpegQuality)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| desiredPPI | Int32 | Pixels par pouce souhaités. 220 haute qualité. 150 qualité d'écran. 96 qualité email. |
| jpegQuality | Int32 | 0 - 100 % qualité JPEG. |

### Exemples

Le code suivant définit le PPI souhaité à 96 et la qualité JPEG à 80 pour les images dans le PDF de sortie.

```csharp
//chargez le fichier source avec les images.
Workbook wb = new Workbook("Book1.xlsx");

PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

//définissez le PPI souhaité à 96 et la qualité JPEG à 80.
pdfSaveOptions.SetImageResample(96, 80);

wb.Save("output.pdf", pdfSaveOptions);
```

### Voir aussi

* class [GridPdfSaveOptions](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


