---
title: "ImageActiveXControl.Picture"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageActiveXControl. Obtient et définit les données de l'image"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picture/
---
## ImageActiveXControl.Picture property

Obtient et définit les données de l'image.

```csharp
public byte[] Picture { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX Image
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 100, 100, 100, 100);
            ImageActiveXControl imgControl = (ImageActiveXControl)shape.ActiveXControl;

            // Définir les propriétés
            imgControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
            imgControl.PictureAlignment = ControlPictureAlignmentType.TopLeft;
            imgControl.IsTiled = false;

            // Définir la propriété Picture (en utilisant un tableau d'octets d'image d'exemple)
            byte[] imageData = new byte[] { 0x00, 0x01, 0x02 }; // Sample image data
            imgControl.Picture = imageData;

            // Vérifier que la propriété Picture a été définie
            Console.WriteLine("Picture data length: " + imgControl.Picture.Length);

            // Enregistrez le classeur
            workbook.Save("ImageActiveXControlDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


