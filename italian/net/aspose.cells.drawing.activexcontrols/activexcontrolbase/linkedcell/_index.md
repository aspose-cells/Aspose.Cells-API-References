---
title: "ActiveXControlBase.LinkedCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ActiveXControlBase proprietà. Ottiene e imposta la cella collegata"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/
---
## ActiveXControlBase.LinkedCell property

Ottiene e imposta la cella collegata.

```csharp
public string LinkedCell { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyLinkedCellDemo
    {
        public static void Run()
        {
            // Inizializza una nuova cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Aggiungere un SpinButtonActiveXControl al primo foglio di lavoro
            Aspose.Cells.Drawing.Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 
                10, 10, 100, 30, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl spinButton = 
                (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;

            // Configurare le proprietà del pulsante spin
            spinButton.Min = 0;
            spinButton.Max = 100;
            spinButton.Position = 50;
            spinButton.SmallChange = 1;

            // Collegare il controllo alla cella A1
            spinButton.LinkedCell = "A1";

            // Impostare il valore della cella A1 per corrispondere alla posizione iniziale
            workbook.Worksheets[0].Cells["A1"].PutValue(spinButton.Position);

            // Salva la cartella di lavoro
            workbook.Save("LinkedCellDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


