---
title: "SpinButtonActiveXControl.Max"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "SpinButtonActiveXControl property. Ottiene e imposta il valore massimo accettabile"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/max/
---
## SpinButtonActiveXControl.Max property

Ottiene e imposta il valore massimo accettabile.

```csharp
public int Max { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyMaxDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un controllo ActiveX SpinButton al foglio di lavoro
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 1, 1, 1, 100, 30);
            
            // Ottieni il controllo ActiveX e imposta la sua proprietà Max
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.Max = 100;
            
            // Salva la cartella di lavoro
            workbook.Save("SpinButtonMaxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


