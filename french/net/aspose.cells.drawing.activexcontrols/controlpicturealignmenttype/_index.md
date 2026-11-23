---
title: "Énumération ControlPictureAlignmentType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType. Représente l'alignement de l'image à l'intérieur du formulaire ou de l'image"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/controlpicturealignmenttype/
---
## ControlPictureAlignmentType enumeration

Représente l'alignement de l'image à l'intérieur du Formulaire ou de l'Image.

```csharp
public enum ControlPictureAlignmentType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| TopLeft | `0` | Le coin supérieur gauche. |
| TopRight | `1` | Le coin supérieur droit. |
| Center | `2` | Le centre. |
| BottomLeft | `3` | Le coin inférieur gauche. |
| BottomRight | `4` | Le coin inférieur droit. |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlsClassControlPictureAlignmentTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un ImageActiveXControl avec tous les paramètres requis
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 
                10,  // left
                10,  // top
                200, // width
                200, // height
                0,   // imageWidth
                0    // imageHeight
            );
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = 
                (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            // Définir les propriétés de l'image
            imageControl.Picture = File.ReadAllBytes("sample.png");
            imageControl.PictureAlignment = Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType.Center;
            imageControl.PictureSizeMode = Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode.Stretch;

            // Enregistrez le classeur
            workbook.Save("ImageControlDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


