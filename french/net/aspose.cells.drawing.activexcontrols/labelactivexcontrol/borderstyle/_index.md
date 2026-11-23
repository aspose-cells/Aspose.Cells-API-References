---
title: "LabelActiveXControl.BorderStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "LabelActiveXControl propriété. Obtient et définit le type de bordure utilisé par le contrôle"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/borderstyle/
---
## LabelActiveXControl.BorderStyle property

Obtient et définit le type de bordure utilisé par le contrôle.

```csharp
public ControlBorderType BorderStyle { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyBorderStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 5, 0, 1, 1, 100, 20);
            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            label.Caption = "Border Style Demo";
            label.BorderStyle = ControlBorderType.Single;
            label.BorderOleColor = 0xFF0000; // Red border

            Console.WriteLine("Label Border Style: " + label.BorderStyle);
            Console.WriteLine("Label Border Color: " + label.BorderOleColor);

            workbook.Save("LabelBorderStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ControlBorderType](../../controlbordertype/)
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


