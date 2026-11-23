---
title: "Enumération ControlPictureSizeMode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode enum. Représente la façon d'afficher l'image."
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/controlpicturesizemode/
---
## ControlPictureSizeMode enumeration

Représente la façon d'afficher l'image.

```csharp
public enum ControlPictureSizeMode
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Clip | `0` | Recadre toute partie de l'image qui dépasse les limites du contrôle. |
| Stretch | `1` | Étire l'image pour remplir la zone du contrôle. Ce réglage déforme l'image dans la direction horizontale ou verticale. |
| Zoom | `3` | Agrandit l'image, mais ne la déforme pas dans la direction horizontale ou verticale. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System.IO;

    public class ControlPictureSizeModeDemo
    {
        public static void ControlPictureSizeModeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une image à la feuille de calcul
            int pictureIndex = worksheet.Pictures.Add(1, 1, "ControlPictureSizeMode.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Ajouter un ImageActiveXControl à la feuille de calcul
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 5, 5,5,100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Définir les données d'image pour le ImageActiveXControl
            imageControl.Picture = File.ReadAllBytes("ControlPictureSizeMode.png");

            // Définir le PictureSizeMode sur Zoom
            imageControl.PictureSizeMode = ControlPictureSizeMode.Zoom;

            // Définir d'autres propriétés de l'ImageActiveXControl
            imageControl.IsAutoSize = true;
            imageControl.BorderStyle = ControlBorderType.Single;
            imageControl.BorderOleColor = 0x000000; // Black color
            imageControl.SpecialEffect = ControlSpecialEffectType.Flat;
            imageControl.PictureAlignment = ControlPictureAlignmentType.Center;
            imageControl.IsTiled = false;

            // Enregistrez le classeur
            workbook.Save("ControlPictureSizeModeExample.xlsx");
            workbook.Save("ControlPictureSizeModeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


