---
title: "ImageActiveXControl.PictureSizeMode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageActiveXControl. Obtient et définit la façon d'afficher l'image"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picturesizemode/
---
## ImageActiveXControl.PictureSizeMode property

Obtient et définit comment afficher l'image.

```csharp
public ControlPictureSizeMode PictureSizeMode { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyPictureSizeModeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez un contrôle Image ActiveX à la feuille de calcul
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 200, 200, 0, 0);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Définir PictureSizeMode et d'autres propriétés
            imageControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
            
            // Charger une image d'exemple (remplacez par le chemin de votre propre image)
            string imagePath = "sample.jpg";
            if (File.Exists(imagePath))
            {
                byte[] imageData = File.ReadAllBytes(imagePath);
                imageControl.Picture = imageData;
            }

            // Enregistrez le classeur
            workbook.Save("ImageActiveXControlDemo.xlsx");

            // Afficher la valeur de PictureSizeMode
            Console.WriteLine($"PictureSizeMode: {imageControl.PictureSizeMode}");
        }
    }
}
```

### Voir aussi

* enum [ControlPictureSizeMode](../../controlpicturesizemode/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


