---
title: "ToggleButtonActiveXControl.PicturePosition"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ToggleButtonActiveXControl. Obtient et définit l'emplacement de l'image du contrôle par rapport à sa légende"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/pictureposition/
---
## ToggleButtonActiveXControl.PicturePosition property

Obtient et définit l'emplacement de l'image du contrôle par rapport à sa légende.

```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyPicturePositionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez un contrôle ActiveX ToggleButton avec tous les paramètres requis
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 100, 30, 0);
            var control = shape.ActiveXControl;

            if (control is ToggleButtonActiveXControl toggleButton)
            {
                // Définir la propriété PicturePosition
                toggleButton.PicturePosition = ControlPicturePositionType.AboveLeft;

                // Définir d'autres propriétés pour démontrer la fonctionnalité
                toggleButton.Caption = "Toggle Button";
                toggleButton.Picture = new byte[0]; // Empty picture for demo
            }

            // Enregistrez le classeur
            workbook.Save("ToggleButtonActiveXControlDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


