---
title: "ImageActiveXControl.PictureAlignment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageActiveXControl. Obtient et définit l'alignement de l'image à l'intérieur du formulaire ou de l'image"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picturealignment/
---
## ImageActiveXControl.PictureAlignment property

Obtient et définit l'alignement de l'image à l'intérieur du Form ou de l'Image.

```csharp
public ControlPictureAlignmentType PictureAlignment { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyPictureAlignmentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 5, 0, 1, 1, 100, 100);
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            // Définir la propriété PictureAlignment
            imageControl.PictureAlignment = Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType.Center;

            // Charger une image d'exemple (remplacez par le chemin réel de l'image)
            string imagePath = "sample.jpg";
            if (File.Exists(imagePath))
            {
                byte[] imageData = File.ReadAllBytes(imagePath);
                imageControl.Picture = imageData;
            }

            workbook.Save("ImageActiveXControlDemo.xlsx");

            Console.WriteLine($"PictureAlignment: {imageControl.PictureAlignment}");
        }
    }
}
```

### Voir aussi

* enum [ControlPictureAlignmentType](../../controlpicturealignmenttype/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


