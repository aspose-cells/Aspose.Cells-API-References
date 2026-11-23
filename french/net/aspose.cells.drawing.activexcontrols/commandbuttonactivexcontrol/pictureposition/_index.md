---
title: "CommandButtonActiveXControl.PicturePosition"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CommandButtonActiveXControl. Obtient et définit l'emplacement de l'image du contrôle par rapport à sa légende"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/pictureposition/
---
## CommandButtonActiveXControl.PicturePosition property

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
    public class CommandButtonActiveXControlPropertyPicturePositionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 2, 2, 2, 2, 100, 30);
            CommandButtonActiveXControl commandButton = (CommandButtonActiveXControl)shape.ActiveXControl;

            commandButton.Caption = "Click Me";
            commandButton.PicturePosition = ControlPicturePositionType.Center;
            
            workbook.Save("CommandButtonWithPicturePosition.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


