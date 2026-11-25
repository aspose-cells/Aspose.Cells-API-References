---
title: "SpinButtonActiveXControl.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "SpinButtonActiveXControl property. Ottiene il tipo del controllo ActiveX"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/type/
---
## SpinButtonActiveXControl.Type property

Ottiene il tipo del controllo ActiveX.

```csharp
public override ControlType Type { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un controllo SpinButton ActiveX (parametri: left, top, width, height)
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 1, 1, 100, 30, 100, 30);
            SpinButtonActiveXControl spinButton = (SpinButtonActiveXControl)shape.ActiveXControl;
            
            // Verifica il tipo di controllo usando la proprietà Type
            if (spinButton.Type == ControlType.SpinButton)
            {
                // Imposta alcune proprietà specifiche per SpinButton
                spinButton.Min = 0;
                spinButton.Max = 100;
                spinButton.Position = 50;
                spinButton.SmallChange = 1;
            }
            
            // Salva la cartella di lavoro
            workbook.Save("SpinButtonActiveXControlDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ControlType](../../controltype/)
* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


