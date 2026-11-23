---
title: "CommandButtonActiveXControl.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "CommandButtonActiveXControl propriété. Obtient le type du contrôle ActiveX"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/type/
---
## CommandButtonActiveXControl.Type property

Obtient le type du contrôle ActiveX.

```csharp
public override ControlType Type { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CommandButtonActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un bouton de commande avec la liste complète des paramètres
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.CommandButton,
                0,  // topRow
                0,  // top
                0,  // leftColumn
                0,  // left
                100,  // width
                100  // height
            );
            var control = (CommandButtonActiveXControl)shape.ActiveXControl;

            control.Caption = "CommandButton1";
            control.PicturePosition = ControlPicturePositionType.AboveCenter;
            control.Accelerator = (char)0;
            control.TakeFocusOnClick = false;
            control.IsWordWrapped = false;
            control.IsEnabled = true;

            Console.WriteLine($"Control Type: {control.Type}");
            Console.WriteLine($"Is CommandButton type: {control.Type == ControlType.CommandButton}");

            workbook.Save("CommandButtonDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ControlType](../../controltype/)
* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


