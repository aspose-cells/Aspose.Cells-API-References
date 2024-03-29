---
title: ToTiff
second_title: Référence de l'API Aspose.Cells pour .NET
description: Rendre la feuille de calcul entière en tant quimage Tiff à diffuser.
type: docs
weight: 80
url: /fr/net/aspose.cells.rendering/sheetrender/totiff/
---
## ToTiff(Stream) {#totiff}

Rendre la feuille de calcul entière en tant qu'image Tiff à diffuser.

```csharp
public void ToTiff(Stream stream)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| stream | Stream | le flux de l'image de sortie |

### Voir également

* class [SheetRender](../../sheetrender)
* espace de noms [Aspose.Cells.Rendering](../../sheetrender)
* Assemblée [Aspose.Cells](../../../)

---

## ToTiff(string) {#totiff_1}

Rendre la feuille de calcul entière en tant qu'image Tiff dans un fichier.

```csharp
public void ToTiff(string filename)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| filename | String | le nom de fichier de l'image de sortie |

### Exemples

Le code suivant sort toutes les pages de la première feuille en image Tiff.

```csharp
// charge le fichier source avec des images.
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

// définit le type d'image de sortie.
imgOpt.SaveFormat = SaveFormat.Tiff;

// rend la première feuille.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

// affiche toutes les pages de la feuille sur l'image Tiff.
sr.ToTiff("output.tiff");
```

### Voir également

* class [SheetRender](../../sheetrender)
* espace de noms [Aspose.Cells.Rendering](../../sheetrender)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
