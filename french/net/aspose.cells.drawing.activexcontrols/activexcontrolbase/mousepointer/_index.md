---
title: "ActiveXControlBase.MousePointer"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ActiveXControlBase. Obtient et définit le type d'icône affiché comme pointeur de souris pour le contrôle"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/
---
## ActiveXControlBase.MousePointer property

Obtient et définit le type d'icône affichée comme pointeur de la souris pour le contrôle.

```csharp
public ControlMousePointerType MousePointer { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyMousePointerDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(ControlType.CommandButton, 1, 0, 1, 0, 100, 50);
            CommandButtonActiveXControl button = (CommandButtonActiveXControl)shape.ActiveXControl;

            button.Caption = "Click Me";
            button.MousePointer = ControlMousePointerType.Help;
            button.MouseIcon = new byte[] { }; // Empty byte array for custom icon (when MousePointer is Custom)
            
            workbook.Save("ActiveXControlMousePointerDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ControlMousePointerType](../../controlmousepointertype/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


