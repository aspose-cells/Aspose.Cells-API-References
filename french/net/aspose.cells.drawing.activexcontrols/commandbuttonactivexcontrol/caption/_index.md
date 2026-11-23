---
title: "CommandButtonActiveXControl.Caption"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CommandButtonActiveXControl. Obtient et définit le texte descriptif qui apparaît sur un contrôle"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/caption/
---
## CommandButtonActiveXControl.Caption property

Obtient et définit le texte descriptif qui apparaît sur un contrôle.

```csharp
public string Caption { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CommandButtonActiveXControlPropertyCaptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CommandButton, 2, 2, 2, 2, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.CommandButtonActiveXControl commandButton = (Aspose.Cells.Drawing.ActiveXControls.CommandButtonActiveXControl)shape.ActiveXControl;

            // Démontrez l'utilisation de la propriété Caption
            commandButton.Caption = "Click Me";
            commandButton.Width = 150;
            commandButton.Height = 50;
            commandButton.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Blue);

            workbook.Save("CommandButtonCaptionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


