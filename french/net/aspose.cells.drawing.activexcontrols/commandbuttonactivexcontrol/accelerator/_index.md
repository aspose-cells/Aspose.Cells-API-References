---
title: "CommandButtonActiveXControl.Accelerator"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CommandButtonActiveXControl. Obtient et définit la touche d'accélérateur pour le contrôle"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/accelerator/
---
## CommandButtonActiveXControl.Accelerator property

Obtient et définit la touche d'accélérateur pour le contrôle.

```csharp
public char Accelerator { get; set; }
```

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CommandButtonActiveXControlPropertyAcceleratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            Shape shape = sheet.Shapes.AddActiveXControl(ControlType.CommandButton, 0, 0, 0, 0, 30, 100);
            CommandButtonActiveXControl button = (CommandButtonActiveXControl)shape.ActiveXControl;

            button.Caption = "CommandButton1";
            button.Accelerator = 'A';
            button.PicturePosition = ControlPicturePositionType.AboveCenter;
            button.IsEnabled = true;

            workbook.Save("CommandButtonAcceleratorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


