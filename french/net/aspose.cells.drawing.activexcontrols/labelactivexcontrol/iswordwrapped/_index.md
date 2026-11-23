---
title: "LabelActiveXControl.IsWordWrapped"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LabelActiveXControl. Indique si le contenu du contrôle se renvoie automatiquement à la fin d’une ligne"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/iswordwrapped/
---
## LabelActiveXControl.IsWordWrapped property

Indique si le contenu du contrôle passe automatiquement à la ligne à la fin d'une ligne.

```csharp
public bool IsWordWrapped { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyIsWordWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.Label, 5, 0, 1, 1, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.LabelActiveXControl label = (Aspose.Cells.Drawing.ActiveXControls.LabelActiveXControl)shape.ActiveXControl;

            label.Caption = "This is a long text that will demonstrate word wrapping when IsWordWrapped is set to true";
            label.IsWordWrapped = true;
            label.IsAutoSize = true;

            Console.WriteLine("Label IsWordWrapped: " + label.IsWordWrapped);
            Console.WriteLine("Label Caption: " + label.Caption);

            workbook.Save("LabelActiveXControlIsWordWrappedDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


