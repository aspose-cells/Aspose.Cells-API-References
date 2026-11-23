---
title: "Classe MsoFormatPicture"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.MsoFormatPicture. Représente le format d'image"
type: docs
url: /fr/net/aspose.cells.drawing/msoformatpicture/
---
## MsoFormatPicture class

Représente le format d'image.

```csharp
public class MsoFormatPicture
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BottomCrop](../../aspose.cells.drawing/msoformatpicture/bottomcrop/) { get; set; } | Représente l'emplacement du bas du rectangle de recadrage exprimé comme un ratio de la hauteur de l'image. |
| [BottomCropInch](../../aspose.cells.drawing/msoformatpicture/bottomcropinch/) { get; set; } | Représente l'emplacement du bas du rectangle de recadrage exprimé en pouces. |
| [Brightness](../../aspose.cells.drawing/msoformatpicture/brightness/) { get; set; } | Représente la modification de la luminosité de l'image en pourcentage. |
| [Contrast](../../aspose.cells.drawing/msoformatpicture/contrast/) { get; set; } | Représente la modification du contraste de l'image en pourcentage. |
| [Gamma](../../aspose.cells.drawing/msoformatpicture/gamma/) { get; set; } | Représente le gamma de l'image. |
| [IsBiLevel](../../aspose.cells.drawing/msoformatpicture/isbilevel/) { get; set; } | Indique si cette image doit être affichée en noir et blanc à deux couleurs. |
| [IsGray](../../aspose.cells.drawing/msoformatpicture/isgray/) { get; set; } | Indique si cette image doit être affichée en niveaux de gris. |
| [LeftCrop](../../aspose.cells.drawing/msoformatpicture/leftcrop/) { get; set; } | Représente l'emplacement du côté gauche du rectangle de recadrage exprimé comme un ratio de la largeur de l'image. |
| [LeftCropInch](../../aspose.cells.drawing/msoformatpicture/leftcropinch/) { get; set; } | Représente l'emplacement du côté gauche du rectangle de recadrage exprimé en pouces. |
| [RightCrop](../../aspose.cells.drawing/msoformatpicture/rightcrop/) { get; set; } | Représente l'emplacement du côté droit du rectangle de recadrage exprimé comme un ratio de la largeur de l'image. |
| [RightCropInch](../../aspose.cells.drawing/msoformatpicture/rightcropinch/) { get; set; } | Représente l'emplacement du côté droit du rectangle de recadrage exprimé en pouces. |
| [TopCrop](../../aspose.cells.drawing/msoformatpicture/topcrop/) { get; set; } | Représente l'emplacement du haut du rectangle de recadrage exprimé comme un ratio de la hauteur de l'image. |
| [TopCropInch](../../aspose.cells.drawing/msoformatpicture/topcropinch/) { get; set; } | Représente l'emplacement du haut du rectangle de recadrage exprimé en pouces. |
| [Transparency](../../aspose.cells.drawing/msoformatpicture/transparency/) { get; set; } | Renvoie ou définit le degré de transparence de la zone comme une valeur de 0,0 (opaque) à 1,0 (transparent). |
| [TransparentColor](../../aspose.cells.drawing/msoformatpicture/transparentcolor/) { get; set; } | Obtient et définit la couleur transparente de l'image. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/msoformatpicture/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/msoformatpicture/gethashcode/)() | Obtient le code de hachage. |

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPictureDemo
    {
        public static void RunDemo()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter une image à la feuille de calcul
            int pictureIndex = sheet.Pictures.Add(5, 5, "MsoFormatPictureDemo.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // Accédez à l'objet MsoFormatPicture
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // Définissez les propriétés de MsoFormatPicture
            formatPicture.TopCropInch = 0.5;
            formatPicture.BottomCropInch = 0.5;
            formatPicture.LeftCropInch = 0.5;
            formatPicture.RightCropInch = 0.5;
            formatPicture.Transparency = 0.5;
            formatPicture.Contrast = 0.8;
            formatPicture.Brightness = 0.6;
            formatPicture.Gamma = 1.0;
            formatPicture.IsBiLevel = false;
            formatPicture.IsGray = false;

            // Définissez la couleur transparente
            CellsColor transparentColor = workbook.CreateCellsColor();
            transparentColor.Color = Color.White;
            formatPicture.TransparentColor = transparentColor;

            // Enregistrez le classeur
            workbook.Save("MsoFormatPictureDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


