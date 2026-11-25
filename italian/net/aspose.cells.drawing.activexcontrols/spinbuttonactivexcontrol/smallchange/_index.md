---
title: "SpinButtonActiveXControl.SmallChange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "SpinButtonActiveXControl property. Ottiene e imposta la quantità di cui la proprietà Position cambia"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/smallchange/
---
## SpinButtonActiveXControl.SmallChange property

Ottiene e imposta la quantità di variazione della proprietà Position

```csharp
public int SmallChange { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertySmallChangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un controllo ActiveX SpinButton al foglio di lavoro
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 0, 1, 0, 100, 30);
            
            // Ottieni il controllo ActiveX e imposta la proprietà SmallChange
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.SmallChange = 5;
            
            // Salva la cartella di lavoro
            workbook.Save("SpinButtonSmallChangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


