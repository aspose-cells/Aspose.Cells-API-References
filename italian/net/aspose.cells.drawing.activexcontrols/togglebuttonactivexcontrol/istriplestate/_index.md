---
title: "ToggleButtonActiveXControl.IsTripleState"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ToggleButtonActiveXControl. Indica come il controllo specificato visualizzerà i valori Null"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/istriplestate/
---
## ToggleButtonActiveXControl.IsTripleState property

Indica come il controllo specificato visualizzerà i valori Null.

```csharp
public bool IsTripleState { get; set; }
```

### Osservazioni

| **Impostazione** | **Description** |
| --- | --- |
| True | Il controllo ciclerà attraverso gli stati per i valori Sì, No e Null. Il controllo appare attenuato (grigio) quando la sua proprietà Value è impostata su Null. |
| False | (Predefinito) Il controllo ciclerà attraverso gli stati per i valori Sì e No. I valori Null vengono visualizzati come se fossero valori No. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyIsTripleStateDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX ToggleButton
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ToggleButton, 1, 0, 1, 0, 100, 30);
            var toggleButton = (Aspose.Cells.Drawing.ActiveXControls.ToggleButtonActiveXControl)shape.ActiveXControl;

            // Imposta la proprietà IsTripleState su true
            toggleButton.IsTripleState = true;
            Console.WriteLine("ToggleButton IsTripleState: " + toggleButton.IsTripleState);

            // Modifica la proprietà IsTripleState su false
            toggleButton.IsTripleState = false;
            Console.WriteLine("ToggleButton IsTripleState: " + toggleButton.IsTripleState);

            // Salva la cartella di lavoro
            workbook.Save("ToggleButtonIsTripleStateDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


