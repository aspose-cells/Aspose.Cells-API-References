---
title: "SpinButtonActiveXControl.Orientation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "SpinButtonActiveXControl property. Ottiene e imposta se lo SpinButton o lo ScrollBar è orientato verticalmente o orizzontalmente"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/orientation/
---
## SpinButtonActiveXControl.Orientation property

Ottiene e imposta se lo SpinButton o lo ScrollBar è orientato verticalmente o orizzontalmente.

```csharp
public ControlScrollOrientation Orientation { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyOrientationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX SpinButton
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 1, 1, 100, 50, 100, 50);
            SpinButtonActiveXControl spinButton = (SpinButtonActiveXControl)shape.ActiveXControl;

            // Verifica e modifica l'orientamento
            if (spinButton.Orientation == ControlScrollOrientation.Auto)
            {
                spinButton.Orientation = ControlScrollOrientation.Horizontal;
            }

            // Salva la cartella di lavoro
            workbook.Save("SpinButtonOrientationDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ControlScrollOrientation](../../controlscrollorientation/)
* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


