---
title: "SpinButtonActiveXControl.Min"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SpinButtonActiveXControl. Ottiene e imposta il valore minimo accettabile"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/min/
---
## SpinButtonActiveXControl.Min property

Ottiene e imposta il valore minimo accettabile.

```csharp
public int Min { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyMinDemo
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
            Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl spinButton = 
                (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            
            // Imposta la proprietà Min del SpinButton
            spinButton.Min = 0;
            
            // Imposta altre proprietà per dimostrare la funzionalità
            spinButton.Max = 100;
            spinButton.Position = 50;
            
            // Salva la cartella di lavoro
            workbook.Save("SpinButtonMinDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


