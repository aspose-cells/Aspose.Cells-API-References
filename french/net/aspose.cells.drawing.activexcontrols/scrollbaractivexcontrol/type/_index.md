---
title: "ScrollBarActiveXControl.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ScrollBarActiveXControl. Obtient le type du contrôle ActiveX"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/type/
---
## ScrollBarActiveXControl.Type property

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
    public class ScrollBarActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez un contrôle ActiveX ScrollBar avec les paramètres corrects
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 1, 1, 100, 20, 0);
            ScrollBarActiveXControl scrollBar = (ScrollBarActiveXControl)shape.ActiveXControl;

            // Vérifiez le type du contrôle en utilisant la propriété Type
            if (scrollBar.Type == ControlType.ScrollBar)
            {
                // Définissez les propriétés spécifiques du ScrollBar
                scrollBar.Max = 100;
                scrollBar.Min = 0;
                scrollBar.Position = 50;
            }

            // Enregistrez le classeur
            workbook.Save("ScrollBarActiveXControlDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ControlType](../../controltype/)
* class [ScrollBarActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


