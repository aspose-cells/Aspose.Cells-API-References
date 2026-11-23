---
title: "LabelActiveXControl.Picture"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "LabelActiveXControl propriété. Obtient et définit les données de l'image"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/picture/
---
## LabelActiveXControl.Picture property

Obtient et définit les données de l'image.

```csharp
public byte[] Picture { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.IO;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX Label
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 1, 1, 1, 1, 100, 50);
            LabelActiveXControl labelControl = (LabelActiveXControl)shape.ActiveXControl;

            // Définir les propriétés de base
            labelControl.Caption = "Sample Label";
            labelControl.PicturePosition = ControlPicturePositionType.LeftTop;

            // Charger une image pour la propriété Picture
            string imagePath = "sample.jpg"; // Replace with actual image path
            if (File.Exists(imagePath))
            {
                labelControl.Picture = File.ReadAllBytes(imagePath);
                Console.WriteLine("Picture set successfully");
            }
            else
            {
                Console.WriteLine("Image file not found, using null picture");
                labelControl.Picture = null;
            }

            // Enregistrez le classeur
            workbook.Save("LabelActiveXControlDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


