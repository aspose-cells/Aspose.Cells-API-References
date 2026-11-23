---
title: "GridSheetRender.ToTiff"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "méthode GridSheetRender. Rendre toute la feuille de calcul en image Tiff vers le flux."
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridsheetrender/totiff/
---
## ToTiff(Stream) {#totiff}

Rendre toute la feuille de calcul en image Tiff vers le flux.

```csharp
public void ToTiff(Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | le flux de l'image de sortie |

### Voir aussi

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToTiff(string) {#totiff_1}

Rendre toute la feuille de calcul en image Tiff vers un fichier.

```csharp
public void ToTiff(string filename)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| nom de fichier | String | le nom de fichier de l'image de sortie |

### Exemples

Le code suivant génère toutes les pages de la première feuille en image Tiff.

```csharp
//chargez le fichier source avec les images.
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

//définir le type d'image de sortie.
imgOpt.SaveFormat = SaveFormat.Tiff;

//rendre la première feuille.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

//générer toutes les pages de la feuille en image Tiff.
sr.ToTiff("output.tiff");
```

### Voir aussi

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


