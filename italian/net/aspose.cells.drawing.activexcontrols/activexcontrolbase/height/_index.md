---
title: "ActiveXControlBase.Height"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ActiveXControlBase. Ottiene e imposta l'altezza del controllo in unità di punti"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/height/
---
## ActiveXControlBase.Height property

Ottiene e imposta l'altezza del controllo in unità di punti.

```csharp
public virtual double Height { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyHeightDemo
    {
        public static void Run()
        {
            // Inizializza una nuova cartella di lavoro
            Workbook workbook = new Workbook();

            // Aggiungi un RadioButton ActiveXControl
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 0, 100, 50);
            RadioButtonActiveXControl activeXControl = (RadioButtonActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà di base
            activeXControl.Caption = "Height Demo";
            activeXControl.IsAutoSize = false; // Disable auto-size to demonstrate Height property

            // Dimostra la proprietà Height
            Console.WriteLine("Original Height: " + activeXControl.Height);
            activeXControl.Height = 75;
            Console.WriteLine("Modified Height: " + activeXControl.Height);

            // Salva la cartella di lavoro
            workbook.Save("ActiveXControlHeightDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


