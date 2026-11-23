---
title: "CommandButtonActiveXControl.Picture"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CommandButtonActiveXControl. Obtient et définit les données de l'image"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/picture/
---
## CommandButtonActiveXControl.Picture property

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
    public class CommandButtonActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une forme pour héberger le contrôle ActiveX avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.CommandButton, 
                1,  // top row
                1,  // left column
                0,  // top position
                0,  // left position
                100, // width
                30); // height
                
            CommandButtonActiveXControl button = (CommandButtonActiveXControl)shape.ActiveXControl;

            // Définir les propriétés
            button.Caption = "Click Me";
            button.PicturePosition = ControlPicturePositionType.AboveCenter;

            // Définissez l'image (un tableau d'octets vide représente aucune image)
            button.Picture = new byte[0];

            // Enregistrez le classeur
            workbook.Save("CommandButtonWithPicture.xlsx");

            // Vérifiez la propriété Picture
            Console.WriteLine("Picture is null: " + (button.Picture == null));
        }
    }
}
```

### Voir aussi

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


